---
title: Strings
instructor_notes: Feel free to re-organize the headings (or add/remove headings) below. We included the headings for your benefit, but it's 100% fine if you want to write your responses in some different structure.
---

# What is a String?

A string is an ordered sequence of some number of characters.  (Including zero.)  Normally one would think of letters, but depending on the character encoding, characters can also include a variety of numbers and symbols.

# What are some examples of information that would be Strings as opposed to some other data type?

If I were referring to, for example, the Beatles' compilation album, I would use a string:  "1".  While it's a numeric character, it's a title.  We don't perform arithmetic on titles.  We just store the characters.  It would be stored as a string, the same way we would store "Help!" as a string.  (I'd like to note here that there are a lot fewer albums with numeric titles than I expected when I checked Wikipedia.)

If I were counting the number of copies of the album that an online retailer had in their inventory, then I would store it as a number:  1.  I would want to be able to increment and decrement that number, or multiply it times a cost to obtain the current inventory value for the accounting system.  However, if I were displaying that number as a part of an inventory system, then the character I'm currently displaying would be a string.

# What is one way, using Ruby, to retrieve the 6th character in a String like `"Ada Lovelace"`? How about the 8th character? What happens if you try to retrieve the value of the _99th_ character (Or any character that doesn't exist)?

Because strings index (start) from 0, the 6th character is actually at index 5.  So, it would be:

"Ada Lovelace"[5]

And then:

"Ada Lovelace"[7]

An attempt to get the 99th character (at index 98) would get a nil result, because that character does not exist.

# The previous question asks about finding, for example, the 6th character in a String. Is it possible to find the **-6th** (Notice the negative symbol!) character in a String? What does that even mean?

Negative indexes will start from the end.  So -1 will retrieve the last character, and -6 will retrieve that many characters from the end.

# What is one way, using Ruby, to replace certain characters in a string with some other set of characters? For example, given `"Sumeet Jain"`, how would you replace all of the `e` characters in my name with exclamation marks? (So it would be `"Sum!!t Jain"`.)

You could just do:

"Sumeet Jain".gsub("e", "!")
