---
title: Strings
instructor_notes: Feel free to re-organize the headings (or add/remove headings) below. We included the headings for your benefit, but it's 100% fine if you want to write your responses in some different structure.
---

# What is a String?

A string is data type that is a collection of letters, numbers, and/or symbols inside of quotations marks (single or double).


# What are some examples of information that would be Strings as opposed to some other data type?

Strings can represent any textual data. Names, phrases, book titles, song lyrics, etc. 
Booleans, Symbols, Numbers, Arrays, Hashes are the other types of data.
Each type has a different set of allowable operations.


# What is one way, using Ruby, to retrieve the 6th character in a String like `"Ada Lovelace"`? How about the 8th character? What happens if you try to retrieve the value of the _99th_ character (Or any character that doesn't exist)?

You could pull the sixth character (or substring) by using the positive position (remembering that the first position in the string is actually in the [0] position and that spaces are included in the position count).

    name = "Ada Lovelace"
    name[6] would return "v"
    
Same with the eighth:

    name[8] would return "l"
    
If you attempt to retrieve the 99th character, your code would return 'nil' which means 'nothingness'.


# The previous question asks about finding, for example, the 6th character in a String. Is it possible to find the **-6th** (Notice the negative symbol!) character in a String? What does that even mean?

Yeah, Every character has both a positive and negative position. You just count back from the end of the string. The last letter of the string is in the -1 position, the second to last is -2, etc.

    name[-6] is "v"
    
    
# What is one way, using Ruby, to replace certain characters in a string with some other set of characters? For example, given `"Sumeet Jain"`, how would you replace all of the `e` characters in my name with exclamation marks? (So it would be `"Sum!!t Jain"`.)

You could use the either the .sub or .gsub methods which stand for substitute and global substitute. The .gsub method acts as a 'find and replace all' command:

    name = "Sumeet Jain"
    name.gsub("e","!")
