require 'rubygems'
require 'rake'

editor  = ENV["EDITOR"] || ""

task :default => :build

desc "Switch between Jekyll-bootstrap themes."
task :switch_theme, :theme do |t, args|
  theme_path = File.join(File.dirname(__FILE__), "_includes", "themes", args.theme)
  layouts_path = File.join(File.dirname(__FILE__), "_layouts")
  
  abort("rake aborted: './_includes/themes/#{args.theme}' directory not found.") unless Dir.exists?(theme_path)
  abort("rake aborted: './_layouts' directory not found.") unless Dir.exists?(layouts_path)
  
  Dir.glob("#{theme_path}/*") do |filename|
    puts "Generating '#{args.theme}' layout: #{File.basename(filename)}"
    
    open("#{layouts_path}/#{File.basename(filename)}", 'w') do |page|
      if File.basename(filename, ".html").downcase == "default"
        page.puts "---"
        page.puts "---"
        page.puts "{% assign theme_asset_path = \"/assets/themes/#{args.theme}\" %}"
      else
        page.puts "---"
        page.puts "layout: default"
        page.puts "---"
      end 
      page.puts "{% include themes/#{args.theme}/#{File.basename(filename)} %}" 
    end
  end
end # task :switch_theme

desc 'Clean up generated site'
task :clean do
  sh 'rm -rf _site'
end

desc 'Test site output for Liquid template errors'
task :test => :build do
  errors = `grep --exclude Rakefile -R 'Liquid error:' _site`
  if errors.nil? || errors.empty?
    puts "No errors"
  else
    puts "Errors:"
    puts errors.inspect
    exit 1
  end
end

desc 'Build site with Jekyll'
task :build => :clean do
  system "jekyll #('--lsi')"
end

desc 'Start server with --auto'
task :server => :clean do
  system "jekyll --server --auto"
end

desc 'Make a new status post'
task :status, [:name] do |t, args|
  if args.name then
    template(args.name, "status")
  else
    puts "Name required"
  end
end

def template(name, type)
  t = Time.now
  contents = "" # otherwise using it below will be badly scoped
  File.open("_posts/yyyy-mm-dd-template-#{type}.md", "rb") do |f|
    contents = f.read
  end
  contents = contents.sub("%date%", t.strftime("%Y-%m-%d %H:%M:%S %z")).sub("%title%", name)
  filename = "_posts/" + t.strftime("%Y-%m-%d-") + name + '.md'
  if File.exists? filename then
    puts "Post already exists: #{filename}"
    return
  end
  File.open(filename, "wb") do |f|
    f.write contents
  end
  puts "created #{filename}"
end

desc "list tasks"
task :list do
  puts "Tasks: #{(Rake::Task.tasks - [Rake::Task[:list]]).join(', ')}"
  puts "(type rake -T for more detail)\n\n"
end