# Gronsfeld-Cipher


The code defines two functions: encrypt and decrypt, which perform encryption and decryption using the Gronsfeld cipher, respectively.

The encrypt function takes two parameters: message (the input message to be encrypted) and key (the sequence of digits used for encryption). It initializes an empty string encryptedMessage to store the encrypted message.

It iterates over each character in the message string. If the character is an alphabet (checked using std::isalpha), it determines the base character ('a' or 'A') based on the case of the character. It calculates the shift value by converting the corresponding digit from the key string to an integer.

It applies the shift to the character by subtracting the base, adding the shift value, taking the modulo 26 to wrap around the alphabet, and finally adding the base back. The resulting character is appended to the encryptedMessage.

The decrypt function is similar to encrypt but reverses the shift to decrypt the message.

The main function prompts the user to enter the message and key. It then calls the encrypt function to encrypt the message using the provided key and displays the encrypted message.

Next, it calls the decrypt function to decrypt the encrypted message using the same key and displays the decrypted message.

The program terminates after displaying the results.

This code correctly handles the encryption and decryption of messages using the Gronsfeld cipher, considering spaces between words without applying any shift.
