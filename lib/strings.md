---
title: Strings
instructor_notes: Feel free to re-organize the headings (or add/remove headings) below. We included the headings for your benefit, but it's 100% fine if you want to write your responses in some different structure.
---

# What is a String?

Strings are sequences of characters that are "strung" together.  Either double or single quotes signify to Ruby when the string starts and ends.
I think of Strings as groups of alphanumeric characters I want Ruby to display literally. 
For example "12 + 12" would be literally displayed as "12 + 12" and not 24.


# What are some examples of information that would be Strings as opposed to some other data type?

Data can come in different types.  A String data type can be words or phrases like "Crazy McJibberish" or "12 + 12", or simply blank " ".  
Other data types such as Numbers (either integers or floats) or Booleans (true or false) analyze and manipulate data differently and use different syntax.
For example "12" is a String of the two digits, 12 is a Number, and 1>2 is a false Boolean argument.

# What is one way, using Ruby, to retrieve the 6th character in a String like `"Ada Lovelace"`? How about the 8th character? What happens if you try to retrieve the value of the _99th_ character (Or any character that doesn't exist)?

One way to to use Ruby to retrieve the 6th and/or 8th character in the above String is to use an Array, retrieving characters using the #[] method using a single integer argument.  
Since Array indexing starts at 0, and index of 5 would retrieve the 6th character "o" and an index of 7 would retrieve the 8th character "e".
In this example, since there are only 12 characters (including the spacing), any attempt to retrieve a character the value of 13 or higher results in a nil return.


# The previous question asks about finding, for example, the 6th character in a String. Is it possible to find the **-6th** (Notice the negative symbol!) character in a String? What does that even mean?

Yes, it is possible o find the -6th character in a String.  
Since Array indexing starts a 0, an index of -6 retrieves the sixth-to-last character in a String, provided the String is at least 6 characters long.
And just like the previous question, any attempt to find the -13th character results in a nil return.

# What is one way, using Ruby, to replace certain characters in a string with some other set of characters? For example, given `"Sumeet Jain"`, how would you replace all of the `e` characters in my name with exclamation marks? (So it would be `"Sum!!t Jain"`.)

One way to replace certain characters in a string with some other set of characters is to use the global substitution string operator --> "Sumeet Jain".gsub('e','!')
