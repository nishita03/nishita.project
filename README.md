#guessing game

import random

n=random.randint(1,99) 
a=0 #the no. of tries
x=False

name=input("Enter player name: ")
print("Hell!", name, ". Welcome to the GUESSING GAME!")

y=input("Enter 'Y' to play or 'Q' to quit: ")

if y.lower()=='q':
      print("Well, bye!")
      
elif y.lower()=='y':
      print("I'm thinking of a number between 1 to 100.")
      while not x:
            g=int(input("Enter you guessed number: "))
            a=a+1
            if g==n:
                x=True
            elif g>n:
                print("Guess a lower number.")
            elif g<n:
                print("Guess a higher number.")
       print("Congratulations! You win! You guess the number correctly.")
       print("The number was: ", n)
       print("It took you",a,"tries to get it right.")

#%%

#guess the color






