# Shellcode_IA32

___Shellcode_IA32___ is a dataset containing _20_ years of shellcodes from a variety of sources is the largest collection of shellcodes in assembly available to date.

This dataset consists of 3,200 examples of instructions in assembly language for _IA-32_ (the 32-bit version of the x86 Intel Architecture) from publicly available security exploits. We collected assembly programs used to generate shellcode from [Exploit Database](https://www.exploit-db.com/shellcodes?platform=linux_x86) and from [shell-storm](http://shell-storm.org/shellcode/).
We enriched the dataset by adding examples of assembly programs for the _IA-32_ architecture from popular tutorials and books. This allowed us to understand how different authors and assembly experts comment and, thus, how to deal with the ambiguity of natural language in this specific context. Our dataset consists of 10% of instructions collected from books and guidelines, and the rest from real shellcodes. 

Our focus is on Linux, the most common OS for security-critical network services. Accordingly, we added assembly instructions written with _Netwide Assembler_ (NASM) for Linux.

Each line of _Shellcode\_IA32_ dataset represents a snippet - intent pair. The _snippet_ is a line or a combination of multiple lines of assembly code, built by following the NASM syntax. The _intent_ is a comment in the English language.


