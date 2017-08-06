# VIGINERE_CIPHER
Program encrypts the text using Viginere cipher. Decryption is possible IF the same KEYWORD and OFFSET will be used for decrypting.

To get executable file called "vgnr" call in terminal program "make" in directory containing files "makefile", "main.c", "operate.c" and "operate.h".

Implementation feature is that the KEYWORD and OFFSET (alphabet offset) defined in file "operate.c".
It might be not convenient if dymanic encrypting/decrypting with different keywords and offsets is needed, but it could be implemented with some upgrade of the code.
In case of changing the keyword OR offset value you should execute make again to get the executable file "vgnr" with desired keyword and offset.


To encrypt:
    - place the file with text in same directory with the executable;
    - execute the program "vgnr" with first parameter - name of the file with open text - and second parameter - action "code";
      Example: ./vgnr opentext code - to encrypt the text in file named "opentext";
      The result of this action is file named "coded" which contains the ciphered text depending on specified KEYWORD and OFFSET.

To decrypt:
    - executable "vgnr" and file with encrypted text should be in the same directory;
    - execute the program "vgnr" and specify name of the file that contains the text to decrypt as first parameter and action "decode" as second parameter;
      Example: ./vgnr coded decode
      The result of this action is file named "decoded" which contains the decrypted text depending on specified KEYWORD and OFFSET.
