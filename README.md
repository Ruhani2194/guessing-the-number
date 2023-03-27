# guessing-the-number
import random
random_number=random.randint(1,100)

guess=int(input("Guess the Number:"))
chances=5
while guess!=random_number:

    if guess>random_number:
        chances=chances-1
        if chances==0:
            print("You Loss the Game!")
            break
        print("Guess is High!")
        print("You Have",chances,"Chances")
        guess=int(input("Guess the Number:"))

    elif guess<random_number:
        chances=chances-1
        if chances==0:
            print("You Loss the Game!")
            exit()
        print("Guess is Low!")
        print("You Have",chances,"Chances")
        guess=int(input("Guess the Number:"))
print("Congratulations! You Have Won!")


