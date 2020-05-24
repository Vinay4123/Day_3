# Day_3
#Q1You are given with a list of integer elements. Make a new list which will
store square of elements of previous list.

a=[1,2,3,4,5,6,7,8,9,0]

print ([i**2 for i in a])

#Q2 From a list containing ints, strings and floats, make three lists to store
them separately.

w=[2, 3.0,4.3,"hello world", 5, 4.3]

x=[]

y=[]

z=[]

for i in w:

    if type(i)==int:
    
        x.append(i)
        
    elif type(i)==float:
    
        y.append(i)
        
    elif type(i)==str:
    
        z.append(i)
        
print(x)

print(y)

print(z)

#Q3 Print the pattern
1
1 2
1 2 3
1 2 3 4
1 2 3 4 5


n=int(input('enter the number of rows'))

for i in range(1,n+1):

  for j in range(1,i+1):
  
    print(j,end='')
    
  print()
  
#Q4 Accept data in two 3*3 matrix and calculate the sum of the matrices.


# Program to add two matrices using nested loop 

X = [[1,2,3], 

	[4 ,5,6], 
  
	[7 ,8,9]] 

Y = [[9,8,7], 

	[6,5,4], 
  
	[3,2,1]] 


result = [[0,0,0], 

		[0,0,0], 
    
		[0,0,0]] 

# iterate through rows 

for i in range(len(X)):

  for j in range(len(X[0])):
  
    result[i][j] = X[i][j] + Y[i][j]
    

for r in result: 

	print(r) 

#Q5 Write a Python program to check whether a given number is a
narcissistic number or not
For example, 371 is a narcissistic number; it has three digits, and if we
cube each digits 3 3  + 7 3  + 1 3  the sum is 371. Other 3-digit narcissistic
numbers are
153 = 1 3  + 5 3  + 3 3
370 = 3 3  + 7 3  + 0 3
407 = 4 3  + 0 3  + 7 3 .
There are also 4-digit narcissistic numbers, some of which are 1634,
8208, 9474 since
1634 = 1 4 +6 4 +3 4 +4 4
8208 = 8 4 +2 4 +0 4 +8 4
9474 = 9 4 +4 4 +7 4 +4 4

n=input('Enter a number')

m=int(n)

s=0

q=m

while(m!=0):

    p=m%10
    
    s+=p**(len(n))
    
    m=m//10
    
if(s==q):

    print('Yes')
    
else:

    print('No')












