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
