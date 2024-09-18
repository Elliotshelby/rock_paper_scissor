#you can also copy the code from here directly

import random
rock= '''
    _______
---'   ____)
      (_____)
      (_____)
      (____)
---.__(___)'''

paper= '''
     _______
---'    ____)____
           ______)
          _______)
         _______)
---.__________)'''

Scissor='''
  _______
---'   ____)____
          ______)
       __________)
      (____)
---.__(___)'''

user_input=int(input("What do you choose? Type 0 for Rock, 1 for Paper or 2 for Scissors"))
print("you chooses\n")
if user_input==0:
  print(rock)
elif user_input==1:
  print(paper)
elif user_input==2:
  print(Scissor)
else:
  print("Invalid input")
comp=random.randint(0,2)
if comp==0:
  print(rock)
elif comp==1:
  print(paper)
elif comp==2:
  print(Scissor)

if user_input==comp:
  print("its a tie")
elif user_input==0 and comp==1:
  print("you lose :(")
elif user_input==0 and comp==2:
  print("you win :)")
elif user_input==1 and comp==0:
  print("you win :)")
elif user_input==1 and comp==2:
  print("you lose :(")
elif user_input==2 and comp==0:
  print("you lose :(")
elif user_input==2 and comp==1:
  print("you lose :(")
