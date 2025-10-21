# Regex in Python: Filter Words Without the Letter 'e'

## 🎯 Aim
To write a Python program that filters out and returns all elements from a list **that do not contain the letter `'e'`**, using **regular expressions (regex)**.

## 🧠 Algorithm
1. Import the `re` module.
2. Initialize an empty list `l1` to store results.
3. Define a list of words:  
   `items = ['goal', 'new', 'user', 'sit', 'eat', 'dinner']`
4. Iterate through each word in the list:
   - Use `re.search(r"e", i)` to check if the word contains `'e'`.
   - If **not**, append the word to `l1`.
5. Print the final filtered list.

## 🧾 Program
```
import re
words = ['apple', 'banana', 'cherry', 'date', 'fig', 'grape']
pattern = re.compile(r'^[^e]*$')
filtered_words = [word for word in words if pattern.match(word)]
print("Words without the letter 'e':", filtered_words)
```
## Output
<img width="490" height="42" alt="Screenshot 2025-10-14 210831" src="https://github.com/user-attachments/assets/d5d718e7-e76c-4cff-8602-413a3b37574c" />

## Result
The program successfully filters and returns all elements from the list that do not contain 'e',using regex
