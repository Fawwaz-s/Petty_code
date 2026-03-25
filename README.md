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

def calcule():
    trun = ('T','R','U','E')
    love = ('L','O','V','E')
    
    man = input('Enter your name: ').upper()
    woman = input('Enter your name:').upper()
    
    

    for man in trun:
        countman= trun.count(man)     
    
    for man in love:
        countman1= love.count(man)
     
    for woman in trun:
        countwoman= trun.count(woman)
    
    for woman in love:
        countwoman1= love.count(woman)
    
    score = (countman +countman1+ countwoman + countwoman1)
    
    print(f'Your score is {score}' )
       
calcule()

---dictionary--

jers = {
    'name':'Fawaz',
    'song'  :'Faded',
    'movie' :'Inception',
    'food'  :'Pizza',
}

print(nams['food']) # will print pizza

#nams['gf'] = 'Sana' # will add new entry into dictionary

jers = {}
print (vers) # will print an empty line 
#nams['gf'] ='We shall'
#print(nams['gf']) #for replacing an entry

for key in jers:
    print(key) # this will just print the keys from jers (name, song,...)
    print(jers[key]) # will print the values (fawaz, faded...)

---------
to use for working with dictionanries
jers.key()
jers.values()
jers.items()

nested dictionaries and list 
travel = {
    'france' :{
        'cities' : ["Paris", "Marseille", "Lyon"]
        },
    'italy' : {
        "cities" : ["Rome", "Milan", "Venice",['Florence', 'Naples']]},
    'spain' : {
        "cities" : ["Madrid", "Barcelona", "Valencia"]
        },
    }

print(travel["italy"]['cities'][3][0]) #Florence

----an aunctioneer---
oruko = input("Enter your name: ")
bid = input("Enter your bid: $")

dico = { oruko: bid }

while True:
    a = input("Are there any other bidders? Type 'yes' or 'no': ").lower()
    if a == "yes":
        oruko = input("Enter a name: ")
        bid = input("Enter your bid: $")
        dico[oruko] = bid
    else:
        if a == "no":
            break
for key in dico:
    if dico[key] == max(dico.values()):
        print(f"The winner is {key} with a bid of ${dico[key]}")
print(dico)

------calculator with dictionary----
def add(a, b):
    return a + b
def subtract(a, b):
    return a - b
def multiply(a, b):
    return a * b
def divide(a, b):
    return a / b

dick = {
    "+": add,
    "-": subtract,
    "*": multiply,
    "/": divide
}

num1 =int(input("Enter first number: "))
num2 =int(input("Enter second number: "))
operation = input("Enter operation (+, -, *, /): ")
ab = True
if operation == "+":
    print(dick["+"](num1, num2))
elif operation == "-":
    print(dick["-"](num1, num2))
elif operation == "*":
    print(dick["*"](num1, num2))
elif operation == "/":
    print(dick["/"](num1, num2))
answer = dick[operation](num1, num2)
print(f'{num1}{operation}{num2}= {dick[operation](num1, num2)}')
    
ab = True
while ab == True:
    pen = input('Do you want to continue with your answer? \n y or n or c to start again ?').lower()
    if pen == 'c':
        operation = (input("Enter operation (+, -, *, /): "))
        num3 = int(input("Enter third number: "))
        if operation == "+":    
            print(dick["+"](answer, num3))
        elif operation == "-":
            print(dick["-"](answer, num3))
        elif operation == "*":
            print(dick["*"](answer, num3))
        elif operation == "/":
            print(dick["/"](answer, num3))
        print(f'{answer}{operation}{num3}= {dick[operation](answer, num3)}')
        
    elif pen == 'y':
        num1 =int(input("Enter first number: "))
        num2 =int(input("Enter second number: "))
        operation = input("Enter operation (+, -, *, /): ")
        if operation == "+":    
            print(dick["+"](num1, num2))
        elif operation == "-":
            print(dick["-"](num1, num2))
        elif operation == "*":
            print(dick["*"](num1, num2))
        elif operation == "/":
            print(dick["/"](num1, num2))
        print(f'{num1}{operation}{num2}= {dick[operation](num1, num2)}')
    else:
        if pen == 'n':
            ab = False
            print('welcome')
---------------------------------------------------------------------------
GUESSING GAME WITH LIVES
import random

