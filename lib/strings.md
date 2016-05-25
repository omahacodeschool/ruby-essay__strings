---
title: Strings
instructor_notes: Feel free to re-organize the headings (or add/remove headings) below. We included the headings for your benefit, but it's 100% fine if you want to write your responses in some different structure.
---

# What is a String?

A string is a sequence of characters between either '' or "".

# What are some examples of information that would be Strings as opposed to some other data type?

When interacting with a user, a string is often the better data type to use. For example, it would make more sense to use a string when asking a question or printing out a response to the user's input.

# What is one way, using Ruby, to retrieve the 6th character in a String like `"Ada Lovelace"`? How about the 8th character? What happens if you try to retrieve the value of the _99th_ character (Or any character that doesn't exist)?

You can retrieve the sixth character in a string by addressing it by it's index within a string. "Ada Lovelace"[6] would select the sixth character in the string starting from the first character and count up to the sixth. You could find the eighth character the same way but when you try to select a character that does not exist nothing is returned.

# The previous question asks about finding, for example, the 6th character in a String. Is it possible to find the **-6th** (Notice the negative symbol!) character in a String? What does that even mean?

From what I read, strings (like arrays) have 0 based indexes. So when you are wanting to find the -6th character in a string Ruby starts counting backwards from the end of the string.

# What is one way, using Ruby, to replace certain characters in a string with some other set of characters? For example, given `"Sumeet Jain"`, how would you replace all of the `e` characters in my name with exclamation marks? (So it would be `"Sum!!t Jain"`.)

You can use the .gsub method replace all the e characters in "Smeet Jain". The first argument given to the .gsub method would be the character to replace. In this case we're replacing all of the e characters. The second argument is the new character you'd like to swap out for the existing characters.
