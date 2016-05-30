---
title: Strings
instructor_notes: Feel free to re-organize the headings (or add/remove headings) below. We included the headings for your benefit, but it's 100% fine if you want to write your responses in some different structure.
---

# What is a String?

A string, simply put, is a collection of special characters, letters, and/or numbers. Strings can be as a simple as a name to something longer like an entire sentence or paragraph.


# What are some examples of information that would be Strings as opposed to some other data type?

Since strings are unique in that they can contain a variety of data types like numbers, spaces, letters, and/or special characters, something like a street address (ex: "1132 E. 22nd St.") would be considered a string since it contains, letters, numbers, and special characters. 


# What is one way, using Ruby, to retrieve the 6th character in a String like `"Ada Lovelace"`? How about the 8th character? What happens if you try to retrieve the value of the _99th_ character (Or any character that doesn't exist)?

Steps to retrieve the 6th character  in "Ada Lovelace":
1) string1 = "Ada Lovelace"
2) string1[5..5]
3) Returns "o"

Code to retrieve the 8th character  in "Ada Lovelace":
1) string1 = "Ada Lovelace"
2) string1[7..7]
3) Returns "e"

Steps to retrieve the 99th character in "Ada Lovelace":
1) string1 = "Ada Lovelace"
2) string1[99..99]
3) Returns nil



# The previous question asks about finding, for example, the 6th character in a String. Is it possible to find the **-6th** (Notice the negative symbol!) character in a String? What does that even mean?

It means when searching for the specified substring, the program will count from the end of the string backwards, with the last position of the string being -1 (since there's no such thing as a -0).


# What is one way, using Ruby, to replace certain characters in a string with some other set of characters? For example, given `"Sumeet Jain"`, how would you replace all of the `e` characters in my name with exclamation marks? (So it would be `"Sum!!t Jain"`.)

Code to replace the "e" in Sumeet's name with an exclamation point ("!"):
1) name1 = "Sumeet Jain"
2) name1.gsub("e","!")