# 19CS301-Module-4
ExNo.4a DICTIONARY- MERGE THE DICTIONARY
### AIM
To write a python program to merge the two python dictionaries into one
### ALGORITHM

Step 1: Start the program.

Step 2: Define the first dictionary dict1 with some key-value pairs.

Step 3: Define the second dictionary dict2 with additional key-value pairs.

Step 4: Use dictionary unpacking ({**dict1, **dict2}) to merge both dictionaries:

Step 5: All key-value pairs from dict1 are included.

Step 6: If a key appears in both dictionaries (like 'Thirty'), the value from dict2 will overwrite the one from dict1.

Step 7: Print the resulting merged dictionary.

Step 8: End the program.

### PROGRAM
```
dict1 = {'Ten': 10, 'Twenty': 20, 'Thirty': 30}
dict2 = {'Thirty': 30, 'Fourty': 40, 'Fifty': 50}
print({**dict1,**dict2})
```
### OUTPUT
![Screenshot 2025-06-02 113211](https://github.com/user-attachments/assets/8b0cb404-7e4d-4239-9d01-2aa4dae65eb7)


 
### RESULT
Thus the python program for to merge the two python dictionaries into one was implemented and executed successfully.

Exp.No:4(b)	EXCEPTION- EXCEPTION HANDLING
### AIM
To create a python program for the solution of value error in exception handling and check whether the number is even or odd.
### ALGORITHM

Step 1: Start the program.

Step 2: Input a value from the user and convert it to an integer, store in variable x.

Step 3: If x % 2 == 0, print "You entered even number."

Step 4: Otherwise, print "An odd number".

Step 5: If a ValueError occurs (e.g., user enters text or a non-integer), catch the exception and:

Step 6: Print "Enter only Number."

Step 7: End the program.
### PROGRAM
```
try:
    x=int(input())
    print("You entered even number.") if x%2==0 else print("An odd number")
except ValueError:
    print("Enter only Number.")
```
### OUTPUT
 ![Screenshot 2025-06-02 113324](https://github.com/user-attachments/assets/ec4429fc-a7ad-4396-99ab-c60d0a3bf5e9)


### RESULT
Thus the python program for handling exceptions was implemented and executed successfully.

EXNo.4C File Handling -Count the frequency of each character in a File
### AIM
To write a Python program to read a file and count the frequency of each character in it.
### ALGORITHM

Step 1:	 Begin the program.

Step 2:	 Define the function create file  andAccept two arguments: file_path (the path to the file) and content (the string content to be written into the file).

Step 3:	 Open the file specified by file_path in write mode ('w'), Write the provided content to the file.

Step 4:	Close the file (this is done automatically when exiting the with block).

Step 5:	 Define the function character frequency,Accept one argument: file_path (the path to the file whose character frequency is to be calculated).

Step 6:	 Open the file specified by file_path in read mode ('r'), Read the content of the file into the variable content.

Step 7:	 Initialize an empty defaultdict of type int (which will store the frequency of each character).

Step 8:	 Loop through each character in the content: For each character ch, increment its corresponding frequency in the dictionary d1.

Step 9:	 Return the dictionary d1, which contains the frequency of each character in the file.

Step 10:	 Terminate the program.
### PROGRAM
```
input_str=input()
grades=input_str.split(',')
try:
    l1=[int(item) for item in grades]
except:
    print("The grades you entered were in an invalid format.")
    print(grades)
else:
    l1=[int(item) for item in grades]
    print(l1)
```
### OUTPUT

 ![image](https://github.com/user-attachments/assets/a23ca630-bc9b-439a-b4f1-fcad2a2e0711)

 
### RESULT
Thus the python program for finding character frequency count in a file, was implemented and executed successfully.

ExNo.4(d). CLASS AND OBJECTS- AREA OF CIRCLE

### AIM
To write Python Program to take the radius from the user and find the area of the circle using class name 'umbrella' and function name 'rain'
### ALGORITHM

Step 1:	 Begin the program.

Step 2:	  Create a class named umbrella.

Step 3:	 Define a method rain(self, r) that accepts a radius r as an argument.

Step 4:	 Inside the rain method: Calculate the area of a circle using the formula: Area = π * r^2. Use the math.pi constant to get the value of π and perform the calculation. Print the 
          result, formatted to two decimal places.

Step 5:	 Prompt the user for an integer input to represent the radius of the circle.

Step 6:	 Create an instance of the umbrella class and store it in the variable u.

Step 7:	 Call the rain method of the umbrella class, passing the user-provided radius r as an argument.

Step 8:	 Terminate the program.
### PROGRAM
```
import math
class umbrella:
    def rain(self,r):
        res=math.pi * r * r
        print(f"Area of circle: {res:.2f}")
r=int(input())
u=umbrella()
u.rain(r)
```
### OUTPUT
![image](https://github.com/user-attachments/assets/aa51e6ae-8312-4d49-85a6-774bfead5223)

 
### RESULT
Thus the python program for calculating the area of a circle was implemented and executed successfully.

Exp.No:4(e)	SEB- ARITHMETIC CALCULATION USING CLASS

### AIM
To write a python program to perform addition and division operation using class and if,elif..
class name should be saveetha, function name should be setvalues( to set a and b values) add and div.cases : choice 1 ->perform addition ,choice 2-> perform division ,  choice 0 -> exiting, other choices -> print 'invalid choice'
### ALGORITHM

Step 1:	 Begin the program.

Step 2:	 Create the Saveetha Class.

Step 3:	 Create the main() function.

Step 4:	 Set the values of a and b using the setvalues(a, b) method of the Saveetha object.

Step 5:	 Start a while True loop to repeatedly ask the user for a choice. 

Step 6:	 Take the user's choice (1 for addition, 2 for division, 0 for exit).

Step 7:	 If the choice is 1, call the add() method and print the result (converted to an integer).

Step 8:	 If the choice is 2, call the div() method and print the result (converted to an integer). Handle division by zero.

Step 9:	 If the choice is 0, print "Exiting!" and exit the loop.

Step 10:	 If the choice is not 1, 2, or 0, print "Invalid choice"

Step 11:	   Terminate the program.
### PROGRAM
```class Saveetha:
    def __init__(self):
        self.a = 0
        self.b = 0

    def setvalues(self, a, b):
        self.a = a
        self.b = b

    def add(self):
        return self.a + self.b

    def div(self):
        if self.b != 0:
            return self.a / self.b
        else:
            return "Error: Division by zero"
def main():
    saveetha_obj = Saveetha()
    a = float(input())``
    b = float(input())
    while True:
        saveetha_obj.setvalues(a, b)
        choice = int(input())
        if choice == 1:
            result = saveetha_obj.add()
            print(f"Result:  {int(result)}")
        elif choice == 2:
            result = saveetha_obj.div()
            print(f"Result:  {int(result)}")
        elif choice == 0:
            print("Exiting!")
            break
        else:
            print("Invalid choice")

# Run the main function
main()
```
### OUTPUT
![Screenshot 2025-06-02 113428](https://github.com/user-attachments/assets/14520a11-b0e3-4444-8a58-c7d8c9e0e3f6)

 
### RESULT
Thus the arithmetic calculation using class has been  implemented and executed successfully.




