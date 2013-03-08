
task :build do
  STDOUT.puts "Yo champ, whats the name of your blog?"
  input = STDIN.gets.strip

  filepath = '_includes/header.html'
  text = File.read(filepath)
  replace = text.gsub(/%site-name/, input)
  File.open(filepath, "w") {|file| file.puts replace}

  puts "awesome, ok moving on."
  Rake::Task["strapline"].reenable
  Rake::Task["strapline"].invoke
end

task :strapline do
  STDOUT.puts "How about a strapline"
  input = STDIN.gets.strip

  filepath = '_includes/header.html'
  text = File.read(filepath)
  replace = text.gsub(/%strapline/, input)
  File.open(filepath, "w") {|file| file.puts replace}
end