# Petty_code
A repository of petty code from simple to complicated task
##Tip Calculator 
`print("Tip Calculator")
peep = float(input('Total amount of people? \n'))
total = float(input("Total amount for service: "))
tip= float(input("how many percent tip (15,20,25)%: "))
tips =float(total*tip/100)
nt=float(tips+total)
ori= (round(nt/peep))
print(f"Each of you will pay ${ori} and your grand total is {nt}")`

##Grade Calculator
`print("Student Grade system")
first = int(input("Enter your first CA Score (Over 20): "))
second = int(input("Enter your second CA Score (Over 20): "))
exam = int(input("Enter your Exam score (Over 60)"))
final = int(first+second+exam)
print(f"Your total score for this course is {final}")
if final >=90:
    print("Your grade for the course is A+")
elif final >= 85:
         print("Your grade for the course is A")
elif final >= 80:
    print("Your grade for the course is A-")
elif final >= 77:
         print("Your grade for the course is B+")
elif final >= 73:
         print("Your grade for the course is B")
elif final >= 70:
         print("Your grade for the course is B-")
elif final >= 65:
         print("Your grade for the course is C+")
elif final >= 60:
         print("Your grade for the course is C")
elif final >= 55:
         print("Your grade for the course is C-")
elif final >= 50:
         print("Your grade for the course is D")
elif final <= 49:
         print("Your grade for the course is F")        `

##Rollercoaster Ticket
height = int(input("Enter height(cm): "))
bill = 0
if height >= 175:
    print("You are eligible to ride")
    age=int(input("Enter your age: "))
    if age<=18:
        print("Your ticket is 12 euros")
        bill = 12
    elif age<=27:
        print("Your Ticket is 18 euros")
        bill = 18 
    elif age >=28:
        print("Your ticket is 25 euros")
        bill = 25
        vet = input("Are you a World War Two Vetran: ")
        if vet == "yes":
            bill=0
    photo=input("Do you want a photo during: ")
    if photo =="Yes":
        print("You have added a photo")
        bill += 3
    elif photo =="Yes" and vet =="yes":
        bill+=0
    if vet!="yes":
        print(f"Your total is {bill}euros")
    else:
        print("Thank you for your service and your ride is free")
else:
    print("Sorry you are not eligible to ride")

##Pizza ordering system 
size = input("Input the size of pizza (small,mid,large)\n")
bill=0
if size =="small":
    print("you have order a small pizza")
    bill=9
    tops=input('do you want extra cheese(yes or no)? \n ')
    if tops=="yes":
        bill+=1.5
    else:
        bill+=0
elif size =="mid":
    print("you have order a medium pizza")
    bill=15
    tops=input('do you want extra cheese(yes or no)? \n ')
    if tops=="yes":
        bill+=2.5
    else:
        bill+=0
elif size =="large":
    print("you have ordered a large pizza")
    bill=20
    tops=input('do you want extra cheese(yes or no)? \n ')
    if tops=="yes":
        bill+=2.5
    else:
        bill+=0
pep=input("do you want some pepperoni with your pizza (yes or no)? \n")
if pep =="yes":
    if size =="small":
        bill+=3
    elif size=="mid":
        bill+=4
    elif size=="large":
        bill+=5.5
else:
    bill+=0
print(f"Your total bill is {bill}")


