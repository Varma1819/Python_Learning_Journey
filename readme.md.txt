print("I like Biriyani")
#this is my 1st python program


#VARAIBLES {Strings,Float,Integer,Boolean}

#For Strings
first_name = "Jaya" # in quotes
food = "biriyani"
email = "jaya123@gmail.com"
print(f"Hi {first_name}") #f means format when we want add any txt with the variable in {} we use f
print(f"Your like {food}")
print(f"yor mail-id was {email}")

#For Integers
age = 23 #no need to be in quotes
quantity = 3
print(f"Age was {age}")

#For Float
price = 10.99
gpa = 8.9
print(f"My Gpa is {gpa}")
print(f"the price is ${price}")

#For Boolean
is_student = True
for_sale = False
if for_sale:
    print("Item for sale")
else:
    print("not for sale")
if is_student:
    print("You are a student")
else:
    print("u r not a student")

OUTPUT:
I like Biriyani
Hi Jaya
Your like biriyani
yor mail-id was jaya123@gmail.com
Age was 23
My Gpa is 8.9
the price is $10.99
not for sale
You are a student

#Typeacasting = the processs of convertiong a varaible from one type to another { str(), int(), float(), bool()}

name ="Mantena Varma"
age = 23
gpa=3.2
is_student = True

print(type(is_student))
gpa = int(gpa)
print(gpa)

age= str(age)
print(age)
print(type(age))

age += "1"
print(age)

name = bool(name)
print(name)

OUTPUT:
<class 'bool'>
3
23
<class 'str'>
231
True



#user input ⌨️
#input() = A fun that prompts the user to enter data
#           Returns the data entered as a string

name=input("What is ur name?:")
age=input("What is ur age?:")

age=int(age) # OR U CAN GIVE AT THE TIME OF INPUT AS int(input("What is ur age?:"))
age = age +1
print(f"Hello{name}!")
print(f"My age is {age} !")
print("Hoo U R Men!")

OUTPUT
What is ur name?:MJR VARMA
What is ur age?:23
HelloMJR VARMA!
My age is 24 !
Hoo U R Men!

#Ex 1   Area of a rectangle

length = float(input("Enter the Len:"))
width = float(input("Enter the Wid:"))
area = length*width
print(f"Area of a rectangle is: {area}cm²")

Enter the Len:12
Enter the Wid:3
Area of a rectangle is: 36.0cm²


#Ex 2 Shpping Cart Program

item=input("what item would u like to buy?: ")
price=float(input("what is the price?: "))
quantity = int(input("how many u like?: "))
total=price * quantity

print(f"u have bought {quantity} x {item}/s")
print(f"u r total is : Rs{total}")

#o/p
what item would u like to buy?: Burgur
what is the price?: 80
how many u like?: 3
u have bought 3 x Burgur/s
u r total is : Rs240.0

# Madlibs game
# wordgame where u create a story by filly in blanks with random words

adjective1 = input("enter adje_1: ")
noun1 = input("enter a noun1: ")
adjective2 = input("enter adjec_1: ")

print(f"Today I went to a {adjective1} park")
print(f"There I saw a {noun1} bird")
print(f"It so {adjective2}")

#O/P
enter adje_1: Peace
enter a noun1: Woodpecker
enter adjec_1: beautiful
Today I went to a Peace park
There I saw a Woodpecker bird
It so beautiful

#Arthematic Operators

frnds =10
#frnds=frnds+1
#frnds +=1       # Argumented assigment operator
#frnds = frnds-2
#frnds -= 2
#frnds = frnds*3
#frnds *=3
#frnds = frnds/2
#frnds /=2
#frnds = frnds **2 i.e square
#frnds **=2
remainder = frnds % 3 # gives remainder by using modulus
print(remainder)

#Built in math related varaibles

x= 2.6
y=2
z=3.3
#result = round(x) # we can get round of that value
#result = abs(y)
#result=pow(4,4) # 4 to the power 4
#result = max(5,3)
#result = min(29,82)

print(result)
#O/P - 29


import math

x=9.37

#print(math.pi) #val of pie
#print(math.e) #exponential const
#result=math.sqrt(x)
#result = math.ceil(x) # always round floating point number to Up
#result = math.floor(x) #floor always down the floating point number


print(result)
#O/P- 9

#EX-1 - Circumference of a Circle i.e - 2*pi*r

import math

radius = float(input("enter the radius of a circle: "))

circumference = 2*math.pi*radius
print(f"the CCFS of circle was : {round(circumference, 2)}")

#output -
enter the radius of a circle: 10.5
the CCFS of circle was : 65.97


#EX-2 - Area of a Circle i.e - pi*r-square

import math

radius = float(input("enter the radius of a circle: "))

area = math.pi * pow(radius, 2)

print(f"the Area of circle was : {round(area, 2)}")

OUTPUT  -
enter the radius of a circle: 11.4
the Area of circle was : 408.28

#EX-3 - Hypothesys  of a ryt angel Triangle  i.e - root of (a^2 + b^2)

import math

a = float(input("enter side of a:"))
b = float(input("enter side of b: "))

c = math.sqrt(pow(a,2) + pow(b,2))
print(f"side of c: {c}")

O/P -
enter side of a:12
enter side of b: 34
side of c: 36.05551275463989












