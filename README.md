# labcodes

Calculator
a=int(input('enter 1st number'))
b=int(input('enter 2nd number'))
c=a+b
d=a-b
e=a*b
f=a/b
g=a%b
h=a//b
i=a**b
print('sum =',c)
print('difference =',d)
print('multiplication =',e)
print('division =',f)
print('modulous =',g)
print('floor division =',h)
print('exponent =',i)
----------------------------------------------------------------------------------------------------------------------------------------------------------------------
Distance measurer
km = float (input("Enter the distance between two cities in kilometers: "))
mtr = km * 1000
cent = km * 100000
inch = km * 2.54 * 100000
ft = km * 30.28 * 1000
print("Distance between two cities in meters is:%f ",mtr)
print("Distance between two cities in centimeters is:%f ",cent)
print("Distance between two cities in inches is:%f ",inch)
print("Distance between two cities in feet is:%f ",ft)
----------------------------------------------------------------------------------------------------------------------------------------------------------------------
Number conversion
n1= input('Enter a Binary number:')
n2= input('Enter a octal number:')
n3= input('Enter a hexadecimal number:')
d1= int(n1, 2)
d2= int(n2, 8)
d3= int(n3, 16)
print('The decimal conversion is:', d1)
print(type(d1))
print('The decimal conversion is:', d2)
print(type(d2))
print('The decimal conversion is:', d3)
print(type(d3))
----------------------------------------------------------------------------------------------------------------------------------------------------------------------
Even odd
a=int(input('enter a number'))
if(a%2==0):
 print('%i is even',a)
else:
 print('%i is odd',a)
----------------------------------------------------------------------------------------------------------------------------------------------------------------------
Sum of list
a=int(input('enter 1st number'))
b=int(input('enter 2nd number'))
c=int(input('enter 3rd number'))
d=int(input('enter 4th number'))
list=[a,b,c,d]
sum=0
for i in list:
 sum=sum+i
print('sum of numbers is',sum)
----------------------------------------------------------------------------------------------------------------------------------------------------------------------
Print pattern

for i in range(1,6):
 for j in range(1,i+1):
  print('*',end=' ')
 print()

----------------------------------------------------------------------------------------------------------------------------------------------------------------------
Rock paper scissor

import random
user1=input("enter a choice(rock,paper,scissors):")
list=["rock","paper","scissors"]
Computer=random.choice(list)
print("user1 value",user1)
print("user2 value",Computer)
if user1==Computer:
    print("its a tie")
elif user1=="rock":
    if Computer=="paper":
        print("computer wins")
    else:
            print("user1 wins")
elif user1=="paper":
    if Computer=="scissors":
        print("computer wins")
    else:
            print("user1 wins")
elif user1=="scissors":
    if Computer=="rock":
        print("computer wins")
    else:
            print("user1 wins")



----------------------------------------------------------------------------------------------------------------------------------------------------------------------


 Sort a listing using bubble sort

X=[ ]
n=int(input("enter the length of list"))
for i in range (n):
    print("enter the element")
    X.append(int(input()))
    print(X[0:n])
for j in range (n-1):
    for i in range ((n-1)-j):
        if(X[i]>X[i+1]):
            temp=X[i]
            X[i]=X[i+1]
            X[i+1]=temp
print(X[0:n])
----------------------------------------------------------------------------------------------------------------------------------------------------------------------
List and tupple operations

