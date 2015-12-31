---
title: Strings
instructor_notes: Feel free to re-organize the headings (or add/remove headings) below. We included the headings for your benefit, but it's 100% fine if you want to write your responses in some different structure.
---

# What is a String?

Data used to represent text.

# What are some examples of information that would be Strings as opposed to some other data type?

'Inconceivable' 'Hello, my name is Inigo Montoya. You killed my father prepare to die' 'I just sucked 1 year of your life away'

# What is one way, using Ruby, to retrieve the 6th character in a String like `"Ada Lovelace"`? How about the 8th character? What happens if you try to retrieve the value of the _99th_ character (Or any character that doesn't exist)?

Using [ ] with a number specified inside will retrieve a corresponding letter for you. However, it doesnt retreive the 6th letter if you put in 6. Instead, it will give you the 7th. I'm thinking this is because it is counting from zero rather than 1.  If you were to put in [0] it would return A. 
To retreive the 8th character you would type 'Ada lovelace' [7].  If you attempt to retreive the 99th character nil is displayed. 

# The previous question asks about finding, for example, the 6th character in a String. Is it possible to find the **-6th** (Notice the negative symbol!) character in a String? What does that even mean?

Using symbols as above for finding a negative character will run the program from the end of the string rather than the beginning.  'Ada Lovelace' [-6] will return v.  V is actually the 6th letter when counting backwards in the string. This is because A is still 0, so -1 is e, -2 is c, etc. etc.

# What is one way, using Ruby, to replace certain characters in a string with some other set of characters? For example, given `"Sumeet Jain"`, how would you replace all of the `e` characters in my name with exclamation marks? (So it would be `"Sum!!t Jain"`.)

Gsub replaces all instances of your chosen characters.  So if we were to sub characters in your name it would look something like Value = value.gsub('e', '!')
