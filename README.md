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
    print(jers[key]) # will print the values (fawaz, song...)

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
