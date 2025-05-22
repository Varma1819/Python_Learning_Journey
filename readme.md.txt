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

 if statements 🤔
#if = Do some code If some conditionis true
#        Else do something else

EX:1
age = int(input("enter ur age:"))

if age >= 100:
    print("you are too old to get Credit Card!")
elif age >18:
    print("you are eligible for Credit Card")
else:
    print("Your are Not eligible for Credit card!")

#OUTPUTS

#enter ur age:18
#Your are Not eligible for Credit card!

#enter ur age:22
#you are eligible for Credit Card!

#enter ur age:111
#you are too old to get Credit Card!

Ex:2
response = input("Do u like the car? (Y/N): ")

if response == "Y": #Comparision Operator
    print("Get into the car!")
else:
    print("Oh! Good Bye then....")

#OUTPUTS

#Do u like the car? (Y/N): N
#Oh! Good Bye then....

#Do u like the car? (Y/N): Y
#Get into the car!

EX:3
Car_for_sale=False

if Car_for_sale:
    print("It is $5000 only!")
else:
    print("Not for sale!")

#OUTPUT
#It is $5000 only!  (if it is True)
#Not for sale!

⭐ calculator program 🧮 USING IF STATEMENTS ONLY

#Python calculator program 🧮

operator = input("Enter an Operator ( + - * / ):")
num1 = float(input("Enter num1:"))
num2 = float(input("Enter num2:"))

if operator == "+":
    result = num1+num2
    print(result)
elif operator == "-":
    result = num1-num2
    print(result)
elif operator == "*":
    result = num1*num2
    print(result)
elif operator == "/":
    result = num1/num2
    print(round(result,3)) #To round upto 3 decimal values after .

else:
    print(f"{operator} is invalid operator!")

#OUTPUTS

#Enter an Operator ( + - * / ):-
#Enter num1:2
#Enter num2:4
#-2.0

#Enter an Operator ( + - * / ):**
#Enter num1:23
#Enter num2:24
#** is invalid operator!

#Enter an Operator ( + - * / ):/
#Enter num1:24
#Enter num2:83
#0.2891566265060241

#Enter an Operator ( + - * / ):/
#Enter num1:28
#Enter num2:12
#2.333

⭐Python weight conversion program 🏋️
#Python weight conversion program 🏋️

weight=float(input("enter your weight:"))
unit=input("Kilograms or Pounds? (K or L): ")

if unit == "K":
    weight = weight*2.205
    unit = "Lbs."
    print(f"Your weight is: {round(weight,1)} {unit}")
elif unit =="L":
    weight = weight/2.205
    unit = "Kgs."
    print(f"Your weight is: {round(weight,1)} {unit}")
else:
    print(f"{unit} was not valid")


#OUTPUTS

#enter your weight:234
#Kilograms or Pounds? (K or L): L
#Your weight is: 106.1 Kgs.

#enter your weight:95
#Kilograms or Pounds? (K or L): K
#Your weight is: 209.5 Lbs.

⭐ temperature conversion program 🌡️

unit = input("Is this temperature in Celsius or Fahrenheit (C/F): ")
temp = float(input("Enter the temperature: "))

if unit == "C":
    temp = round((9 * temp) / 5 + 32, 1)
    print(f"The temperature in Fahrenheit is: {temp}°F")
elif unit == "F":
    temp = round((temp - 32) * 5 / 9, 1)
    print(f"The temperature in Celsius is: {temp}°C")
else:
    print(f"{unit} is an invalid unit of measurement")

#OUTPUT
#Is this temperature in Celsius or Fahrenheit (C/F): F
#Enter the temperature: 134
#The temperature in Celsius is: 56.7°C

#Is this temperature in Celsius or Fahrenheit (C/F): C
#Enter the temperature: 45
#The temperature in Fahrenheit is: 113.0°F

logical operators 🌦️ = evaluate Multiple conditions That is( or and not )

#                           Or = at least one condition must be true
#                           End = both conditions must be true
#                           Not = inverse the condition [ not false, not true ]

EX-1: OR

temp = -5
is_raining = True

if temp>35  or temp<0 or is_raining:
    print("Event cancelled!")
else:
    print("Event still scheduled!")


#Event cancelled! #if temp is -5
#Event cancelled! #if temp is 36
#Event cancelled! #if is_raining is True
#Event still scheduled! #if temp is 5; or FalsE

EX-2: AND

temp = 28
is_Sunny = True  #Means sunny out outside

if temp >= 28 and is_Sunny:
    print("It is hot outside and also sunny ")
elif temp <= 0 and is_Sunny:
    print("It is cold outside and also sunny")
elif 20 > temp > 0 and is_Sunny:
    print("It is  warm outside and also sunny")

#outputs:
#It is  warm outside and also sunny ; if temp = 6
#It is cold outside and also sunny ; if temp =-3
#It is hot outside and also sunny ; if temp =28

