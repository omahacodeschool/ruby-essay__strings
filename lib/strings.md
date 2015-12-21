---
title: Strings
instructor_notes: Feel free to re-organize the headings (or add/remove headings) below. We included the headings for your benefit, but it's 100% fine if you want to write your responses in some different structure.
---

# What is a String?

In ruby, a string is simply a character or combination/sequence of characters placed in between quotes (single or double).

# What are some examples of information that would be Strings as opposed to some other data type?

Almost any information one would find in a phonebook/contacts list would be a great example of where strings are used. Everything from the names to email 
addresses would all be strings. Even the phone nunbers in a contact list are strings, in that they are not treated as
mere mathematical numbers used for calculating and so forth, and would be seen rather as a combination of numbers with no actual numerical value.

# What is one way, using Ruby, to retrieve the 6th character in a String like `"Ada Lovelace"`? How about the 8th character? What happens if you try to retrieve the value of the _99th_ character (Or any character that doesn't exist)?

One simple way to retrieve the 6th character of the string "Ada Lovelace" would be to place the index of the character you are trying to retrieve in
brackets as follows:
"Ada Lovelace"[5]. 

In this case, the index of 5 is used, even though we are looking for the 6th letter. This can be confusing at first,
but is due to the fact that in most (or all?) programming langauages, the first character or item in an index begins at 0.

If you try to retrieve a character index that does not exist (one that is larger than the number of characters in the string), you will get an output of "Nil" because 
there is nothing that matches the criteria.

# The previous question asks about finding, for example, the 6th character in a String. Is it possible to find the **-6th** (Notice the negative symbol!) character in a String? What does that even mean?

It is possible to find the -6th character in a string in Ruby. In this case, if one used the same string as the above example, using "Ada Lovelace"[-6]
we would retrieve the character "v". What's happening here is that if an index is negative, it is counted from the end of the string, as opposed to starting at the beginning.

# What is one way, using Ruby, to replace certain characters in a string with some other set of characters? For example, given `"Sumeet Jain"`, how would you replace all of the `e` characters in my name with exclamation marks? (So it would be `"Sum!!t Jain"`.)

One way to replace certain characters in a string with other characters would be as follows:

Example:
"Sumeet Jain".gsub('e', '!')

This would give us "Sum!!t Jain" 

What's happening above is that the ".gsub" method in Ruby allows us to replace a character with another. We do this in the area in the parantheses, known as parameters, after .gsub.
In the parenthesis, the character to be replaced goes in first, before the comma, and the character to replace it with goes in second (after the comma).
If we left off the "g" and used the ".sub" method instead, it would only replace the
first occurance of the letter "e"; using the "g" makes the method "global" which replaces all occurances of the letter. 
