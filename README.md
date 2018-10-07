# Hello-World
Just my first repository

#Problem FizzBuzz

(1..50).each do |n|
n
  if n % 15 == 0
  puts "FizzBuzz"
  end
  if n % 3 == 0
  n = "Fizz"
  end
  if n % 5 == 0 
  puts "Buzz"
  else puts n
  end
end


#the vowel game
puts "Enter text here: "

game = gets.chomp


char = game.split('')

count = 0

char.each do |x|
  if x == "a"
  count += 1
  end
  if x == "e"
  count += 1
  end
  if x == "i"
  count += 1
  end
  if x == "o"
  count += 1
  end
  if x == "u"
  count += 1
  end
end

puts count


#Who are you and where you from?

print "What's your first name? "
first_name = gets.chomp
first_name.capitalize!

print "What's your last name? "
last_name = gets.chomp
last_name.capitalize!

print "What's your city? "
city = gets.chomp
city.capitalize!

print "What's your state? "
state = gets.chomp
state.upcase!

puts "Your name is #{first_name} #{last_name} and you are from #{city}, #{state}."

#Daffy Duck

print "Enter input: "
user_input = gets.chomp
user_input.downcase!

if user_input.include? "s"
  user_input.gsub!(/s/, "th")
else puts "Nothing to do here!"
end

user_input.capitalize!

puts user_input



#loop practices

i = 0

=begin
while i < 5
  i += 1
  print "Ruby!"
end
=end

=begin
loop do
  i += 1
  print "Hello"
  break if i == 5
end
=end

=begin
b = [1, 2, 3, 4, 5]

b.each do
  print "Ruby"
end
=end

=begin
g = 0
until g == 5
  g += 1
  print "Bell"
end
=end

=begin
i = "Jello"

5.times do 
  print i
end
=end

=begin
for i in 1..5
  print "Gem"
end
=end


#Redacted text

puts "Enter text: "
text = gets.chomp
text.downcase!

puts "Enter redacted: "
redacted = gets.chomp
redacted.downcase!

words = text.split (" ")
words.each do |x|
  if x == redacted
    print "REDACTED "
  else print x + " "
  end
end


#word count code

puts "Enter text here: "
text = gets.chomp

words = text.split

frequencies = Hash.new(0)

words.each do |word|
  frequencies[word] += 1
end

frequencies = frequencies.sort_by do |word, count|
  count
end

frequencies.reverse!

frequencies.each do |k,v|
  puts k + " " + v.to_s
end
