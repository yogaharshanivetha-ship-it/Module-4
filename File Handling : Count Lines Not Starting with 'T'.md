# File Handling in Python: Count Lines Not Starting with 'T'

## 🎯 Aim
To write a Python program that counts the number of lines in a text file `story.txt` that do **not** start with the alphabet `'T'`.

## 🧠 Algorithm
1. Open the file `story.txt` in **read mode**.
2. Initialize a counter `count` to zero.
3. Iterate through each line of the file:
   - Check if the first character of the line is **not** `'T'`.
   - If the line does not start with `'T'`, increment the `count` by 1.
4. After processing all lines, print the `count` value, which represents the number of lines that do not start with `'T'`.

## 🧾 Program
```
import io

data = """Today is sunny
Nice weather
Tomorrow will be cloudy
Great dinner"""

file = io.StringIO(data)

count = 0
for line in file:
    if not line.startswith("T"):
        count += 1

print(count)
```

## Output

<img width="1265" height="496" alt="image" src="https://github.com/user-attachments/assets/4915a030-10e7-482b-803a-d39de07ff730" />

## Result
The program reads each line from the file story.txt and counts the number of lines that do not start with the character 'T'. After checking all lines, it prints the count.
