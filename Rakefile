task :todo do
  num = 0

  File.read("article.txt").lines do |line|
    num += 1
    puts "#{num}: #{line}" if line =~ /TODO:/
  end
end
