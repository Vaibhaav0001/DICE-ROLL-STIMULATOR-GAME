
import random
print("$$$ DICE ROLL STIMULATOR GAME $$$")
print()
print("Rules:One who will have max number obtain will win this game")
print()
print("How many players are there to play")
n=int(input())
temp={}
for i in range(1,n+1):
    print("player",i,"enter",i,"to roll the dice",end=" ")
    j=int(input())
    if j==i:
        no=random.randint(1,6)
        print(no)
        temp[i]=no
    else:
        print("wrong input!",end=" "+"XXXXXXX"+" "+"You are out.")
        print()
largest=max(temp.values())
for key,value in temp.items():
    if value==largest:
        print("Conratulations!!!",key,"you are Winner",value)
        
