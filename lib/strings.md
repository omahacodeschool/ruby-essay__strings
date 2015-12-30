---
title: Strings
instructor_notes: Feel free to re-organize the headings (or add/remove headings) below. We included the headings for your benefit, but it's 100% fine if you want to write your responses in some different structure.
---

# What is a String?

A string is a character or series of characters (letters, words, symbols, paragraphs, digits, spaces etc., or they can just be empty). Strings are written inside of single or double quotes. Putting something inside double quotes will make Ruby evaluate information in the string differently. For example, using double quotes for strings makes it so that escape characters will be evaluated correctly, whereas using single quotes will make Ruby take these escape characters literally and your output will have unnecessary characters in it and none of the actual commands will be performed.  


# What are some examples of information that would be Strings as opposed to some other data type?

Strings are different than integers and floats. Numbers can be strings, but once they’re in quotes they’re called digits and they behave differently. For example, integers are used for arithmetic, so 2 + 2 = 4. However, as strings, ‘2’ + ‘2’ = 22, just the same as ‘Sun’ + ‘day’ = Sunday.


# What is one way, using Ruby, to retrieve the 6th character in a String like `"Ada Lovelace"`? How about the 8th character? What happens if you try to retrieve the value of the _99th_ character (Or any character that doesn't exist)?

I know you said you didn’t need code for these prompts but I think I can’t put this into words without showing the code. To pull out a substring (in this case the 6th character), you would use code like this:

string = "Ada Lovelace"
string[6]

Or if you want the 8th character, replace the 6 with an 8 and you’ll get a “l” back instead of a “v.” Ruby counts each character (including spaces) starting with zero, not one. That is, unless you’re counting backwards. For reasons I’m not certain of yet, backwards counting starts right at -1 on the last character instead of zero. 

If you try to retrieve the 99th character or another that doesn’t exist in the string, it returns nil.


# The previous question asks about finding, for example, the 6th character in a String. Is it possible to find the **-6th** (Notice the negative symbol!) character in a String? What does that even mean?

Yes, you can use the negative positions of a string if you’re looking for a character based on it’s distance from the end of a string. It’s just a matter counting backward instead of forward and it might make more sense to do it this way in some instances. 


# What is one way, using Ruby, to replace certain characters in a string with some other set of characters? For example, given `"Sumeet Jain"`, how would you replace all of the `e` characters in my name with exclamation marks? (So it would be `"Sum!!t Jain"`.)

For that you would “replace a substring” as it’s called. Since we need more than one thing changed, we’d use the gsub (global) method which would change all of the e’s to exclamation points instead of just the first occurrence like the plain old sub method would do. Here’s the code:  "Sumeet Jain" .gsub('e','!')

