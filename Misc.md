# Esoteric
Find the flag here:</br>
--[----->+<]>.++++++.-----------.++++++.[----->+<]>.----.---.+++[->+++<]>+.-------.++++++++++.++++++++++.++[->+++<]>.+++.[--->+<]>----.+++[->+++<]>++.++++++++.+++++.--------.-[--->+<]>--.+[->+++<]>+.++++++++.>--[-->+++<]>.

To understand what this code is, I made a plenty of research</br>
1. I searched as ***"What is esoteric"***, ***"Esoteric cryptography"***, ***"Esoteric coding"***
2. I found a clue while researching as ***"Esoteric coding"***
3. [Esoteric coding](https://en.wikipedia.org/wiki/Esoteric_programming_language) is "An esoteric programming language is a programming language designed to test the boundaries of computer programming language design, as a proof of concept, as software art, as a hacking interface to another language, or as a joke."
4. And the I found the answer, this coding is [Brainfuck](https://en.wikipedia.org/wiki/Esoteric_programming_language#Brainfuck)
5. [Brainfuck](https://en.wikipedia.org/wiki/Brainfuck) is "an esoteric programming language created in 1993 by Urban Müller. Notable for its extreme minimalism, the language consists of only eight simple commands and an instruction pointer. While it is fully Turing complete, it is not intended for practical use, but to challenge and amuse programmers."
6. The main issue was I don't know how to decode it and I found this [website](https://www.tutorialspoint.com/execute_brainfk_online.php)

![image](https://user-images.githubusercontent.com/50519199/121124792-2e8d6000-c82e-11eb-8846-97ba3a936e4a.png)

**flag{wtf_is_brainfuck}**

# Reggie McRegex
Find the flag in the attached file containing a haystack. Not including the quotes, the flag will be in the format of "flag{here_is_a_flag}". The text between the curly braces can consist of lowercase characters and underscores and be a maximum length of 16. You'll know it when you see it.</br>
Download haystack.txt

![image](https://user-images.githubusercontent.com/50519199/121124960-714f3800-c82e-11eb-8e4a-ee806a239ff2.png)

I opened the file by LibreOffice and there were 1555 pages, 726 words, 7.257.622 characters, and it is hard to find answer if you think read all of them.</br>
We have three clues given in the question:
1. The answer must be start as ***"flag{"***
2. The length of answer must be ***16 between the curly braces.***
3. The answer must be end as ***"}"***

Firstly, I run ``grep -o -e '.....................}\b' haystack.txt > haystackv1.txt`` to extract ending with "}" and inclueded "flag{"</br>
***Dot means number of character in the answer with flag{***</br>
Then, I run ``grep -o -e '\bflag{.................' haystackv1.txt`` to find which value start with "flag{"</br>
***Dot means number of character in the answer with }***

**flag{thy_flag_is_this}**

# Quit Messing With My Flags
This flag had an accident. What's it really supposed to be?</br>
flag{161EBD7D45089B3446EE4E0D86DBCF92}

I copied and pasted the value on Google Search, it's MD5 and decode it.

**flag{P@ssw0rd}**

# Find The Encoding
DeZmqMUkDJceycJHJPzZet

I used CyberChef to understand what is encoding and it's Base58

![image](https://user-images.githubusercontent.com/50519199/121127178-0c95dc80-c832-11eb-813d-74cca9e0b7f1.png)


**flag{not_base64}**
