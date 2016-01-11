---
title: Strings
instructor_notes: Feel free to re-organize the headings (or add/remove headings) below. We included the headings for your benefit, but it's 100% fine if you want to write your responses in some different structure.
---

# What is a String?

A string is a way of holding data (usually characters forming words or sentences) that retains the order of the characters.

# What are some examples of information that would be Strings as opposed to some other data type?

Questions or answers the program needs to give to users would use a string, since strings are easy for someone who doesn't know code to read. Also any information that is static, that doesn't need to be manipulated mathematically, or information that needs to stay as a chunk to be plugged into other methods should be strings.

# What is one way, using Ruby, to retrieve the 6th character in a String like `"Ada Lovelace"`? How about the 8th character? What happens if you try to retrieve the value of the _99th_ character (Or any character that doesn't exist)?# The previous question asks about finding, for example, the 6th character in a String. Is it possible to find the **-6th** (Notice the negative symbol!) character in a String? What does that even mean?

Much like when you retrieve things from an array, you can use name_of_string[character] to find a specific character in a string. For example if hero = "Ada Lovelace" you can use hero[6] to retrieve "v." If you try to retrieve a number that is outside the number of characters in a string, it will return "nil," because nothing is there. If you ask for hero[-6], the negative tell Ruby to count from the end instead of the beginning of the string. (In this case, the answer will still be "v")


# What is one way, using Ruby, to replace certain characters in a string with some other set of characters? For example, given `"Sumeet Jain"`, how would you replace all of the `e` characters in my name with exclamation marks? (So it would be `"Sum!!t Jain"`.)

You can replace characters using .sub and .gsub (.sub will replace once, .gsub will replace all occurances). To turn your name into "Sum!!t Jain" (which woud be exciting) you can use name.gsub("e","!")
