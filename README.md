# Python
Programming in Python
Write python program to print first letter of your name 
a) Example: Peter
               *      *
               *             *
               *              *
               *      *
               *
               *
               *
b) Print your name by using for loop

c) check the user name is palindrome or not
str="K";    
j = 5;    
i = 0;  
for Row in range(0,7):    
    for Col in range(0,7):     
        if (Col == 1 or ((Row == Col + 1) and Col != 0)):  
            str=str+"*"    
        elif (Row == i and Col == j):  
              str=str+"*"    
              i=i+1  
              j=j-1  
        else:      
            str=str+" "    
    str=str+"\n"    
print(str);  
#Define a function 
def isPalindrome(string): 
    if (string == string[::-1]) : 
        return "The string is a palindrome." 
    else: 
        return "The string is not a palindrome." 
 
#Enter input string 
string = input ("Enter string: ") 
 
print(isPalindrome(string))
