# rock_paper_sissor
Rock, Paper, Scissors is a simple game where the user competes with the computer using basic rules and random selection.

mport random
'''
1 for rock
-1 for paper
0 for sissor
'''
computer=  random.choice([-1, 0, 1])
youstr= input("Enter your choice: ")
youDict= {"r":1, "p":-1, "s":0}
reverseDict = {1: "Rock", -1:"Paper", 0:"Sissor"}

you = youDict[youstr]

print(f"You chose{reverseDict[you]}\ncomputer chose {reverseDict[computer]} ")

if(computer == you):
    print("its draw")

else:
    if(computer == -1 and you == 1):
        print("you win")

    elif(computer == 1 and you == -1):
        print("you lose")

    elif(computer == -1 and you == 0):
        print("you win")

    elif(computer == 0 and you == -1):
        print("you lose")

    elif(computer == 1 and you == 0):
        print("you lose")

    elif(computer == 0 and you == 1):
        print("you win")

    
    else:
        print("something went wrong")
    

