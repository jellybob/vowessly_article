task :todo do
  num = 0

  File.read("article.txt").lines do |line|
    num += 1
    puts "#{num}: #{line}" if line =~ /TODO:/
  end
end

task :count do
  puts %x{cat article.txt | wc -w}
end

task :build do
  %x{markdown article.txt > article.html}
end

task :default => :build
