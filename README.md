# 19CS301-Module7
EX: 7.1 RECURSION
### Aim: 
To Write a Python program to find the sum of square of a first n Natural Numbers using recursion

### Algorithm:
STEP 1: Start.

STEP 2: Define a function.

STEP 3: return for termination of the function. 

STEP 4: Create a recursive case to calculate the result.

STEP 5: Print the result. STEP 6: Stop.

### Program:
```
def sum_of_numbers(n):
    if(n<=0):
        return 0
    return(n**2 + sum_of_numbers(n-1))
n = int(input())
print('Result is',sum_of_numbers(n))
```
### Output:
![image](https://github.com/23013357/19CS301-Module7/blob/main/vv.png)

### Result: Thus, the given program is implemented and executed successfully .
 

EX: 7.2 TYPES OF RECURSIONS
### Aim:
To Write aPython program to display Arithmetic Progression  series by reading the difference between the numbers and limit  using  head recursion.


### Algorithm:
STEP 1: Start.

STEP 2: Define a function.

STEP 3: Create a recursive case in the first line of function for head recursion.

STEP 4: Print the result.

STEP 5: Stop.
### Program:
```
def fun(n,d):
    if (n > 0):
        fun(n-d,d)
        print(n, end=" ")
 
d= int(input())
n = int(input())
fun(n,d)

```
### Output:
![image](https://github.com/23013357/19CS301-Module7/blob/main/bb.png)

###Result: Thus, the given program is implemented and executed successfully.
 


EX: 7.3 TAYLOR SERIES

### Aim: 
To python program to evaluate the series using recursion by collecting the x and n values from the user.
### ALGORITHM:
STEP 1: Start.

STEP 2: Create a variable x and n.

STEP 3: Get the values of x and n from user.

STEP 4: Create a base case and recursive case to calculate the result.

STEP 5: Print the result.

STEP 6: Stop.
### Program:
```
def series(x,n):
         if n==0:
            return 1
         else:
            return x**n/n+series(x,n-1)
x = int(input())
n = int(input())
print(series(x,n))
```
### Output:
![image](https://github.com/user-attachments/assets/1d00b1a4-cecb-466f-8593-805f00d27461)

 
### Result: Thus, the given program is implemented and executed successfully .
 

EX: 7.4 Solve by recursion relation

### Aim: 
To Write a Python Program to find whether a string is a palindrome or not using recursion

### Algorithm:
STEP 1: Start.

STEP 2: Define a function.

STEP 3: Create a base case and recursive case to calculate the result.

STEP 4: Create a variable and get input from user.

STEP 5 : Call the function.

STEP 6: Print the result.

STEP 7: Stop.

### Program:
```
def is_palindrome(word):
      if len(word)<1:
            return True
      else:
            if word[0]==word[-1]:
                 return is_palindrome(word[1:-1])
             else:
                  return False
word = str(input())
if is_palindrome(word)==True:
        print("String is a palindrome")
else:
        print("String is not a palindrome")
```
### Output:
![image](https://github.com/user-attachments/assets/d30ef836-1901-448a-a146-dc905fdc3198)

### Result: Thus, the given program is implemented and executed successfully .


 EX: 7.5   Tail recursion

### Aim: 
To Write a Python Program to convert a decimal number to a binary number using tail recursion.


### Algorithm:

Start

Input: Take a decimal number n as input.

Base Case: If n == 0, return 0 (base case of the recursion).

Recursive Step: If n != 0, calculate the binary digit as n % 2 (remainder when divided by 2).

Recursion: Call the decimal_binary() function recursively with n // 2 (integer division by 2).

Combine Result: Append the binary digit to the result of the recursive call using 10 * result (shifting the binary digits left).

Output: Return the final binary representation of the number.

End

### Program:
```
def decimal_binary(n):
    if n==0:
        return 0
    else:
        return (n% 2)+10*decimal_binary(int(n/2))
n=int(input())
print(decimal_binary(n))
```
### Output:
![image](https://github.com/23013357/19CS301-Module7/blob/main/MODUL%207.png)

### Result: Thus, the given program is implemented and executed successfully .
 

