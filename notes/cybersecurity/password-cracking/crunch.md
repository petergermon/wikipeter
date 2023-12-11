\[ [Wikipeter](../../../README.md) > [Cybersecurity](../cybersecurity.md)  > [Password Cracking](password-cracking.md) > Crunch \]

# Crunch

**Crunch** is a command-line tool that can be used to generate custom wordlists. It is a powerful tool that can be used to create wordlists for a variety of purposes, including password cracking, dictionary attacks, and brute-force attacks.

To use Crunch, you will need to specify the following information:
- The minimum and maximum length of the words in the wordlist.
- The character set that you want to use.
- Any other options that you want to use.

1. For example, the following command will generate a wordlist of all possible combinations of lowercase letters from 2 to 6 characters in length:
	`crunch 2 6`
	This will generate a wordlist that contains all possible combinations of lowercase letters from 2 to 6 characters in length. The wordlist will be saved to standard output, so you will need to redirect it to a file if you want to save it.

2. You can also use crunch to generate wordlists that contain specific characters or patterns. For example, the following command will generate a wordlist that contains all possible combinations of lowercase letters, numbers, and symbols from 2 to 6 characters in length:c
	`crunch 2 6 -c abcdefghijklmnopqrstuvwxyz0123456789!@#$%^&*()`

3. To generate a wordlist of all possible combinations of lowercase letters, numbers, and symbols from 2 to 6 characters in length, and to remove common words and phrases from the wordlist:
	`crunch 2 6 -c abcdefghijklmnopqrstuvwxyz0123456789!@#$%^&*() -o`

4. To generate a wordlist of all possible combinations of lowercase letters, numbers, and symbols from 2 to 6 characters in length, and to save the wordlist to a file called wordlist.txt:
	`crunch 2 6 -c abcdefghijklmnopqrstuvwxyz0123456789!@#$%^&*() > wordlist.txt`
