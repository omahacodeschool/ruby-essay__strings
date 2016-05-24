---
title: Strings
instructor_notes: Feel free to re-organize the headings (or add/remove headings) below. We included the headings for your benefit, but it's 100% fine if you want to write your responses in some different structure.
---

# What is a String?

A sequence of characters strung together placed in between "" or ''. Used to store collection of characters.

# What are some examples of information that would be Strings as opposed to some other data type?

Paragraphs, sentences, greetings, addresses, or any other alphanumeric data.

# What is one way, using Ruby, to retrieve the 6th character in a String like `"Ada Lovelace"`? How about the 8th character? What happens if you try to retrieve the value of the _99th_ character (Or any character that doesn't exist)?

String = "Ada Lovelace"
String[5]
String[7]
String[98] would return nil

# The previous question asks about finding, for example, the 6th character in a String. Is it possible to find the **-6th** (Notice the negative symbol!) character in a String? What does that even mean?

Yes, it means it starts count backwards from the end with the last letter in the string being -1. String[-6] => v

# What is one way, using Ruby, to replace certain characters in a string with some other set of characters? For example, given `"Sumeet Jain"`, how would you replace all of the `e` characters in my name with exclamation marks? (So it would be `"Sum!!t Jain"`.)

This taks can be completed using .gsub

name = "Sumeet Jain"
name.gsub("e","!")
    => "Sum!!t Jain"
