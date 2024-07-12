import random
Rock = '''
    _______
---'   ____)
      (_____)
      (_____)
      (____)
---.__(___)
'''
Paper = '''
     _______
---'    ____)____
           ______)
          _______)
         _______)
---.__________)
'''
Scissors = '''
    _______
---'   ____)____
          ______)
       __________)
      (____)
---.__(___)
'''
# 1- Rock, 2- Paper. 3- Scissors
game = {
    (1, Rock): "Draw",
    (1, Paper): "Lost",
    (1, Scissors): "Won",
    (2, Rock): "Won",
    (2, Paper): "Draw",
    (2, Scissors): "Lost",
    (3, Rock): "Lost",
    (3, Paper): "Won",
    (3, Scissors): "Draw"
}
Times = int(input("How many times are you playing: (1) , (2) or (3): "))
# Decision = "YES"
score, score2 = 0, 0
while Times > 0:
    Robot_Choice = random.choice([Rock, Paper, Scissors])
    Your_Choice = int(input("Enter: \nA) 1 For Rock\nB) 2 For Paper\nC) 3 For Scissors\nEnter: "))
    Result = game[Your_Choice, Robot_Choice]
    if Result == "Won":
        score += 1
    if Result == "Lost":
        score2 += 1
    if Your_Choice == 1:
        Your_Choice = Rock
    elif Your_Choice == 3:
        Your_Choice = Scissors
    elif Your_Choice == 2:
        Your_Choice = Paper
    print(f"You played: \n{Your_Choice}\n The Robot played: \n{Robot_Choice} \n You {Result}")
    # Decision = input("Do you want to play again ?\n (Yes) | (No): ").upper()
    Times -= 1
if score > score2:
    Final_Result = f"You got {score} points and the robot got {score2}, you won !"
elif score < score2:
    Final_Result = f"You got {score} points and the robot got {score2}, you lost !"
else:
    Final_Result = f"You both got {score} Its a draw"
print(f"{Final_Result}")
