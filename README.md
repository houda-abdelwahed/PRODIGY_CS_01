# PRODIGY_CS_01
caesar cipher with python
## How it works
The script uses a simple substitution cipher for encryption and decryption. Here's how it works:

### Encryption

1. Each character in the input message is converted to its ASCII value.
2. The encryption key is added to each ASCII value.
3. The modified ASCII values are converted back to characters.
4. The encrypted message is formed by joining these characters.

### Decryption

1. Each character in the encrypted message is converted to its ASCII value.
2. The encryption key is subtracted from each ASCII value.
3. The modified ASCII values are converted back to characters.
4. The decrypted message is formed by joining these characters.

# the code:
message_to_encrypt = input("Enter your text: ") \n
Key = int(input("Enter the key: ")) \n
encrypted_message = [(ord(i) + Key) for i in message_to_encrypt] \n
encrypted_message = [chr(i) for i in encrypted_message] \n
encrypted = "".join(encrypted_message) \n
decrypted_message = [(ord(i) - Key) for i in encrypted_message] \n
decrypted_message = [chr(i) for i in decrypted_message] \n
decrypted = "".join(decrypted_message) \n
print("The encrypted message is:", encrypted) \n
print("The decrypted message is:", decrypted) \n