# empty list
My_list = []
# list of integers
My_list=[1, 2, 3]
# list with mixed data types
My_list = [1, "Hello", 3.4]
print(My_list)
# nested list
My_list = ["mouse", [8, 4, 6], ['a']]
My_list = ['p', 'r', 'o', 'b', 'e']
print(My_list[0])
print(My_list[2])
print(My_list[4])
# Nested List
N_list = ["Happy", [2, 0, 1, 5]]
# Nested indexing
print(N_list[0][0])
print(N_list[1][2])
#negative indexing
My_list = ['p','r','o','b','e']
print(My_list[-1])#negative indexing
print(My_list[-5])
# List slicing in Python
My_list = ['p','r','o','g','r','a','m','i','z']
# elements 3rd to 5th
print(My_list[2:5])
# elements beginning to 4th
print(My_list[:-5])
# elements 6th to end
print(My_list[5:])
# elements beginning to end
print(My_list[:])
# add or update the element in list
Odd = [2, 4, 6, 8]
# change the 1st item
Odd[0] = 1
print(Odd)
# change 2nd to 4th items
Odd[1:4] = [3, 5, 7]
print(Odd)
# Appending and Extending lists in Python
Odd = [1, 3, 5]
Odd.append(7)
print(Odd)
Odd.extend([9, 11, 13])
print(Odd)
# Concatenating and repeating lists
Odd = [1, 3, 5]
print(Odd + [9, 7, 5])#Concatenating lists
print(Odd * 3)# repeating lists
# Demonstration of list insert() method
Odd = [1, 9]
Odd.insert(1,3)
print(Odd)
Odd[2:2] = [5, 7]
print(Odd)
# deleting list items
My_list = ['p', 'r', 'o', 'b', 'l', 'e', 'm']
del My_list[2]# delete one item
print(My_list)
del My_list[1:5]# delete multiple items
print(My_list)
del My_list# delete entire list
#print(My_list)# Error: List not defined
#Remove list
My_list = ['p','r','o','b','l','e','m']
My_list.remove('p')
# Output: [‘r’, ‘o’, ‘b’, ‘l’, ‘e’, ‘m’]
print(My_list)
# Output: ‘o’
print(My_list.pop(1))
# Output: [‘r’, ‘b’, ‘l’, ‘e’, ‘m’]
print(My_list)
# Output: ‘m’
print(My_list.pop())
# Output: [‘r’, ‘b’, ‘l’, ‘e’]
print(My_list)
My_list.clear()
# Output: []
print(My_list)
# Python list methods
My_list = [3, 8, 1, 6, 0, 8, 4]
print(My_list.index(8)) # Using index method
print(My_list.count(8))# Count method
My_list.sort() #sort method
print(My_list)
My_list.reverse()#reverse method
print(My_list)
----------------------------------------------------------------------------------------------------------------------------------------------------------------------
  Set dictionary and string operations 
 print("----------Set----------")
S1={1,2,3,4,5,6}
S2={1,2,3}
print("Original set", S1)
S1.add(8)
print("Add 8 in set", S1)
S1.remove(8)
print("Remove 8 in set", S1)
S1.pop()
print("Pop element default 1st element in set", S1)
print("Length set", len(S1))
S1.update([8,9])
print("updated 8,9 in set",S1)
S1.discard(3)
print("discard 3",S1)
S1={1,2,3,4,5,6}
S2={1,2,3,9}
print("Reinitialize S1 ::",S1)
print("initialize S2 ::",S2)
print("S2 subset of S1 ::",S2.issubset(S1))
print("S2 superset of S1 ::",S2.issuperset(S1))
print("S1 Union S2 ::",S1.union(S2))
print("S1 Intersection S2 ::",S1.intersection(S2))
print("S1 diffrence S2 ::",S1-S2)
print("S1 Symmetric diffrence S2 ::",S1^S2)
S3=S2.copy()
print("Copy S3 as S2",S3)
print("Length of S3::",len(S3))
print("Min of S3::",min(S3))
print("Max of S3::",max(S3))
print("Sum of S3::",sum(S3))
print("Sorted of S3::",sorted(S3))
print("-----------Dictionary---------------")
A={"Name":"Abcdef","age":18,"address":"kalyan"}
print("Dictionary A",A)
print("Keys of Dictionary A",A.keys())
print("Values of Dictionary A",A.values())
print("Items of Dictionary A",A.items())
print("Length of A",len(A))
print("A[name]", A['Name'])
print("Get age ", A.get('age'))
A['tel']=322233
print("Adding tel",A)
C=A.clear()
print("Clearing A :",A)
A={'name':'bj','age':23,'contact':666555,'gender':'male'}
B={'name':'bj','age':23,'contact':666555,'ge':'male',"rank":1}
A.update(B)
print("Updating A with B : ",A)
My_dict = {'name':'Jack', 'age': 26}
print("New dictionary :: ",My_dict)
My_dict['age'] = 27
#Output: {'age': 27, 'name': 'Jack'}
print("Change age 26 to 27 :: ",My_dict)
# add item
My_dict['address'] = ['Downtown']
# Output: {'address': 'Downtown', 'age': 27, 'name': 'Jack'}
print("Add new address field :: ",My_dict)
print("-----------String--------------")
str="Welcome to python"
print("String:",str)
print("Extract letter",str[2])
print("Extract last character ",str[-1])
print("Return range of charater",str[3:7])
print("Return all characters from indes 5",str[5:])
print("Return all characters before index 6",str[:6])
print("Replace python with java",str.replace('python','java'))
print("In operator Checkin",'Wel'in str)
print("Not in Operator checking",'N' not in str)
print("To capitalize first charater",str.capitalize())
print("To convert all string to lowercase",str.lower())
print("To convert all string to uppercase",str.upper())
str1='o'
print("To count the occurence of letter o in str",str.count(str1))
print("To return the substring using split()",str.split())
print("To return the substring using split() till some limit",str.split(' ',1))
seq=('ab','bc','cd')
print("The string obtained by using join()",str.join(seq))
print("Length of String",len(str))
----------------------------------------------------------------------------------------------------------------------------------------------------------------------
 1d and multidimensional
  import array as arr
