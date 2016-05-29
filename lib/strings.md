---
title: Strings
instructor_notes: Feel free to re-organize the headings (or add/remove headings) below. We included the headings for your benefit, but it's 100% fine if you want to write your responses in some different structure.
---

# What is a String?

A sequence of characters denoted by double or single quotaion marks.  
Strings can be as short as one letter or as long as a book.

# What are some examples of information that would be Strings as opposed to some other data type?

Anytime there is text a string is good to use.
Strings are easy to manipulate.  
You would not want to use a string if you have a list or paired data - hashes and arrays would be better choices.
You would not want to use a string if you want to perform operations on numbers.


# What is one way, using Ruby, to retrieve the 6th character in a String like `"Ada Lovelace"`? How about the 8th character? What happens if you try to retrieve the value of the _99th_ character (Or any character that doesn't exist)?

The characters in a string are indexed based starting with 0 so the sixth character would be index 5.
The 8th character is index 7.
Trying to retrieve a value that does not exist will return nil.

string = "Ada Lovelace"

puts string[5] => o
puts string[7] => e
puts string[99] =>


# The previous question asks about finding, for example, the 6th character in a String. Is it possible to find the **-6th** (Notice the negative symbol!) character in a String? What does that even mean?

It is possible to find the -6th character.  
This would be the sixth character from the end

string = "Ada Lovelace"
puts string[-6] => v

# What is one way, using Ruby, to replace certain characters in a string with some other set of characters? For example, given `"Sumeet Jain"`, how would you replace all of the `e` characters in my name with exclamation marks? (So it would be `"Sum!!t Jain"`.)

You would have to use global substitution if you want to replace all the 'e's with '!'s

puts "Summet Jain".gsub("e", "!")
