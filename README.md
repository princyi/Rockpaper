# Rockpaper
PYTHON LANGUAGE
Slight Rock,Paper, &amp; Seissor game for Beginner level Project 

Code:-
import random
while True:
      my_answer = input("choose: rock, paper or scissors:")
      my_answer = my_answer.lower()

      if my_answer == "quit":
          break

      if my_answer != "rock" and my_answer != "paper" and my_answer !="scissors":
          print("Pleas choose a correct answers")
          continue

      computer_answer = random.choice(["rock","paper","scissors"])
      print(f"computer chose:{computer_answer}")

      if my_answer == computer_answer:
          print("you tied")
          continue
      elif my_answer == "paper"  and computer_answer == "rock":
          print("you win!")
          break
      elif my_answer == "rock" and computer_answer == "scissor":
          print("you win!")
          break
      elif my_answer == "scissor" and computer_answer == "paper":
          print("you win!")
          break
      else:
          print("you lose.try again!")

