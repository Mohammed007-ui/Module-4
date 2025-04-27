# Exp.No:18  
## FILES - FREQUENCY OF CHARACTERS IN A FILE

---

### AIM  
To write a Python program that reads a file and counts the frequency of each character in it.

---

### ALGORITHM

1. Begin the program.  
2. Define the function `create_file()` that accepts two arguments:  
   - `file_path`: The path to the file.  
   - `content`: The string content to be written into the file.  
3. Open the file specified by `file_path` in write mode (`'w'`), and write the provided `content` into the file.  
4. Close the file (this is automatically done when exiting the `with` block).  
5. Define the function `character_frequency()` that accepts one argument:  
   - `file_path`: The path to the file whose character frequency is to be calculated.  
6. Open the file specified by `file_path` in read mode (`'r'`), and read its content into the variable `content`.  
7. Initialize an empty dictionary (`d1`) to store the frequency of each character using `defaultdict(int)`.  
8. Loop through each character in the `content`:  
   - For each character `ch`, increment its corresponding frequency in the dictionary `d1`.  
9. Return the dictionary `d1`, which contains the frequency of each character in the file.  
10. Terminate the program.

---

### PROGRAM

```
# Reg.No:
# Name:

# Input content from the user
content = input("Enter the content: ")

# Dictionary to store character frequency
d1 = {}

# Counting frequency of each character
for ch in content:
    if ch in d1:
        d1[ch] += 1
    else:
        d1[ch] = 1

# Printing the frequency
print("\nCharacter Frequencies:")
for char, count in d1.items():
    if char == ' ':
        print("'space' :", count)
    elif char == '\n':
        print("'newline' :", count)
    else:
        print(f"'{char}' :", count)

```

### OUTPUT
![image](https://github.com/user-attachments/assets/943b617f-9325-4a2a-b47f-8226dedf9302)

### RESULT
Thus, the program to count the frequency of characters (without using file handling) was successfully written and executed.


