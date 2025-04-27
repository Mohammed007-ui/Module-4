# Exp.No:20  
## SEB - ARITHMETIC CALCULATION USING CLASS

---

### AIM  
To write a Python program to perform addition and division operations using a class. The class should be named `Saveetha`, and the function names should be `setvalues` (to set `a` and `b` values), `add`, and `div`. The program should handle the following cases:  
- `choice 1` → Perform addition  
- `choice 2` → Perform division  
- `choice 0` → Exit  
- For other choices, print 'Invalid choice'

---

### ALGORITHM

1. Begin the program.  
2. Create a class `Saveetha`.  
3. Define the following methods inside the `Saveetha` class:  
   - `__init__(self)`: Initializes `a` and `b` to zero.  
   - `setvalues(self, a, b)`: Sets the values of `a` and `b`.  
   - `add(self)`: Performs the addition operation.  
   - `div(self)`: Performs the division operation. If `b` is zero, returns an error message for division by zero.  
4. Create a `main()` function.  
5. Take input from the user for the values of `a` and `b` using `setvalues(a, b)` method.  
6. Use a `while True` loop to repeatedly ask the user for a choice:  
   - If the choice is 1, call the `add()` method and print the result.  
   - If the choice is 2, call the `div()` method and print the result. Handle division by zero.  
   - If the choice is 0, print "Exiting!" and exit the loop.  
   - If the choice is not 1, 2, or 0, print "Invalid choice".  
7. Terminate the program.

---
### PROGRAM

```

class Saveetha:
    def __init__(self):
        self.a = 0
        self.b = 0

    def setvalues(self, a, b):
        self.a = a
        self.b = b

    def add(self):
        return self.a + self.b

    def div(self):
        if self.b == 0:
            return "Error: Division by zero is not allowed."
        else:
            return self.a / self.b
def main():
    s = Saveetha()
    a = int(input("Enter the first number (a): "))
    b = int(input("Enter the second number (b): "))
    s.setvalues(a, b)

    while True:
        print("\nChoices:")
        print("1. Addition")
        print("2. Division")
        print("0. Exit")
        choice = int(input("Enter your choice: "))

        if choice == 1:
            result = s.add()
            print(f"Addition result: {result}")
        elif choice == 2:
            result = s.div()
            print(f"Division result: {result}")
        elif choice == 0:
            print("Exiting!")
            break
        else:
            print("Invalid choice")
main()
```

### OUTPUT
![image](https://github.com/user-attachments/assets/d7341244-6d86-48ef-a0a4-a3006133c50f)

### RESULT
Thus, the Python program to perform addition and division operations using a class Saveetha was successfully written and executed.
