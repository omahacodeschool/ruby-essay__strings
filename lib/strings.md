---
title: Strings
instructor_notes: Feel free to re-organize the headings (or add/remove headings) below. We included the headings for your benefit, but it's 100% fine if you want to write your responses in some different structure.
---

# What is a String?

A string is a sequence within single or double quotes that can hold virtually any combination of characters, often representing human language. Ruby can 

# What are some examples of information that would be Strings as opposed to some other data type?

Names of people, places, things, ideas, nonsense combinations of letters, numbers that are part of a name (example: 1812 Overture), 

# What is one way, using Ruby, to retrieve the 6th character in a String like `"Ada Lovelace"`? How about the 8th character? What happens if you try to retrieve the value of the _99th_ character (Or any character that doesn't exist)?

Learned a new method, "byteslice," that seems to do exactly that. 
My little test program from repl.it - Ruby:

Ham = "Hamilton is the most popular show on Broadway today."
Ham.byteslice(7)

When I run this it returns "n". 
When I run it with the (0) instead of (7) it returns "H". So the counting starts at zero instead of one.
When I run it with (6,7) it returns a string of 7 characters starting with the 6th one. 
When I run it with (6..9) it returns a string of characters starting with the 6th and ending with the 9th.
When I run it with (-1) it returns ".". When I change it to (-5) it returns "o". So with the minus sign, it counts backwards from the end of the string, with -1 identifying the last character in the string.
When I run it with (-0) it returns "H" so (0) and (-0) seem to point to the same position. 
When I run it with (92) it returns "nil".

I was able to modify my program to do 2 things:
1. The user inputs the number. (I had forgotten how to convert the input to an integer but found that again.) 
2. Make the counting start with one instead of zero. That was not a complete success. 
When I input "1" I do get the "H" in "Hamilton." 
But "0" is now the last character. 
Negative numbers now count from the end of the phrase, starting with the zeroth character. So that "-5" returns the "t" that is the 6th character from the end.
Inputs of number groups don't work. As written my program only pays attention to the first number in the group, so (6..8) returns just the 6th character, "t". 
There's probably a way to do it but I don't have it yet.

#PROGRAM TO INPUT A NUMBER AND HAVE IT GIVE YOU THE CORRESPONDING LETTER IN A STRING
puts "Here's a game. I have written a phrase and will give you one character from the phrase at a time, until you can guess the phrase. Low score wins."
Ham = "Hamilton is the most popular show on Broadway today."

puts "Please provide a number here. The number will correspond to the position of that character in the phrase. It may be a space."
number = gets.chomp
usenumber = number.to_i
finalnumber = usenumber-1

Ham.byteslice(finalnumber)

# The previous question asks about finding, for example, the 6th character in a String. Is it possible to find the **-6th** (Notice the negative symbol!) character in a String? What does that even mean?

YES. The minus sign seems to make the program count backwards from the end of the string. I think I covered this above.

# What is one way, using Ruby, to replace certain characters in a string with some other set of characters? For example, given `"Sumeet Jain"`, how would you replace all of the `e` characters in my name with exclamation marks? (So it would be `"Sum!!t Jain"`.)

I learned a little bit about using a method "gsub." There are probably other ways to do this.
#PROGRAM TO SUBSTITUTE EACH INSTANCE OF A CHARACTER IN A STRING WITH ANOTHER CHARACTER
TestString = "Sumeet Jain"
TestString.gsub!('e','!')
This works. It returned "Sum!!t Jain". It also worked when I used a longer substitution (I tried "77") instead of "!". 
I tried it with or without the exclamation point on "gsub!" and it seemed to work in repl.it either way. 
"Sub" only replaced the first "e" in my repl.it testing. "Gsub"replaced both. 

