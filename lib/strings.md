---
title: Strings
instructor_notes: Feel free to re-organize the headings (or add/remove headings) below. We included the headings for your benefit, but it's 100% fine if you want to write your responses in some different structure.
---

# What is a String?

In computer programming, a string is traditionally a sequence of characters, either as a literal constant or as some kind of variable. 

# What are some examples of information that would be Strings as opposed to some other data type?

An example of string would be address = '123 Central Avenue' or puts = Hello world! as apposed to numeric data which would be something like and integer or a float.

# What is one way, using Ruby, to retrieve the 6th character in a String like `"Ada Lovelace"`? How about the 8th character? What happens if you try to retrieve the value of the _99th_ character (Or any character that doesn't exist)?

One way to retrieve the 6th character in Ada Lovelace would be to do something like this: 
character = 'Ada Lovelace'
character[6]
That would retrieve the letter 'v'. You would do the same for the 8th letter but simply change that [6] to a [8]. It's called the bracket operator. If you try to get one for the 99th it simply comes back as nil.

# The previous question asks about finding, for example, the 6th character in a String. Is it possible to find the **-6th** (Notice the negative symbol!) character in a String? What does that even mean?

It is possible to get the -6th character. The difference is that it counts from the end of the string, back. It's called a negative indice.

# What is one way, using Ruby, to replace certain characters in a string with some other set of characters? For example, given `"Sumeet Jain"`, how would you replace all of the `e` characters in my name with exclamation marks? (So it would be `"Sum!!t Jain"`.)

The gsub and gsub! methods provide another quick and easy way of replacing a substring with another string. These methods take two arguments, the search string and the replacement string. The gsub method returns a modified string, leaving the original string unchanged.
