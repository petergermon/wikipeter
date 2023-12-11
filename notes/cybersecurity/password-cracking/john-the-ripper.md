\[ [Wikipeter](../../../README.md) > [Cybersecurity](../cybersecurity.md)  > [Password Cracking](password-cracking.md) > John The Ripper\]

# John The Ripper
John the Ripper is a powerful password cracking tool that supports a variety of encryption algorithms. It is a command-line tool, so you will need to be comfortable using the terminal. To use it, you will need to provide a list of possible passwords (in a text file), and then run the command:
`john --wordlist=password_list.txt filename.txt`

This command will run John the Ripper using the list of passwords provided (in the password_list.txt file) and the built-in rules. 

## Zip File Password Cracking
Here is the syntax to get the password hash of a zip file:
`zip2john file.zip > zip.txt`

The above command will get the hash from the zip file and store it in the zip.txt file. You can then use John to crack the hash.
`$john zip.txt`

## Dictionary Attacks
A dictionary attack is a type of password cracking technique which attempts to guess a password by trying commonly-used words or phrases. This type of attack is usually much faster than a brute-force attack and can be used with any type of encryption algorithm.

To use it for a dictionary attack, you will need to provide a list of possible passwords (in a text file) and then run the command:
`john --format=hashtype --wordlist=wordlist.txt filename.txt`

This command will run John the Ripper using the list of passwords provided and the built-in dictionary rules.

## Rainbow Table Attacks
A rainbow table attack is a type of password cracking technique which uses pre-computed hashes of commonly-used words or phrases to quickly guess a password. This type of attack is usually much faster than a brute-force attack and can be used with any type of encryption algorithm.

To use it for a rainbow table attack, you will need to provide a list of pre-computed hashes (in a text file) and then run the command:
`john --format=[hash type] --rainbow=[hash list]`

This command will run John the Ripper using the list of pre-computed hashes provided and the specified hash type. The --rainbow option will enable the rainbow table attack mode.