EX-3: NOT
temp = 5
is_Sunny = False  #Means not sunny outside

if temp >= 28 and not is_Sunny: #not is_sunny -> i.e false means cloudy.
    print("It is hot outside and also cloudy ")
elif temp <= 0 and not is_Sunny:
    print("It is cold outside and also cloudy")
elif 20 > temp > 0 and not is_Sunny:
    print("It is  warm outside and also cloudy")
else:
    print(f"{temp} is not valid!!")
#outputs:
#It is hot outside and also cloudy ; if temp = 28 when is_Sunny = False
#It is cold outside and also cloudy ; if temp = 0 when is_Sunny = False
#It is  warm outside and also cloudy ; if temp = 5 when is_Sunny = False




#  CONDITION EXPRESSIONS = A one line shortcut for the if-else statement (ternary operator)

#                         Print or assign one of two values based on a condition
#                           X if 'condition' else y

#biology_class= "yes"
#print("Today Class is there" if biology_class == "No"  else "No class") #o/p: No class

#temp=-3
#weather="Its Cold! put on some bonfire" if temp < 0 else "Hottie Day!!"
#print(weather) #o/p:Its Cold! put on some bonfire

#a=3
#b=4
#print("a is min" if a<b else "b is max") #o/p: a is min



string methods 〰️

ph_num = input("enter ur ph num:")
#result = len(name) #O/P: enter ur name: MJR VARMA - 10
#result = name.find("A") #O/P: enter ur name:MJR VARMA - 5
#result = name.rfind("R") #O/P: enter ur name:MJR VARMA - 6
#name = name.capitalize() #O/P: enter ur name:mjr varma - Mjr varma
#name = name.upper() #O/P: enter ur name:mjr varma - MJR VARMA
#name = name.lower() #O/P: enter ur name:MJR VARMA - mjr varma
#result = name.islower() #O/P: enter ur name:MJR VARMA - False
#result = name.isdigit() #O/P: enter ur name:mjr123 - False
#result = phone_number.count("2") #O/P: enter ur ph num:1223-422-452-11 - 5
#ph_num = ph_num.replace("-"," ") #O/P: enter ur ph num:123-234-2442-1 = 123 234 2442 1
print(ph_num)


#  Validate user input exercise
# 1. username is no more than 12 characters
# 2. username Must not contain spaces
# 3. Username must not contain digits

user_name = input("Enter a User_name:")

if len(user_name) > 12:
    print("More than 12 Chracters...") #O/P: Enter a User_name:M JAYA RAKESH VARMA - More than 12 Chracters...
elif user_name.find(" ") != -1:
    print("No Spaces Please!!!") #O/P: Enter a User_name: MJR Varma - No Spaces Please!!!
elif not user_name.isalpha():
    print("No Digits Please!!!") #O/P: Enter a User_name:Rakesh123 - No Digits Please!!!
else:
    print(f"Welcome {user_name}") #O/P: Enter a User_name:MJR Varma - Welcome MJR Varma



# String Indexing✂️
                        Accesing elements of a sequence using [] (indexing operator)
                        [start : end : step]

credit_num = "1213-4213-4561-2113"

#print(credit_num[4]) # Print the digit/word/symbol at the index 4
#print(credit_num[:4]) #print the digits until index 4 (but not index 4) from index 0 - 1213
#print(credit_num[5:9]) #prints numbers from index 5 to until index 9 - 4213
#print(credit_num[5:]) #prints from index 5 to until end - 4213-4561-2113
#print(credit_num[-1]) #prints the first number from backward (reverse) - 3
#print(credit_num[::2]) #prints every second character from the string - 11-2346-13
#print(credit_num[::3]) #O/P: 132-623
#print(credit_num[2:9:2]) #prints from 2 to until 9 by step of 2 - 1-23
#last_digits = credit_num[-4:] , print(last_digits) #By using negitive indexing we print the last_digits - 2113
#credit_num = credit_num[::-1] , print(credit_num) #Reverse a string by using a negative indexing - 3112-1654-3124-3121


#  format specifiers 💬= {value:flags} format a value based on what
#                        flags are inserted

# .(number)f = round to that many decimal places (fixed point)
# :(number) = allocate that many spaces
# :03 = allocate and zero pad that many spaces
# :< = left justify
# :> = right justify
# :^ = center align
# :+ = use a plus sign to indicate positive value
# := = place sign to leftmost position
# :  = insert a space before positive numbers
# :, = comma separator


mrp_1 = 1000.3343
mrp_2 = -112.45
mrp_3 = 12424.55

#print(f"MRP 1 is {mrp_1:.2f}")
#Here :.2f round to that many decimal places (fixed point)...  we can customize accordingly whrer stock prices need to precise we keep :.6f i.e; it gives 6 decimal floating_points after point...
#print(f"MRP 2 is {mrp_2:.2f}")
#print(f"MRP 3 is {mrp_3:.2f}")
# O/P: MRP 1 is 10.33 , MRP 2 is -112.45 , MRP 3 is 14.55


