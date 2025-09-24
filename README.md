# 🐶 Simple Guess the Animal Game for Kids

animals = {
    "cat": "I like to chase mice and I say 'meow'.",
    "dog": "I am a loyal friend and I say 'woof'.",
    "cow": "I give milk and I say 'moo'.",
    "lion": "I am the king of the jungle and I roar loudly.",
    "elephant": "I am very big and I have a long trunk."
}

def main():
    print("🎮 Welcome to Guess the Animal!")
    print("I will describe an animal, and you try to guess it.\n")

    for animal, clue in animals.items():
        print("🤔 Clue:", clue)
        guess = input("Your guess: ").lower().strip()
        if guess == animal:
            print("🎉 Correct! It's", animal, "\n")
        else:
            print("❌ Oops! The answer was", animal, "\n")

    print("👏 Game over! Thanks for playing!")

if __name__ == "__main__":
    main()
