---
title: Strings
instructor_notes: Feel free to re-organize the headings (or add/remove headings) below. We included the headings for your benefit, but it's 100% fine if you want to write your responses in some different structure.
---

# What is a String?

A sequence of characters grouped together, enclosed by either single or double quotation marks.

# What are some examples of information that would be Strings as opposed to some other data type?

Text in any length - letters, words, sentences - would be treated as a string. 
Numerals used in a non-mathematical way (as a digit) would be part of a string, but if intended to be used in calculations, would be a number, rather than a string.

# What is one way, using Ruby, to retrieve the 6th character in a String like `"Ada Lovelace"`? How about the 8th character? What happens if you try to retrieve the value of the _99th_ character (Or any character that doesn't exist)?

The code to retrieve the sixth character, then the eighth character, is as follows:
a = "Ada Lovelace"
puts a[6]
puts a[8]

If you were to enter '99' or any number greater than 11, it returns a blank space. 

# The previous question asks about finding, for example, the 6th character in a String. Is it possible to find the **-6th** (Notice the negative symbol!) character in a String? What does that even mean?

puts a[-6] returns v, which is the 6th character when you begin counting at the end of the string (which is the functionality of using the negative number)

# What is one way, using Ruby, to replace certain characters in a string with some other set of characters? For example, given `"Sumeet Jain"`, how would you replace all of the `e` characters in my name with exclamation marks? (So it would be `"Sum!!t Jain"`.)

"Sumeet Jain".gsub('e','!')
