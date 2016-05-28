---
title: Strings
instructor_notes: Feel free to re-organize the headings (or add/remove headings) below. We included the headings for your benefit, but it's 100% fine if you want to write your responses in some different structure.
---

# What is a String?

A String is a sequence of characters either as literal constant or some kind of variable. 
Strings are one of the most used data types in programming and are surrounded with single or double quotes. 

# What are some examples of information that would be Strings as opposed to some other data type?

An example of strings is sentences or paragraphs on a website. Strings normally contain information to be read by a user. 
Numbers for math related problems such as multiplication or adding would be used as integer/fixnum data type instead of strings. 

# What is one way, using Ruby, to retrieve the 6th character in a String like `"Ada Lovelace"`? How about the 8th character? What happens if you try to retrieve the value of the _99th_ character (Or any character that doesn't exist)?

To find the 6th character it would be “Ada Lovelace” [6] and would be “v”.
To find the 8th character it would be “Ada Lovelace”[8] and would be “l”.
When retrieving value higher than the amount of characters in the string you would receive nil. 


# The previous question asks about finding, for example, the 6th character in a String. Is it possible to find the **-6th** (Notice the negative symbol!) character in a String? What does that even mean?

The negative sign would tell the search start from the end of the string and go backwards six characters. 

# What is one way, using Ruby, to replace certain characters in a string with some other set of characters? For example, given `"Sumeet Jain"`, how would you replace all of the `e` characters in my name with exclamation marks? (So it would be `"Sum!!t Jain"`.)

You would use the gsub method. The code would be “Sumeet Jain”.gsub(‘e’, ‘!’). 