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
