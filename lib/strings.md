---
title: Strings
instructor_notes: Feel free to re-organize the headings (or add/remove headings) below. We included the headings for your benefit, but it's 100% fine if you want to write your responses in some different structure.
---

# What is a String?

A string is a sequence of characters.

# What are some examples of information that would be Strings as opposed to some other data type?

Most text that isn't part of a command will be a string, as it appears on the web as a string. Additionally, when numbers are supposed to be put together (but not added arithmetically), they are stored as strings.

# What is one way, using Ruby, to retrieve the 6th character in a String like `"Ada Lovelace"`? How about the 8th character? What happens if you try to retrieve the value of the _99th_ character (Or any character that doesn't exist)?

The best way I've come up with is to store the string as a variable and then use brackets with the number of the position you're looking for, like this:
string = "abcdefghijklmnop";
string [6] + ', ' + string [8];
When I enter a position number that doesn't exist, the program returns 'nil'.

# The previous question asks about finding, for example, the 6th character in a String. Is it possible to find the **-6th** (Notice the negative symbol!) character in a String? What does that even mean?

The program returns the character that is however many positions from the end of the string, ex. entering [-6] returns the sixth to last character in the string.

# What is one way, using Ruby, to replace certain characters in a string with some other set of characters? For example, given `"Sumeet Jain"`, how would you replace all of the `e` characters in my name with exclamation marks? (So it would be `"Sum!!t Jain"`.)

After again storing the string as a variable, you can use the .gsub command to replace characters. To do what you asked above, I wrote this:
string = "Sumeet Jain";
string.gsub('e', '!')
