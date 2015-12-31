---
title: Strings
instructor_notes: Feel free to re-organize the headings (or add/remove headings) below. We included the headings for your benefit, but it's 100% fine if you want to write your responses in some different structure.
---

# What is a String?

A string is a group of characters placed between single or double quotes.

# What are some examples of information that would be Strings as opposed to some other data type?

Here are some examples of strings: "4" or '4', as opposed to the integer 4. "With the quotation marks, this sentence is considered a string as well."

# What is one way, using Ruby, to retrieve the 6th character in a String like `"Ada Lovelace"`? How about the 8th character? What happens if you try to retrieve the value of the _99th_ character (Or any character that doesn't exist)?

One way, using Ruby, to retrieve the 6th character would be: puts "Ada Lovelace"[6]. This prints 'v'. To retrieve the 8th character, do the same but replace the 6 with an 8 (puts "Ada Lovelace"[8]). If this process is attempted to retrieve the 99th character, the computer will print nothing.

# The previous question asks about finding, for example, the 6th character in a String. Is it possible to find the **-6th** (Notice the negative symbol!) character in a String? What does that even mean?

It is possible, and using the setup (puts "Ada Lovelace"[ ]) with a -6 will retrieve 'v'. Retrieving characters with a negaative value starts the count at the end of the string instead of the beginning. Replacing the value with -1 would retrieve 'e', -2: 'c', and so forth.

# What is one way, using Ruby, to replace certain characters in a string with some other set of characters? For example, given `"Sumeet Jain"`, how would you replace all of the `e` characters in my name with exclamation marks? (So it would be `"Sum!!t Jain"`.)

One way that I found to replace each istance of the letter 'e' in "Sumeet Jain" would be: puts "Sumeet Jain".tr("e", "!").
