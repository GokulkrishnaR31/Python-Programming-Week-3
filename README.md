# Python-Programming-Week-3
Admission Eligibility

Write a program to find the eligibility of admission for a professional course based on the following criteria:

Marks in Maths >= 65

Marks in Physics >= 55

Marks in Chemistry >= 50

Or

Total in all three subjects >= 180

CODE:

m=int(input())

p=int(input())

c=int(input())

t=m+p+c

if m >= 65 and p>=55 and c>=50 or t>=180: 

    print("The candidate is eligible")

else:

    print("The candidate is not eligible")
#Classifying Triangles

A triangle can be classified based on the lengths of its sides as equilateral, isosceles or scalene. All three sides of an equilateral triangle have the same length. An isosceles triangle has two sides that are the same length, and a third side that is a different length. If all of the sides have different lengths then the triangle is scalene.

Write a program that reads the lengths of the three sides of a triangle from the user. Then display a message that states the triangle’s type.

CODE:

a=int(input())

b=int(input())

c=int(input())

if(a==b==c):

    print("That's a equilateral triangle")

elif(a==b or b==c or a==c):

    print("That's a isosceles triangle")

else:

    print("That's a scalene triangle")
    #Electricity Bill

Write a program to calculate and print the Electricity bill where the unit consumed by the user is given from test case. It prints the total amount the customer has to pay. The charge are as follows: 

Unit                                                     Charge / Unit

Upto 199                                             @1.20

200 and above but less than 400        @1.50

400 and above but less than 600        @1.80

600 and above                                    @2.00

If bill exceeds Rs.400 then a surcharge of 15% will be charged and the minimum bill should be of Rs.100/- 



CODE:

n=float(input())



if n<=199:

    a=n*1.20

elif n>=200 and n<400:

    a=n*1.50

elif n>=400 and n<600:

    a=n*1.80

elif n>=600:

    a=n*2.00

   

if (a<100):

    a=100

elif a>400:

    a=a+(0.15*a)

print("%.2f"%a)
#IN/OUT

Ms. Sita, the faculty handling programming lab for you is very strict. Your seniors have told you that she will not allow you to enter the week's lab if you have not completed atleast half the number of problems given last week. Many of you didn't understand this statement and so they requested the good programmers from your batch to write a program to find whether a student will be allowed into a week's lab given the number of problems given last week and the number of problems solved by the student in that week.

 

CODE:

n1=int(input())

n2=int(input())

if(n1/2>=n2):

    print("OUT")

else:

    print("IN")
    #Vowel or Consonant

In this exercise you will create a program that reads a letter of the alphabet from the user. If the user enters a, e, i, o or u then your program should display a message indicating that the entered letter is a vowel. If the user enters 'y' then your program should display a message indicating that sometimes y is a vowel, and sometimes y is a consonant. Otherwise your program should display a message indicating that the letter is a consonant.

CODE:

v=input()

if(v=='a' or v=='e' or v=='i' or v=='o' or v=='u'):

    print("It's a vowel.")

elif(v=='y'):

    print("Sometimes it's a vowel... Sometimes it's a consonant.")

else:

    print("It's a consonant.")

#Leap Year

Most years have 365 days. However, the time required for the Earth to orbit the Sun is actually slightly more than that. As a result, an extra day, February 29, is included in some years to correct for this difference. Such years are referred to as leap years. The rules for determining whether or not a year is a leap year follow:

• Any year that is divisible by 400 is a leap year.

• Of the remaining years, any year that is divisible by 100 is not a leap year.

• Of the remaining years, any year that is divisible by 4 is a leap year.

• All other years are not leap years.

Write a program that reads a year from the user and displays a message indicating whether or not it is a leap year.

CODE:

year = int(input())



if year % 400 == 0:

    print(f"{year} is a leap year.")

elif year % 100 == 0:

    print(f"{year} is not a leap year.")

elif year % 4 == 0:

    print(f"{year} is a leap year.")

else:

    print(f"{year} is not a leap year.")

#Month name to days

The length of a month varies from 28 to 31 days. In this exercise you will create a program that reads the name of a month from the user as a string. Then your program should display the number of days in that month. Display “28 or 29 days” for February so that leap years are addressed.





CODE:

m=input()

if (m=="February"):

    print("February has 28 or 29 days in it.")

elif(m=="January" or m=="March" or m=="May" or m=="July" or m=="August" or m=="October" or m=="December"):

    print(m,"has 31 days in it.")

else:

    print(m,"has 30 days in it.")

#Pythagorean triple

Three numbers form a Pythagorean triple if the sum of squares of two numbers is equal to the square of the third.

For example, 3, 5 and 4 form a Pythagorean triple, since 3*3 + 4*4 = 25 = 5*5 

You are given three integers, a, b, and c. They need not be given in increasing order. If they form a Pythagorean triple, then print "Yes", otherwise, print "No". 

CODE:

a=int(input())

b=int(input())

c=int(input())

if(a==b==c):

    print("That's a equilateral triangle")

elif(a==b or b==c or a==c):

    print("That's a isosceles triangle")

else:

    print("That's a scalene triangle")
    #Second last digit

Write a program that returns the second last digit of the given number. Second last digit is being referred 10the digit in the tens place in the given number.

For example, if the given number is 197, the second last digit is 9.

Note1 - The second last digit should be returned as a positive number. i.e. if the given number is -197, the second last digit is 9.

Note2 - If the given number is a single digit number, then the second last digit does not exist. In such cases, the program should return -1. i.e. if the given number is 5, the second last digit should be returned as -1.





CODE:

n=abs(int(input()))

a=str(n)

if(n>=10):

    print(a[-2:-1])

else:

    print("-1")
    #Chinese Zodiac

The Chinese zodiac assigns animals to years in a 12 year cycle. One 12 year cycle is shown in the table below. The pattern repeats from there, with 2012 being another year of the dragon, and 1999 being another year of the hare.

Year Animal

2000 Dragon

2001 Snake

2002 Horse

2003 Sheep

2004 Monkey

2005 Rooster

2006 Dog

2007 Pig

2008 Rat

2009 Ox

2010 Tiger

2011 Hare

Write a program that reads a year from the user and displays the animal associated with that year. Your program should work correctly for any year greater than or equal to zero, not just the ones listed in the table.
CODE:

y=int(input())

if y%12==0:

    print(y,"is the year of the Monkey.")

elif y%12==1:

    print(y,"is the year of the Rooster.")

elif y%12==2:

    print(y,"is the year of the Dog.")

elif y%12==3:

    print(y,"is the year of the Pig.")

elif y%12==4:

    print(y,"is the year of the Rat.")

elif y%12==5:

    print(y,"is the year of the Ox.")

elif y%12==6:

    print(y,"is the year of the Tiger.")

elif y%12==7:

    print(y,"is the year of the Hare.")

elif y%12==8:

    print(y,"is the year of the Dragon.")

elif y%12==9:

    print(y,"is the year of the Snake.")

elif y%12==10:

    print(y,"is the year of the Horse.")

elif y%12==11:

    print(y,"is the year of the Sheep.")
