"""Problem Description
Given an alphabet decryption key like the one below, create a program that can crack any message using the decryption key."""

alphabet = ["a", "b", "c", "d", "e", "f", "g", "h", "i", "j", "k", "l", "m", "n", "o", "p", "q", "r", "s", "t", "u", "v", "w", "x", "y", "z"]
abcs = "abcdefghijklmnopqrstuvwxyz"
decryption_key = ["!", ")", "$", "(", "£", "*", "%", "&", ">", "<", "@", "a", "b", "c", "d", "e", "f", "g", "h", "i", "j", "k", "l", "m", "n", "o"]
encrypted_abcs = "!)$(£*&><@abcdefghijklmno"

decryption_pairs = list(zip(alphabet, decryption_key))
# print(decryption_pairs)

my_message = "bridget"
# answer = input("encrypt or decrypt?")

def encrypt(message):
    encrypted_message = ""
    for letter in message:
        message_index = abcs.find(letter)
        letter = decryption_key[message_index+1]
        encrypted_message += letter
    return encrypted_message

print(encrypt(my_message))


def decrypt(message):
    decrypted_message = ""
    for letter in message:
        message_index = encrypted_abcs.find(letter)
        letter = alphabet[message_index+1]
        decrypted_message += letter
    return decrypted_message

print(decrypt("$h<£&*j"))
