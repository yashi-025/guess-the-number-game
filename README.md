# guess-the-number-game
import random
min=int(input("enter the lower limit:"))
max=int(input("enter the highest limit:"))
num=random.randint(min,max)
guess=None
count=0
while guess!=num:
    guess=int(input("guess the number:"))
    if guess==num:
        print("wohoo!! you won!!")
        count+=1
        print("total attempts taken:",count)
        if count<=5:
            print("superb gammer!! :)")
        else:
            print("good try")    
        break
    elif guess>num:
        print("too high!")
        count+=1
    elif guess<num:
        print("too low!") 
        count+=1   
    