a=arr.array('i',[1,2,3]) # creating an array with integer type
print("The new created array is :",end=" ") #printing original array
for i in range(0,3):
    print(a[i],end=" ")
print()

b=arr.array('d',[2.5,3.2,3.3])# creating an array with float type
print("The new created array is :",end=" ") #printing original array
for i in range(0,3):
    print(b[i],end=" ")
print()

a.insert(1,4) #inserting array using insert() function
print("Arra after insertion:",end=" ")
for i in (a):
    print(i,end=" ")
print()

b.append(4.4)#adding an element using append()
print("Array after insertion:",end=" ")
for i in (b):
    print(i,end=" ")
print()

print("Accessing int element:",a[0])#accessing element of array
print("Accessing float element:",b[2])

print("The popped element is:",end=" ")#using pop() to remove element at 2nd position
print(a.pop(3))
print("The array after popping is:",end=" ")
for i in range (0,3):
    print(a[i],end=" ")
    
a.remove(1)#using remove() to remove 1st occurence of 1
print("The array after removing is:",end=" ")
for i in range (0,2):
    print(a[i],end=" ")

c=arr.array('i',[1,2,34,7]) #using index of 1st occurrence of element of 34
print("the index of 1st occurrence of 2 is:",end=" ")
print(c.index(34))

c[2]=78 #updating a element in a array
print("Array after updation:",end=" ")
for i in range (0,4):
    print(c[i],end=" ")
----------------------------------------------------------------------------------------------------------------------------------------------------------------------
 Factorial of no
  
def factorial(n):
 if n == 0:
     return 1
 else:
    return n * factorial(n-1)
n=int(input("enter a number "))
print('factorial of',n,'is')
print(factorial(n))
----------------------------------------------------------------------------------------------------------------------------------------------------------------------
 Square of no
def square(list):
 ret = []
 for i in list:
     ret.append(i ** 2)
 return ret
x=[12,23,9,13,8,7]
print(x)
print(square(x))
----------------------------------------------------------------------------------------------------------------------------------------------------------------------
File handling
 import pickle
print ("***WRITE file*****")
f=open('myfile.txt','w') #Create file if not exist and open it for writting
s1=input('Enter Your Text to be written in to file: ')
f.write(s1) #write text into file
f.close() #Close file
print("")
print ("***Read file *****")
f1=open('myfile.txt','r') #open file for reading
print ("Contents of file are")
s=f1.read()
print (s)
f1.close()#Close file
print("")
print ("***Append file*****")
f=open('myfile.txt','a') #open file for Appending
s2=input('Enter text to be appended in original file..')
f.write(s2)
f.close() #Close file
print("")
print ("")
print ("***Read Appended file*****")
f1=open('myfile.txt','r') #Create file if not exist and open it for reading
s=f1.read()
print (s)
f.close()
print ("***WITH OPEN*****")
with open('sample.txt','w') as f:
    s3=input('Enter text for WITHOPEN write..')
    f.write(s3)
with open('sample.txt','r') as f:
    for line in f:
        print (line)

----------------------------------------------------------------------------------------------------------------------------------------------------------------------

