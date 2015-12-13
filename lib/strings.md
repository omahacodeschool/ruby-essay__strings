---
title: Strings
instructor_notes: Feel free to re-organize the headings (or add/remove headings) below. We included the headings for your benefit, but it's 100% fine if you want to write your responses in some different structure.
---

# What is a String?

A string is a sequence of characters.  The beginning and end of a string are indicated by the use of single or double quotation marks.  It doesn't generally matter which you use, but you need to be consistent.  So, if you start with a single quotation mark, you need to end with a single quotation mark.  In Ruby, the single quotation marks cause the computer to intepret whatever's inside them literally though, so if you want to use something like an escape character, use the double ones.

# What are some examples of information that would be Strings as opposed to some other data type?

Generally, you'll have three main data types, i.e., string, integer, and float.  Integer and float are numbers.  Integers are what they are in any math class you've likely taken and float refers to numbers with decimals or a "flaoting point".  String is merely a sequence of characters that are "strung" together.  What sort of characters they are don't matter.  There can be numbers, symbols, or letters.  Of note, if you use a number in a string it's treated solely as a character and doing math with it will require some fiddling.  By and large though, strings contain non-numeric information, names, sentences, paragraphs, whole novels, etc.

# What is one way, using Ruby, to retrieve the 6th character in a String like `"Ada Lovelace"`? How about the 8th character? What happens if you try to retrieve the value of the _99th_ character (Or any character that doesn't exist)?

Well, if you've established assigned "Ada Lovelace" to a variable, value = "Ada Lovelace", then you can get the 6th character by telling the computer to "print" or "puts" value[5].  This should return the sixth character or "o".  To get the 8th character, you'd do the same thing but instead of 5 you'd put 7 in brackets.  The reason you use 5 and 7 to get the 6th and 8th characters respectively, is that elements in a string are counted a bit strangely.  The first character is 0, the second 1, and so on.  When I tried getting it to return a value that wasn't in the string, the 99th character, it just returned a blank followed by "=>nil".  I got this same result for other values that weren't in the string, e.g., 70, 34, etc.  If I had to hazard a guess, I think ruby treats the space in a string after the last character as a void, i.e, there could be something there, but there isn't so it returns a blank.  It doesn't return an error, so it doesn't have a problem with asking that question.

# The previous question asks about finding, for example, the 6th character in a String. Is it possible to find the **-6th** (Notice the negative symbol!) character in a String? What does that even mean?

Yes, it is possible to find the -6th character in a string.  It's just that ruby interprets this request as the user wanting to know what the sixth character as counted from the end of the string is.  In the case of "Ada Lovelace", when you plug in -6, you get "v".  It's worth noting that unlike when counting from the front of the string, counting from the end begins with a 1 and not a 0.

# What is one way, using Ruby, to replace certain characters in a string with some other set of characters? For example, given `"Sumeet Jain"`, how would you replace all of the `e` characters in my name with exclamation marks? (So it would be `"Sum!!t Jain"`.)

First, you'd create a string of your name and assign it to a variable, something like name = "Sumeet Jain".  Then, you can tell the computer to swap out characters in the name string within a certain range.  So, name[3..4] = "!!".  Now, when you tell it to print out name it should return "Sum!!t Jain".  There are other methods you can apply, but this one's fairly straight forward.
