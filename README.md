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

game = "The vowel game. This is my first try."

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
