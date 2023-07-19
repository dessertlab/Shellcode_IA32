# Shellcode_IA32

___Shellcode_IA32___ is a dataset containing more than _20_ years of shellcodes from a variety of sources and is the largest collection of shellcodes in assembly available to date. We are currently extending the dataset. Up to now, we released three versions of the dataset.

## Version 1: Shellcode_IA32

***Shellcode_IA32*** was presented for the first time in the paper [Shellcode_IA32: A Dataset for Automatic Shellcode Generation](https://aclanthology.org/2021.nlp4prog-1.7), accepted to the 1st Workshop on Natural Language Processing for Programming (NLP4Prog 2021). 
This version consists of 3,200 examples of instructions in assembly language for _IA-32_ (the 32-bit version of the x86 Intel Architecture) from publicly available security exploits. We collected assembly programs used to generate shellcode from [exploit-db](https://www.exploit-db.com/shellcodes?platform=linux_x86) and from [shell-storm](http://shell-storm.org/shellcode/).
We enriched the dataset by adding examples of assembly programs for the _IA-32_ architecture from popular tutorials and books. This allowed us to understand how different authors and assembly experts comment and, thus, how to deal with the ambiguity of natural language in this specific context. Our dataset consists of 10% of instructions collected from books and guidelines, and the rest from real shellcodes. 

Our focus is on Linux, the most common OS for security-critical network services. Accordingly, we added assembly instructions written with _Netwide Assembler_ (NASM) for Linux.

Each line of _Shellcode\_IA32_ dataset represents a snippet - intent pair. The _snippet_ is a line or a combination of multiple lines of assembly code, built by following the NASM syntax. The _intent_ is a comment in the English language.

We conducted an extensive experimental evaluation using the _Shellcode\_IA32_ dataset in the journal paper [Can we generate shellcodes via natural language? An empirical study](https://doi.org/10.1007/s10515-022-00331-3), published in the Automated Software Engineering (AUSE) journal. The paper also contains further statistics on the dataset.

## Version 2: Decoder Dataset

Shellcode_IA32 dataset has been extended to build the ***Decoder Dataset*** (an assembly dataset used for decoding the encoded shellcodes) presented in the paper [EVIL: Exploiting Software via Natural Language](https://doi.org/10.1109/ISSRE52982.2021.00042). The extended dataset and the code to reproduce the experiments of the paper can be found on [this GitHub repository](https://github.com/dessertlab/EVIL). This second version of the dataset includes 3,715 assembly code snippets with their description in the English language.


## Version 3: Extended_Shellcode_IA32

We further enriched the dataset (***Extended_Shellcode_IA32***) with additional samples of shellcodes collected from publicly available security exploits, reaching 5,900 unique pairs of assembly code snippets/English intents. 

Our dataset also includes 1,374 intents (~23% of the dataset) that generate multiple lines of assembly code, separated by the newline character \n. These multi-line snippets contain many different assembly instructions (e.g., whole functions).
