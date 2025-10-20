def encrypt(original_text, shift_amount):
    encrypted_text = ""

    for char in original_text:
        position = alphabet.index(char)
        new_position = (position + shift_amount) % 26
        shifted_letter = alphabet[new_position]
        encrypted_text += shifted_letter

    print(f"Here is the encoded result: {encrypted_text}")
