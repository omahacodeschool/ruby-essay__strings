---
title: Strings
instructor_notes: Feel free to re-organize the headings (or add/remove headings) below. We included the headings for your benefit, but it's 100% fine if you want to write your responses in some different structure.
---

# What is a String?

A string is any collection of numbers and or letters ketp together.

# What are some examples of information that would be Strings as opposed to some other data type?

anything placed in () to remain as a set, to be used as whole, or in parts depending on the user

# What is one way, using Ruby, to retrieve the 6th character in a String like `"Ada Lovelace"`? How about the 8th character? What happens if you try to retrieve the value of the _99th_ character (Or any character that doesn't exist)?

after defining the string, set out [] to define what character you want to select or retrieve

# The previous question asks about finding, for example, the 6th character in a String. Is it possible to find the **-6th** (Notice the negative symbol!) character in a String? What does that even mean?

Of course, finding the negative 6 would be no different to ruby, it would still count, starting at 0, backwards around the string to six places back.

# What is one way, using Ruby, to replace certain characters in a string with some other set of characters? For example, given `"Sumeet Jain"`, how would you replace all of the `e` characters in my name with exclamation marks? (So it would be `"Sum!!t Jain"`.)

myString = "Sumeet Jain"

myString[3..4]= "!!"

puts myString
