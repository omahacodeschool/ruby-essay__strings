---
title: Strings
instructor_notes: Feel free to re-organize the headings (or add/remove headings) below. We included the headings for your benefit, but it's 100% fine if you want to write your responses in some different structure.
---

# What is a String?

A string is a group of characters defined by being inside double ("") or single ('') quotations. Strings can be one word, sentence or a paragraph. They are how programs communicate with the users.
Example- "hello"

# What are some examples of information that would be Strings as opposed to some other data type?

Strings store data as text, such as a name ("Nikki") or an address ("321 North St"). You would store these information as strings as opposed to a number, which is for integers, or as a boolean, in which it would test if it was true or false.

# What is one way, using Ruby, to retrieve the 6th character in a String like `"Ada Lovelace"`? How about the 8th character? What happens if you try to retrieve the value of the _99th_ character (Or any character that doesn't exist)?

In Ruby, you can retrieve a character from a string by using the method str[n]. For this example, you would type "Ada Lovelace"[5] to retrieve the 6th character and "Ada Lovelance"[7] to retrieve the 8th character because in programming, counting begins at 0 instead of 1.
If you try to retrieve the 99th character or any character that does not exist, it comes back as nil, or nothing.

# The previous question asks about finding, for example, the 6th character in a String. Is it possible to find the **-6th** (Notice the negative symbol!) character in a String? What does that even mean?

In Ruby, if you use a negative number in character retrieval, it will run the process backwards and will begin to count from the end of the string instead of the beginning. Since there is no -0, the process begins at -1, which will always retrieve that last character in a string despite the length.

# What is one way, using Ruby, to replace certain characters in a string with some other set of characters? For example, given `"Sumeet Jain"`, how would you replace all of the `e` characters in my name with exclamation marks? (So it would be `"Sum!!t Jain"`.)

In Ruby, you can replace characters in a string with other characters by using the sub or gsub methods. Sub will replace only the first instance of this character while gsub will replace all instances.
name = "Sumeet Jain"
name = "name.gsub" ("e" , "!")
puts value

Prints "Sum!!t Jain"