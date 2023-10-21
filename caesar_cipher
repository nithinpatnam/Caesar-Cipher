def caesar_cipher(text, shift):
    result = ""

    for char in text:
        if char.isalpha():
            # Determine the case (uppercase or lowercase)
            case = ord('A') if char.isupper() else ord('a')

            # Apply the shift and wrap around the alphabet
            result += chr((ord(char) - case + shift) % 26 + case)
        else:
            # If the character is not a letter, leave it unchanged
            result += char

    return result

# Get user input
plaintext = input("Enter the text to encrypt/decrypt: ")
shift_amount = int(input("Enter the shift amount (positive for encryption, negative for decryption): "))

# Encrypt/decrypt the input text
encrypted_text = caesar_cipher(plaintext, shift_amount)

# Display the results
print(f"\nOriginal text: {plaintext}")
print(f"Shift amount: {shift_amount}")
print(f"Result: {encrypted_text}")
