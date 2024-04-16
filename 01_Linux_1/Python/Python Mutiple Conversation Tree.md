# Python Mutiple Conversation Tree


import random
import string

def generate_password():
    characters = string.ascii_letters + string.digits + string.punctuation
    password = ''.join(random.choice(characters) for _ in range(12))
    return password

def main():
    print("Hello, how are you? Are you feeling good or bad?")
    answer_feeling = input().strip().lower()

    if answer_feeling == "good":
        print("Glad to hear! Would you like me to generate you a password? Yes or No?")
        answer_generate = input().strip().lower()

        if answer_generate == "yes":
            password = generate_password()
            print("Generated Password:", password)
        elif answer_generate == "no":
            print("Okay, have a nice day!")
        else:
            print("Invalid input.")

    elif answer_feeling == "bad":
        print("Sorry to hear that, can I make you feel better with a strong generated password? Yes or No?")
        answer_generate = input().strip().lower()

        if answer_generate == "yes":
            password = generate_password()
            print("Generated Password:", password)
        elif answer_generate == "no":
            print("Glad you feel bad :). Hope you never **** ******")
        else:
            print("Invalid input.")

    else:
        print("Invalid input.")

if __name__ == "__main__":
    main()
