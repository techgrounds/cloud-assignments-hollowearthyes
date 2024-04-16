# Python password generator


import random
import string


characters = string.ascii_letters + string.digits + string.punctuation

password = ""

while len(password) < 30:

    random_number = random.randint(1, 9)

    random_letter = random.choice(string.ascii_lowercase + string.ascii_uppercase)

    random_character = random.choice(characters)

    password += str(random_number) + random_letter + random_character

password = password[:30]

print("Generated Password:", password)
