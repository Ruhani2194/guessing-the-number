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
       
