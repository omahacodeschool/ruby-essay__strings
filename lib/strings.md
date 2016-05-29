---
title: Strings
instructor_notes: Feel free to re-organize the headings (or add/remove headings) below. We included the headings for your benefit, but it's 100% fine if you want to write your responses in some different structure.
---

# What is a String?

A string is a set (sorry, not trying to use that in an official sense) or sequence of characters.  Usually strings are a sequence of unicode characters that represent characters which themselves represent human language (http://www.tutorialspoint.com/ruby/ruby_strings.htm)
So, 'This is a string' is a string of a sequence of characters.

# What are some examples of information that would be Strings as opposed to some other data type?

Strings can be in single or double quotes.  So, collected elements in quotes are usually examples of strings.  Here is an instance of a string: example = "This is a string" , and another example is: statement = 'I am not a dog.'  Sequences of characters without quotation marks would not be strings, but could be name for the string for instance, or a key or value, for instance.

# What is one way, using Ruby, to retrieve the 6th character in a String like `"Ada Lovelace"`? How about the 8th character? What happens if you try to retrieve the value of the _99th_ character (Or any character that doesn't exist)?

To retrieve the 6th character of the string, you would just put that character in brackets next to the string, like this: example[6], which in my example, above, would get "s" as a result.  In the string like "Ada Lovelace", we would get "v".  The 8th character would give us 'l' as a result. if we tried to get the 99th character, or a character that was not part of the string (because it is not in the length of that string, in this case), we would get nil as a return.

# The previous question asks about finding, for example, the 6th character in a String. Is it possible to find the **-6th** (Notice the negative symbol!) character in a String? What does that even mean?

When there is a negative symbol in front of the number representing the charater of the string, that means that the count begins from the end of the string, and not the front. The -6th character for "Ada Lovelace" is "v".   

# What is one way, using Ruby, to replace certain characters in a string with some other set of characters? For example, given `"Sumeet Jain"`, how would you replace all of the `e` characters in my name with exclamation marks? (So it would be `"Sum!!t Jain"`.)

In ruby there are two different commands or code functions that can replace characters.  It just depends on what you are looking for: gsub replaces all instance, whereas sub replaces just the first instance of that certain character.  So if you just want to replace the first instance of that character or set of characters, you would just use sub, whereas in this case, replacing all of the 'e' characters inn "Sumeet Jain" would be gsub.  The code would look something like:
name = "Sumeet Jain"
name.gsub("e", "!")
puts name

I think that would result in "Sum!!t Jain"