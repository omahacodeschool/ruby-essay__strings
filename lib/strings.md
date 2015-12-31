---
title: Strings
instructor_notes: Feel free to re-organize the headings (or add/remove headings) below. We included the headings for your benefit, but it's 100% fine if you want to write your responses in some different structure.
---

# What is a String?

A string is a sequence of characters. 

# What are some examples of information that would be Strings as opposed to some other data type?

Some examples of information that would be strings as opposed to other data types are names, program instructions, or any messages to the user. 

# What is one way, using Ruby, to retrieve the 6th character in a String like `"Ada Lovelace"`? How about the 8th character? What happens if you try to retrieve the value of the _99th_ character (Or any character that doesn't exist)?

One way to retrieve the 6th character of a string is to use the "[]" method. By placing a 6 inside of the brackets and immediately following a string, for example "Ava Lovelace"[6], Ruby will return the 6th character, "v". The same thing applies for the 8th character. Just place an 8 in the brackets and ruby will return the 8th character in the string "l". Any time you try to retrieve a character that does not exist, ruby will return a "nil" informing the user that there was nothing for ruby to return. 

# The previous question asks about finding, for example, the 6th character in a String. Is it possible to find the **-6th** (Notice the negative symbol!) character in a String? What does that even mean?

It is possible to retrieve the -6th character in a string. What that means is the ruby will start at the end of the string and count backwards. In the previous example, [-6] would return "v" again.

# What is one way, using Ruby, to replace certain characters in a string with some other set of characters? For example, given `"Sumeet Jain"`, how would you replace all of the `e` characters in my name with exclamation marks? (So it would be `"Sum!!t Jain"`.)

Strings can be altered with the "[]=" method. There are multiple ways to use this command to replace certain characters in a string, however, in order to execute the given example, assuming your name, "Sumeet Jain", was stored in a string variable named "string", string[3,2]= "!!" would provide the correct outcome. Another, perhaps more straightforward way to achieve this outcome would be to simple replace the "e"s in your name with "!"s using the gsub! method. Using the same variable, string.gsub!("e", "1") would produce the same output. 
