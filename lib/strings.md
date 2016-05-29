---
title: Strings
instructor_notes: Feel free to re-organize the headings (or add/remove headings) below. We included the headings for your benefit, but it's 100% fine if you want to write your responses in some different structure.
---

# What is a String?

A string is anything contained between quotation marks (""). A string can be used to store any kind of 


# What are some examples of information that would be Strings as opposed to some other data type?

Most forms of text work well in strings. Whether they are long passages from a book or just a simple message like "Hello".
Numbers can be put in strings, but if they are to be used in any kind of mathematics, it would be best to leave them as an integer/float.
Numbers in a string only have value as a series of numerals, not as a whole number. In Ruby "100" is merely a one followed by two zeroes, trying to divide that probably won't get you what you want!


# What is one way, using Ruby, to retrieve the 6th character in a String like `"Ada Lovelace"`? How about the 8th character? What happens if you try to retrieve the value of the _99th_ character (Or any character that doesn't exist)?

I'd start by defining that string as a variable to use it more efficiently like hero = "Ada Lovelace" because she was a bad-ass in general.
Then I can take the variable 'hero' and using brackets I can identify the 6th character like this:

    hero[5]
    
The '5' represents the sixth letter because the first character (A) is actually in the 'zero' position. 
So hero[0] will be 'A' and hero[5] will be the 'o'. Similarly hero[7] will pull out the 8th letter, 'e'. These characters that get pulled out are 'substrings' within the bigger one.
Trying to find the 99th character will result in a 'nil' because no character exists in that position.


# The previous question asks about finding, for example, the 6th character in a String. Is it possible to find the **-6th** (Notice the negative symbol!) character in a String? What does that even mean?

It is possible to find a negative position in a string, the '-' tells Ruby to count from the end of the string instead of the start. In this case -6 gets you a 'v' because it starts from the last 'e' at the -1 position.


# What is one way, using Ruby, to replace certain characters in a string with some other set of characters? For example, given `"Sumeet Jain"`, how would you replace all of the `e` characters in my name with exclamation marks? (So it would be `"Sum!!t Jain"`.)

To replace characters in a string, I'll start with labelling my string with something like instructor = "Sumeet Jain".
Using the .sub and .gsub I can essentially perform a find-&-replace but on the specified string. Using .sub replaces one instance of the substring you want to replace and .gsub will replace all instances of that substring.
To use .sub and .gsub I have to create an argument that will tell the virtual machine to find the offending substring and replace it with something else. In this case 'e' for '!' 
In this case I'll be using .gsub to replace both e's. The argument for .gsub follows it inside parentheses.

    instructor = "Sumeet Jain"
    instructor.gsub("e","!")
    
This method tells the VM to find all the e's in the string and replace them with exclamation points.