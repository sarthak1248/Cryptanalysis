# COMPARATIVE ANALYSIS OF  CRYPTOGRAPHIC ALGORITHMS
The project aims at taking a step into the field of cryptanalysis by comparing various traditional cryptographic algorithms based on their execution time and output complexity. The traditional cryptographic algorithms (ciphers) which will be analyzed are Caesar cipher, Vigenere cipher, and one-time pad cipher. 
The Project consists of the main program which will include all the three ciphers and the menu which has options for using the ciphers. The program will have an opening menu where the user can select the option in which the cipher does, he wants to encrypt or decrypt his input. The cipher will generate the encrypted or decrypted output along with the execution time. This relative practical use of ciphers parallelly will help us understand their mechanism when performed on a similar input, and, will finally be useful to compare and contrast them.

The following distinct ciphers will be analyzed:

1.	Caesar Cipher: It is one of the very earliest and simplest forms of coding a message. It’s simply a type of substitution cipher. Put simply each letter is shifted an exact number of letters away from the original letter. For example, using a key of two, letter 'A' would become 'C' and 'D' would become 'F' in the coded message. The encryption can be represented using modular arithmetic by first transforming the letters into numbers, according to the scheme, A = 0, B = 1…, Z = 25, then encryption of a letter by a shift n can be described mathematically as En(x)=(x+n) mod 26 (where En(x) is Encryption Phase with shift n) and Dn(x)=(x-n) mod 26 (where Dn(x) Decryption Phase with shift n). This cipher is named after Julius Caesar, who used it in his private correspondence.

2.	Vigenere Cipher: The Vigenere cipher, was invented by a Frenchman, Blaise de Vigenere in the 16th century. It utilizes a simple form of polyalphabetic substitution. A polyalphabetic cipher is any cipher based on substitution, using multiple substitution alphabets. The encryption of the original text is done using the Vigenere square or Vigenere table. The table consists of the alphabet written out 26 times in different rows, each alphabet shifted cyclically to the left compared to the previous alphabet, corresponding to the 26 possible Caesar Ciphers. The cipher uses a different alphabet from one of the rows and the alphabet used at each point depends on a repeating keyword.

For example, if the plaintext is 'Geeks' and the key used is 'Ayush', the first letter of the plaintext, G is paired with A, the first letter of the key. So, use row G and column A of the Vigenere square, namely G. Similarly, for the second letter of the plaintext, the second letter of the key is used, the letter at row E, and column Y is C. The rest of the plaintext is enciphered similarly. Decryption is performed by going to the row in the table (shown in Fig 1.2) corresponding to the key, finding the position of the ciphertext letter in this row, and then using the column’s label as the plaintext.

 
3.	One-time pad (OTP): This encryption method is a binary additive stream cipher, where a stream of truly random keys is generated and then combined with the plain text for encryption or with the ciphertext for decryption by an ‘exclusive OR’ (XOR) addition. To encrypt plain text data, the sender uses a key string equal or more in length to the plain text. The key is used by mixing (XOR- ing) bit by bit, always a bit of the key with a bit of the plain text to create a bit of ciphertext. First described by Frank Miller in 1882, the one-time pad was re-invented in 1917. On July 22, 1919,
U.S. Patent 1,310,719 was issued to Gilbert Vernam for the XOR operation used for the encryption of a one-time pad.

One-time pad encryption is a very simple, yet completely unbreakable cipher method if the following conditions are strictly fulfilled:

•	The key must be truly random.
•	The key must be at least as long as the plaintext.
•	The key must never be reused in whole or in part
•	The key must be kept completely secret.

The security strength of the traditional one-time-pad encryption system depends on the randomness of the secret key. However, it can be hard to generate a truly random key by using the existing technologies and methods. Therefore, we pay more attention to the logical operation used in the encryption and decryption but not to how to generate the random key. This cipher has been used for decades in electronic cipher systems for encrypting customers’ sensitive data. the key used for encoding the message is completely random and is as long as the message itself. That is why the only possible attack on such a cipher is a brute force attack.