Classes object and method class person
from datetime import date
today=date.today()
class person:
    def __init__(self,name):
     self.name=name
    def age(self):
        birth_year=int(input('enter your year of birth :'))
        age=today.year-birth_year
        return age
x=person(input('enter your name :'))
data=x.age()
print('your age is :',data)
----------------------------------------------------------------------------------------------------------------------------------------------------------------------
Toyota .csv  maplotlib and seaborn
import numpy as np
import matplotlib.pyplot as plt  
cars_data=pd.read_csv('Toyota.csv',index_col=0,na_values=["??","???"])
print(cars_data)
plt.scatter(cars_data['Age'],cars_data['Price'], c='red')
plt.title("price vs Age")
plt.xlabel("age")
plt.ylabel('price')
plt.show 
plt.hist(cars_data['KM'])
plt.hist(cars_data['KM'],color='green',edgecolor='white',bins=5)
plt.title("Histogram of kilometer")
plt.xlabel("kilometer")
plt.ylabel('frequecny')
plt.show
import seaborn as sns 
sns.set(style='darkgrid')
sns.regplot(x=cars_data['Age'],y=cars_data['Price'])
sns.set(style='darkgrid')
sns.regplot(x=cars_data['Age'],y=cars_data['Price'],fit_reg=False)





----------------------------------------------------------------------------------------------------------------------------------------------------------------------

 Hotel.csv 
   import pandas as pd
data_hotel=pd.read_csv('hotel_bookings.csv')
print(data_hotel.head(10))
print(data_hotel.tail(10))
arrival=data_hotel.loc[:,['arrival_date_month']]
print(arrival)
data_hotel.describe()
main=data_hotel.query('is_canceled==0')
print(main)
main.query('arrival_date_year==2017')
data_hotel=pd.read_csv('hotel_bookings.csv',index_col=0)
print(data_hotel)
print(data_hotel.info)
data_hotel=pd.read_csv('hotel_bookings.csv',index_col=0,na_values=["??","???"])
print(data_hotel)
print(data_hotel.head(10))
data_hotel.isnull().sum()
data_hotel['agent'].mean()
data_hotel['agent'].fillna(data_hotel['agent'].mean(),inplace=True)
print(data_hotel.isnull().sum())
print(data_hotel.head(10))
----------------------------------------------------------------------------------------------------------------------------------------------------------------------
Convert image binary and gray scale
      import matplotlib.pyplot as plt
import numpy as np
import cv2
img_path='/content/pizza.jpg'
img = cv2.imread(img_path)
print(img)
for i,col in enumerate(color):
  hist = cv2.calcHist([img],[i],None,[256],[0,256])
  plt.plot(hist,color = col)
  plt.xlim([0,256])
plt.show
img = cv2.imread(img_path)
plt.hist(img.ravel(),256,[0,256])
plt.show()
print(img.shape)
print("Rows of Pixels: %d Rows"%(img.shape[0]))
print("Columns of Pixels: %d Columns"%(img.shape[1]))
print("Color Channels: %d Color Channels"%(img.shape[2]))
plt.title('Input image')
plt.imshow(img)
plt.subplot(2,1,1)
plt.imshow(img)
plt.subplot(2,1,1)
plt.imshow(img)
plt.subplot(2,1,2)
R, G, B = img[:,:,0], img[:,:,1], img[:,:,2]
imgGray = 0.2989 * R + 0.5870 * G + 0.1140 * B
plt.imshow(imgGray, cmap='gray')
plt.show()
----------------------------------------------------------------------------------------------------------------------------------------------------------------------
 GUI
 ##from tkinter import *
##window=Tk()
### add widgets here
##window.title('Hello Python')
##window.geometry("400x200")
##window.minsize(100,100)
##window.maxsize(500,700)
##class1=Label(text="The class is good")
##class1.pack()
##window.mainloop()

from tkinter import *
root=Tk()  # create root window
c= Canvas(root,bg='blue',height=700,width=1200, cursor='pencil')
#id=c.create_line(50,50,200,50,200,150,50,150,width=4,fill="white")    # create line in the canvas joining points (50,50)(c=200,r=50)(200,150)
c.pack()   # add canvas to the root window

root.mainloop()



