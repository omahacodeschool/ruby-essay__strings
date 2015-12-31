---
title: Strings
instructor_notes: Feel free to re-organize the headings (or add/remove headings) below. 
We included the headings for your benefit, but it's 100% fine if you want to write your responses in some different structure.
---

# What is a String?

A string is a collection of numbers or letters that are distinct from data objects in the sense that the string: '42 geese.reverse' not only 
doesn't contain the number 42 (the number that is 15 less than 57), but also will not use the reverse action to flip the order of the 
preceeding word "geese." 

# What are some examples of information that would be Strings as opposed to some other data type?

A series of numbers like '435' is not an integer. 
'435'to_i 
would convert the string to a number that could be used with math operations. 
Any words that could be misinterpreted as Ruby commands are safe within the quotes that contain a string.  
The words to a novel, or a list of names, would be suited to strings rather than, say, financial calculations or stock tickers 
which would benefit from the use of math operations.

# What is one way, using Ruby, to retrieve the 6th character in a String like `"Ada Lovelace"`? How about the 8th character? 
What happens if you try to retrieve the value of the _99th_ character (Or any character that doesn't exist)?

Because Ruby is zero-based indexed, the 6th character in "Ada Lovelace" is in the 5th position (starting with "0th"). 
So, use:

string = "Ada Lovelace"
string[5]

If trying to retrieve a non-existent character, the program returns =>nil 

# The previous question asks about finding, for example, the 6th character in a String. 
Is it possible to find the **-6th** (Notice the negative symbol!) character in a String? What does that even mean?

Yes, that would mean the 6th character from the end. In the example above, string[-6] returns v.

# What is one way, using Ruby, to replace certain characters in a string with some other set of characters? 
For example, given `"Sumeet Jain"`, how would you replace all of the `e` characters in my name with exclamation marks? 
(So it would be `"Sum!!t Jain"`.)

My code would look like this:

my_string = "Sumeet Jain".gsub("e","!") 
puts my_string


(note that using sub would only replace the first instance of 'e'. Gsub will replace all instances of 'e' in the string) 

