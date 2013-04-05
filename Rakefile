
task :site_name do
  STDOUT.puts "Yo champ, what do you want to name your blog?"
  input = STDIN.gets.strip

  update_content(
    '_includes/header.html',
    '%site-name',
    input,
    "awesome name!"
  )

  update_content(
    '_includes/site-credits.html',
    '%site-name',
    input,
    ""
  )

  update_content(
    'index.html',
    '%site-name',
    input,
    ""
  )
end

task :site_strap do
  STDOUT.puts "And something for a strapline? Or even your job title.."
  input = STDIN.gets.strip

  update_content(
    '_includes/header.html',
    '%site-strap',
    input,
    "... Nicely put"
  )

end

task :about do
  STDOUT.puts "Ok, tell me about yourself in a few paragraphs..."
  input = STDIN.gets.strip

  update_content(
    '_includes/footer.html',
    '%about',
    input,
    "smooth operator.."
  )

end

task :twitter do
  STDOUT.puts "What is your twitter username?"
  input = STDIN.gets.strip

  update_content(
    '_includes/site-credits.html',
    '%twitter-name',
    input,
    "AWESOME!! You've not got yourself a follow button :)"
  )

end

task :analytics do
  STDOUT.puts "And to finish.. Whats your Google Analytics ID"
  input = STDIN.gets.strip

  update_content(
    '_includes/google_analytics.html',
    'xxxxxxx',
    input,
    "AWESOME!! That's it, all sorted. Go write some great articles!"
  )

end

task :build => [:site_name, :site_strap, :about, :twitter, :analytics] do

end

def update_content(filepath, phrase, input, response)

  text = File.read(filepath)
  replace = text.gsub(/#{phrase}/, input)
  File.open(filepath, "w") {|file| file.puts replace}
  puts response
end
