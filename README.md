# DungeonsAndDragonsDice

This is a program that helps roll as many die with as many sides as someone needs for the board game they are playing. 

This is a great app for any Dungeon and Dragons players. 

This program uses a while loop that relies on the random library to generate random numbers for the number of times there is dice and the range of numbers there is sides.

<img width="657" alt="Screen Shot 2022-07-29 at 9 50 50 PM" src="https://user-images.githubusercontent.com/66803124/181865736-33484ee8-43b3-46e9-a98d-918b6f11299a.png">

```
from random import randint
#need inputs for # of dice.
#need input for nested for loop for sides of dice.
num_dice = int(input("how many dice are you rolling? \n"))
num_sides = int(input("how many sides on each die? \n"))

while True:
    result ="|"
    for die in range(num_dice):
        rand = randint(1,num_sides)
        result += f"{rand}|"
    print(result)
    reply = input("Roll again? (q to quit)")
    if reply == "q":
        break
 ```
