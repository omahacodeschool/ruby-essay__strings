---
title: Strings
instructor_notes: Feel free to re-organize the headings (or add/remove headings) below. We included the headings for your benefit, but it's 100% fine if you want to write your responses in some different structure.
---

# What is a String?

A string is a data type that consists of a combination of characters or values. Strings are surrounded by "" or '' marks. 

# What are some examples of information that would be Strings as opposed to some other data type?

Letters, words, sentences, or numbers that are read or printed to the screen and are not telling the computer to do something would be examples of strings. Numbers which are used mathematically and boolean operators like true or false would not be strings.

# What is one way, using Ruby, to retrieve the 6th character in a String like `"Ada Lovelace"`? How about the 8th character? What happens if you try to retrieve the value of the _99th_ character (Or any character that doesn't exist)?

A string is an array, so each value in a string has an index number, starting at 0. For example, since it is the 5th value, the index for "L" in "Ada Lovelace" is 4. So to retrieve the 6th character, I would look for the value with an index of 5. The code "Ada Lovelace" [5] would return "o". For the 8th character, I would look for the value with an index of 7. If I search for an index that is greater than the number of characters in a string, it returns nil.

# The previous question asks about finding, for example, the 6th character in a String. Is it possible to find the **-6th** (Notice the negative symbol!) character in a String? What does that even mean?

It is possible. Using the negative sign tells Ruby to index the characters in reverse. Therefore, "Ada Lovelace" [-5] would return "e".

# What is one way, using Ruby, to replace certain characters in a string with some other set of characters? For example, given `"Sumeet Jain"`, how would you replace all of the `e` characters in my name with exclamation marks? (So it would be `"Sum!!t Jain"`.)

One method would be to use a regular expression and the gsub method to globally substitue all instances of the letter "e" with a "!". For example, "Sumeet Jain".gsub(/e/, "!") would output "Sum!!t Jain".