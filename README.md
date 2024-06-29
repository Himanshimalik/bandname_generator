# bandname_generator
IT is a fun game program that generates band names with some information of the user.
Author: Himanshi Malik

#Code starts from here:
import random
rock = '''
    _______
---'   ____)
      (_____)
      (_____)
      (____)
---.__(___)
'''

paper = '''
    _______
---'   ____)____
          ______)
          _______)
         _______)
---.__________)
'''

scissors = '''
    _______
---'   ____)____
          ______)
       __________)
      (____)
---.__(___)
'''

#Write your code below this line 👇
print("Play Rock Paper Scissors with the computer ^.^\n")
user_choice = int(input("What do you choose? 0 for rock, 1 for paper and 2 for scissors.\n"))
print(user_choice)

computer_choice = random.randint(0,2)
print(computer_choice)

if user_choice == 0 and computer_choice == 1:
    print(f"{rock}\n{paper}\nYou lose.")
elif user_choice == 0 and computer_choice == 2:
    print(f"{rock}\n{scissors}\nYou Win! Hurrah!")
elif user_choice == 1 and computer_choice == 0:
    print(f"{paper}\n{rock}\nYou win! Hurrah!")
elif user_choice == 1 and computer_choice == 2:
    print(f"{paper}\n{scissors}\nYou lose :( Try again next time~")
elif user_choice == 2 and computer_choice == 0:
    print(f"{scissors}\n{rock}\nYou lose :( Try again next time~")
elif user_choice == 2 and computer_choice == 1:
    print(f"{scissors}\n{paper}\nYou Win! Hurrah!")
elif user_choice == computer_choice:
    print("Draw")