#print(f"MRP 1 is {mrp_1:10}") # :(number) = allocate that many spaces
#print(f"MRP 2 is {mrp_2:10}")
#print(f"MRP 3 is {mrp_3:10}")
#O/P :
#MRP 1 is    10.3343
#MRP 2 is    -112.45
#MRP 3 is      14.55


# :010 = allocate and zero pad that many spaces
#print(f"MRP 1 is {mrp_1:010}")
#print(f"MRP 2 is {mrp_2:010}")
#print(f"MRP 3 is {mrp_3:010}")
#O/P :
#MRP 1 is    10.3343
#MRP 2 is    -112.45
#MRP 3 is      14.55


# :< = left justify
# :> = right justify
# :^ = center align
#print(f"MRP 1 is {mrp_1:<10}")
#print(f"MRP 2 is {mrp_2:>10}")
#print(f"MRP 3 is {mrp_3:^10}")
#MRP 1 is 10.3343
#MRP 2 is    -112.45
#MRP 3 is   14.55


# :+ = use a plus sign to indicate positive value
# :  = insert a space before positive numbers
#print(f"MRP 1 is {mrp_1:+}")
#print(f"MRP 2 is {mrp_2:+}")
#print(f"MRP 3 is {mrp_3: }")
#O/P:
#MRP 1 is +10.3343
#MRP 2 is -112.45
#MRP 3 is  14.55


# :, = comma separator
#print(f"MRP 1 is {mrp_1:,}")
#print(f"MRP 2 is {mrp_2:,}")
#print(f"MRP 3 is {mrp_3:,}")
#O/P:
#MRP 1 is 1,000.3343
#MRP 2 is -112.45
#MRP 3 is 12,424.55


# := = place sign to leftmost position
#print(f"MRP 1 is {mrp_1:=}")
#print(f"MRP 2 is {mrp_2:=}")
#print(f"MRP 3 is {mrp_3:=}")
#O/P:
#MRP 1 is 1000.3343
#MRP 2 is -112.45
#MRP 3 is 12424.55



while loops ♾️ -
                    Execute some code WHILE some condition remains true

#EX:1
name = input("enter ur name:")
while name == "":
    print("Plzzz enter ur name!!!!")
    name = input("Uff... enter ur name properly:")     #This line is a chance to escaspe...
                                                        If u give "Plzzz enter ur name!!!!" and
                                                        leaves it.. then it falls into infite loop
print(f"Hello {name}")
#O/P:
#enter ur name:
#Plzzz enter ur name!!!!
#Uff... enter ur name properly: Rakesh
#Hello  Rakesh


#EX:2
age = int(input("enter ur age:"))
while age < 0:
    print("Age must be Positive Number!!")
    age = int(input("Enter ur age:"))
print(f"You are {age} year/s old")
#O/P:
#enter ur age:-3
#Age must be Positive Number!!
#Enter ur age:6
#You are 6 year/s old


#EX:3 (with logical operators this tymm ( not / ! )...)
food = input("enter food u like (q to quit!): ")
while food != "q":
    print(f"You like {food}")
    food = input("Enter another food u like (q to quit):")
print("bye")
#O/P:
#enter food u like (q to quit!): Biryani
#You like Biryani
#Enter another food u like (q to quit):Apollo Fish
#You like Apollo Fish
#Enter another food u like (q to quit):q
#bye


#EX:4
while True:
    num = int(input("Enter a number between 1 - 10: "))

    if num < 1 or num > 10:
        print(f"{num} is not valid!! Please try again.\n")
    else:
        if num == 7:
            print("Thala For a Reason")
        print(f"{num} lies between 1 - 10")
        break  # exit loop when valid input is received

#Enter a number between 1 - 10: 12
#12 is not valid!! Please try again.
#Enter a number between 1 - 10: 2
#2 lies between 1 - 10
#Enter a number between 1 - 10: 7
#Thala For a Reason
#7 lies between 1 - 10


⭐ Python compound interest calculator 💵

principle = 0
rate = 0
time = 0
while principle <= 0:
    principle = float(input("Enter the principle amount:"))
    if principle <=0:
        print("It cant be zero!")
while rate <= 0:
    rate = float(input("Enter the Intrest rate:"))
    if rate <=0:
        print("It cant be zero!")
while time <= 0:
    time = float(input("Enter the No of Years:"))
    if time <=0:
        print("It cant be zero!")
total = principle * pow((1 + rate / 100), time)
print(f"Balance amount was: Rs {total:.2f}")

#O/P:
Enter the principle amount:2000
Enter the Intrest rate:10
Enter the No of Years:2
Balance amount was: Rs 2420.00











