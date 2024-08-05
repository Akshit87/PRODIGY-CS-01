def encrypt(text, shift):
    result = ""
    for i in range(len(text)):
        char = text[i]
        # Encrypt uppercase characters
        if char.isupper():
            result += chr((ord(char) + shift - 65) % 26 + 65)
        # Encrypt lowercase characters
        elif char.islower():
            result += chr((ord(char) + shift - 97) % 26 + 97       
        # Add non-alphabetic characters as is
        else:
            result += char
    return result
def decrypt(text, shift):
    return encrypt(text, -shift)
def main():
    while True:
        choice = input("Do you want to (E)ncrypt or (D)ecrypt a message? (E/D): ").upper(    
        if choice in ['E', 'D']:
            message = input("Enter your message: ")
            shift = int(input("Enter shift value: "))
            if choice == 'E':
                print("Encrypted message:", encrypt(message, shift))
            else:
                print("Decrypted message:", decrypt(message, shift)          
            break
        else:
            print("Invalid choice. Please enter 'E' to encrypt or 'D' to decrypt.")
if __name__ == "__main__":
    main()
