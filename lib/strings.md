---
title: Strings
instructor_notes: Feel free to re-organize the headings (or add/remove headings) below. We included the headings for your benefit, but it's 100% fine if you want to write your responses in some different structure.
---

# What is a String?

    #A string is any combination of characters with either single or double quotes at the beginning and end of
    #the characters. Also, the quotation marks have to match.

# What are some examples of information that would be Strings as opposed to some other data type?

    # text
    # passwords, user input
    # can assign them to variables
    # if you want to display a message

# What is one way, using Ruby, to retrieve the 6th character in a String like `"Ada Lovelace"`? How about the 8th character? What happens if you try to retrieve the value of the _99th_ character (Or any character that doesn't exist)?
   
    # you can retrieve characters based on their index, you just have to remember that indexes start at 0, not 1.
    #x = "Ada Lovelace"
    #(6th character)    puts x[5]    
    #(8th character)    puts x[7]
    
    # puts x[21] will run without causing an error, and will output a blank space since
    #that character does not exist. So it appears to have no output 

# The previous question asks about finding, for example, the 6th character in a String. Is it possible to find the **-6th** (Notice the negative symbol!) character in a String? What does that even mean?

    #Yes, finding the -6th character of a string is possible. Instead of moving from left to
    # right, it will go from right to left. The index of the last character of the string is -1,
    #instead of 0. Then the second to last character is -2 and so forth.

# What is one way, using Ruby, to replace certain characters in a string with some other set of characters? For example, given `"Sumeet Jain"`, how would you replace all of the `e` characters in my name with exclamation marks? (So it would be `"Sum!!t Jain"`.)
   
    # global substitution method will replace a given string anytime it appears. If you only want to 
    #replace the given string the first time it appears you can use the substitution method.
    
    #puts "Sumeet Jain".gsub("e","!")
