---
title: Strings
instructor_notes: Feel free to re-organize the headings (or add/remove headings) below. We included the headings for your benefit, but it's 100% fine if you want to write your responses in some different structure.
---

# What is a String?

A string is a serries of charecters in Ruby.  They are placed between quotation marks, and are used to communicate with users.

# What are some examples of information that would be Strings as opposed to some other data type?

A string could be used to ask a user to input a value for something.  However, the user's input may need to be interpreted as an integer in order for it to interact
with other data within the code.  A program used for cost estimating may need to use strings as well as other data types. 

# What is one way, using Ruby, to retrieve the 6th character in a String like `"Ada Lovelace"`? How about the 8th character? What happens if you try to retrieve the value of the _99th_ character (Or any character that doesn't exist)?

One way to search for characters in the string "Ada Lovelace" is to set the string to a variable (lets say x = "Ada Lovelace") and then search that variable using x[6]. 
You can replace a the numbe, beginning with 0, inside the [] to find different characters. Ruby will return nil if the absolute value of the number
inside the [] is larger than the number of characters in the string.

# The previous question asks about finding, for example, the 6th character in a String. Is it possible to find the **-6th** (Notice the negative symbol!) character in a String? What does that even mean?

In the previous, retrieving the 6th character would mean retrieving the 6th character from the beginning of the string.  If you added a negative symbol to the character you wanted
to retrieve, in our case -6.  You would then retrieve the 6th character from the end of the string.  Which in the case of "Ada Lovelace" would both be the letter "v".

# What is one way, using Ruby, to replace certain characters in a string with some other set of characters? For example, given `"Sumeet Jain"`, how would you replace all of the `e` characters in my name with exclamation marks? (So it would be `"Sum!!t Jain"`.)

One way to replace characters in Ruby is with '.gsub'.  With .gsub you can tell Ruby to replace all of a one character in a string with another character.  
