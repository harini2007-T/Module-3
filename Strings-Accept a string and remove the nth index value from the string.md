# Module-3
# 🧹 Strings-Remove Nth Index Character from a String

## 🎯 Aim
To write a Python program that accepts a string and removes the character at a specified index.

## 🧠 Algorithm
1. Define a function named `remove` that takes the input string as an argument.
2. Read the index `n` from the user input.
3. Initialize an empty string `a` to store the new string.
4. Iterate over each index of the string using a `for` loop.
5. Check if the current index `i` is not equal to `n`.
6. If `i != n`, append the character at index `i` to string `a`.
7. After the loop, return the modified string `a`.
8. Print the final result.

## 💻 Program
Add Code Here
```
# Function to remove character at index n
def remove(string, n):
    a = ""  # Initialize an empty string
    for i in range(len(string)):
        if i != n:  # Skip the character at index n
            a = a + string[i]
    return a

# Get input string from user
string = input("Enter a string: ")

# Get index to remove
n = int(input("Enter the index to remove: "))

# Display result
print("Modified string:", remove(string, n))
```
## Output
<img width="799" height="103" alt="image" src="https://github.com/user-attachments/assets/3e436ef5-0879-45bc-9020-d1038a7cc04a" />


## Result
The program successfully takes a string and an index number from the user, removes the character at the specified index, and prints the modified string without that character.
