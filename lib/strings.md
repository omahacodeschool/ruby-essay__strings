---
title: Strings
instructor_notes: Feel free to re-organize the headings (or add/remove headings) below. We included the headings for your benefit, but it's 100% fine if you want to write your responses in some different structure.
---

# What is a String?

'A string of characters between quotations.'

# What are some examples of information that would be Strings as opposed to some other data type?

charaters, words, numbers, symbols

# What is one way, using Ruby, to retrieve the 6th character in a String like `"Ada Lovelace"`? How about the 8th character? What happens if you try to retrieve the value of the _99th_ character (Or any character that doesn't exist)?
You can retrieve specific charaters in a string using the [] method.

"Ada Lovelace"[6]
"Ada Lovelace"[8]

If you try to retrieve a variable that doesnt exist it returns nothing => nil


# The previous question asks about finding, for example, the 6th character in a String. Is it possible to find the **-6th** (Notice the negative symbol!) character in a String?
When using the negative symbol the program counts backwards from the end of the string. 

So "Ada Lovelace"[-6] returns the value v  

#What does that even mean?

The program is interpreting [-6] as the sixth variable of the string starting from the last.


# What is one way, using Ruby, to replace certain characters in a string with some other set of characters? For example, given `"Sumeet Jain"`, how would you replace all of the `e` characters in my name with exclamation marks? (So it would be `"Sum!!t Jain"`.)

You can replace certain charaters in a string using .gsub method. 

"Sumeet Jain".gsub(/e/, "!")