def choose():
    jap = input('Choose difficulty: Easy, Medium, Hard: ').capitalize()
    
    if jap == "Easy":
        number = random.randint(1, 100)
        lives = 10
        guess = False
        
        print(f"Difficulty set to Easy. You have {lives} lives.")

        while guess != True:
            storm = int(input('Enter a number between 1 and 100: '))

            if storm == number:
                print("Congratulations! You guessed the number.")
                guess = True
                
            elif storm > number:
                lives -= 1
                print("Wrong!! Your guess is too high.")
                if lives > 0:
                    print(f"You have {lives} lives remaining.")
            else:
                lives -= 1
                print("Wrong!! Your guess is too low.")
                if lives > 0:
                    print(f"You have {lives} lives remaining.")

        if lives == 0:
            print(f"Game Over! The number was {number}.")
            
    elif jap == "Medium":
        number = random.randint(1, 100)
        lives = 5
        guess = False
        
        print(f"Difficulty set to Medium. You have {lives} lives.")

        while guess != True:
            storm = int(input('Enter a number between 1 and 100: '))

            if storm == number:
                print("Congratulations! You guessed the number.")
                guess = True
                
            elif storm > number:
                lives -= 1
                print("Wrong!! Your guess is too high.")
                if lives > 0:
                    print(f"You have {lives} lives remaining.")
            else:
                lives -= 1
                print("Wrong!! Your guess is too low.")
                if lives > 0:
                    print(f"You have {lives} lives remaining.")

        if lives == 0:
            print(f"Game Over! The number was {number}.")
            
    elif jap == "Hard":
        number = random.randint(1, 100)
        lives = 3
        guess = False
        
        print(f"Difficulty set to Hard. You have {lives} lives.")

        while guess != True:
            storm = int(input('Enter a number between 1 and 100: '))

            if storm == number:
                print("Congratulations! You guessed the number.")
                guess = True
                
            elif storm > number:
                lives -= 1
                print("Wrong!! Your guess is too high.")
                if lives > 0:
                    print(f"You have {lives} lives remaining.")
            else:
                lives -= 1
                print("Wrong!! Your guess is too low.")
                if lives > 0:
                    print(f"You have {lives} lives remaining.")

        if lives == 0:
            print(f"Game Over! The number was {number}.")
             
    else:
       print("Invalid difficulty level")
                
choose()


-----------------------------------------------------------------------------------------------------------------------------
import random

data = [
    {
        'name': 'Bukayo Saka',
        'google_searches': 920000,
        'occupation': 'footballer'
    },
    {
        'name': 'Lionel Messi',
        'google_searches': 1850000,
        'occupation': 'footballer'
    },
    {
        'name': 'Cristiano Ronaldo',
        'google_searches': 3200000,
        'occupation': 'footballer'
    },
    {
        'name': 'Taylor Swift',
        'google_searches': 4500000,
        'occupation': 'singer'
    },
    {
        'name': 'MrBeast',
        'google_searches': 2800000,
        'occupation': 'youtuber'
    },
    {
        'name': 'Kylian Mbappé',
        'google_searches': 1100000,
        'occupation': 'footballer'
    },
    {
        'name': 'Selena Gomez',
        'google_searches': 2100000,
        'occupation': 'singer & actress'
    },
    {
        'name': 'Elon Musk',
        'google_searches': 1650000,
        'occupation': 'businessman'
    },
    {
        'name': 'Virat Kohli',
        'google_searches': 1350000,
        'occupation': 'cricketer'
    },
    {
        'name': 'Zendaya',
        'google_searches': 1900000,
        'occupation': 'actress'
    }
]

def topgame():

    
    guess = False
    counter = 0
    
    
            
    while guess != True:
            item1 = random.choice(data) 
            item2 = random.choice(data)
    
            oruko = item1['name']
            oruko2 = item2['name']
    
            meta = item1['google_searches']
            meta2 = item2['google_searches']
            
            staff = input(f"Which one has more google searches? {oruko} or {oruko2} ? ").title()
            
            if staff != oruko and staff != oruko2:
                print('Invalid input! Please choose either of the two options.')
                continue
            
            if (meta > meta2) and (staff == oruko):
                print('Correct!')
                counter += 1
           
            elif (meta < meta2) and (staff == oruko2):
                print('Correct!')
                counter += 1
           
            elif (meta > meta2) and (staff == oruko2):
                print('Wrong!')
                print(f'Your final score is {counter}')
                guess = False
            
            elif (meta < meta2) and (staff == oruko):
                print('Wrong!')
                print(f'Your final score is {counter}')
                guess = False
       
            
    
   
topgame()
        
    
       

