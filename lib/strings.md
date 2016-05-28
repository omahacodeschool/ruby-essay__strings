---
title: Strings
instructor_notes: Feel free to re-organize the headings (or add/remove headings) below. We included the headings for your benefit, but it's 100% fine if you want to write your responses in some different structure.
---

# What is a String?

A String is a variable that stores a sequences of characters.

# What are some examples of information that would be Strings as opposed to some other data type?

Words, sentences or any kind of text would be a String.  Also, input from a user is often saved as a String, even if it will be converted to another variable type later.

# What is one way, using Ruby, to retrieve the 6th character in a String like `"Ada Lovelace"`? How about the 8th character? What happens if you try to retrieve the value of the _99th_ character (Or any character that doesn't exist)?

"Ada Lovelace"[6] and "Ada Lovelace"[8].  string_name[n] will return the nth character of any String.  Attempting to retrieve a nonexistant character returns the value 'nil'.

# The previous question asks about finding, for example, the 6th character in a String. Is it possible to find the **-6th** (Notice the negative symbol!) character in a String? What does that even mean?

string_name[-6] will return the character 6 places from the end of the String, so "Ada Lovelace"[-6] still returns "v" while "Ada Lovelace"[-8] returns "L"

# What is one way, using Ruby, to replace certain characters in a string with some other set of characters? For example, given `"Sumeet Jain"`, how would you replace all of the `e` characters in my name with exclamation marks? (So it would be `"Sum!!t Jain"`.)

gsub will replace all instances of a character in a string, so "Sumeet Jain".gsub('e','!') returns "Sum!!t Jain".
