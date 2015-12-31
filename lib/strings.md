---
title: Strings
instructor_notes: Feel free to re-organize the headings (or add/remove headings) below. We included the headings for your benefit, but it's 100% fine if you want to write your responses in some different structure.
---

# What is a String?

Strings are sequences of characters used to communicate with a user. The characters in a String can be letters, words, sentences, paragraphs, greetings, commands, etc.

# What are some examples of information that would be Strings as opposed to some other data type?

An example of a String would be a name input from a user, or literally the letters of a person's name strung together as a word.
Another example of a String is a message I want to communicate to a user. If I wanted to tell a user that Fred likes pizza, I could use the String "Fred likes pizza". 
Similarly, if I want to tell a user that there is only one hour of battery power left on their computer, I could communicate that using the String "You have one hour of battery power left". 
However, if I want to actually calculate the amount of battery power left on their computer, I would want to use integers, a different data type, to subtract the amount of depleted battery power from the full amount of battery power.

# What is one way, using Ruby, to retrieve the 6th character in a String like `"Ada Lovelace"`? How about the 8th character? What happens if you try to retrieve the value of the _99th_ character (Or any character that doesn't exist)?

You could pull out a Substring from the String using the character position number. Do this by placing [6], or the number 6 in brackets at the end of your String. You could do the same to pull out the 8th character using the number 8 instead of 6.
If asked to retrieve the 99th character, the program would return ‘nil’ since that character does not exist. You could find out if a String has a 99th character prior to trying to pull it out as a substring by running a command to count the total number of characters in a string first.

# The previous question asks about finding, for example, the 6th character in a String. Is it possible to find the **-6th** (Notice the negative symbol!) character in a String? What does that even mean?

A negative number used when referring to character positon simply indicates the position of the character counting backward from the end of the String. So the -6th character in the String "Ada Lovelace" would be 'v'.

# What is one way, using Ruby, to replace certain characters in a string with some other set of characters? For example, given `"Sumeet Jain"`, how would you replace all of the `e` characters in my name with exclamation marks? (So it would be `"Sum!!t Jain"`.)

You could use the .gsub method to replace all occurrences of a certain character in a String with a different character. The .gsub method subsitutes one character for another globally, or every time it occurs within the given String.
Using this method, you could replace all of the 'e's in Sumeet with exclamation marks using the following code: "Sumeet Jain".gsub!("e","!")


