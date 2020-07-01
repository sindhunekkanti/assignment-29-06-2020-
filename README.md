# assignment(29-06-2020)
#1 open a file in python using try and except
try:
    f = open("xyz.txt", "r")
except IOError:    
    print("No file by that name")

#2 split data in a file
h=open('xyz.txt','r')
content=h.readlines()
print(content.split())

#3 read the contents of a file using with statement
with open("C:\\...\\...\\...\\record-13.txt") as f:
    content=f.readlines()
    print(content) 

#4 remove file and directory
import os
file_path = '/tmp/file.txt'
try:
    os.remove(file_path)
except OSError as e:
    print("Error: %s : %s" % (file_path, e.strerror))

#5 create list and access elements in list
l=[10,20,30,40,50,60,70,80,90] 
a=l[1]
b=l[2]
c=l[4]
print(a,b,c)
