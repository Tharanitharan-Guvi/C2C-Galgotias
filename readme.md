# C2C Galgotias University

## Question 4

### Approach 1: Using Arithmetic Operators

```python
nums = int(input())
print("Ones Digit - ", nums % 10)
nums //= 10
print('Tens Digit - ', nums % 10)
nums //= 10
print('Hundreds Digit -', nums % 10)
nums //= 10
print('Thousands Digit - ', nums % 10)
```

### Approach 2: Using While Loop

```python
nums = int(input())
position = ['Ones', 'Tens', 'Hundreds', 'Thousands']
index = 0

while nums:
    print(f'{position[index]} digit - ', nums % 10)
    nums //= 10
    index += 1
```

### Approach 3: Using For Loop

```python
nums = input()
position = ['Ones', 'Tens', 'Hundreds', 'Thousands']
index = 0

for num in nums:
    print(f'{position[index]} digit - ', num)
    index += 1
```

## Question 6

### Approach - 1 Using String Slicing

```
# Pseudo Code
- Input: Integer 'num'
- Convert 'num' to a string
- Use string slicing to reverse the string
- Print the reversed string
```

```python
# Program
num = 12345
num_str = str(num)
reversed_str = num_str[::-1]
print(int(reversed_str))
```

### Approach - 2 Using While Loop

```
# Pseudo Code
- Input: Integer 'num'
- Initialize 'reversed_num' to 0
- While 'num' is not 0:
  - Get the last digit of 'num'
  - Multiply 'reversed_num' by 10 and add the last digit
  - Update 'num' by removing the last digit
- Print 'reversed_num'
```

```python
# Program
num = 12345
reversed_num = 0

while num != 0:
    digit = num % 10
    reversed_num = reversed_num * 10 + digit
    num = num // 10

print(reversed_num)
```

### Approach - 3 Convert to Strings and List, Reverse, and Join

```
# Pseudo Code
- Input: Integer 'num'
- Convert 'num' to a string
- Convert the string to a list of characters
- Reverse the list
- Join the list to form a string
- Convert the string back to an integer
- Print the reversed integer
```

```python
# Program
num = 12345
num_str = str(num)
char_list = list(num_str)
char_list.reverse()
reversed_str = ''.join(char_list)
print(int(reversed_str))
```

## Question 8

You are given a list of numbers `L=[12, 13, 14, 15, 21]`. Write a Python program to perform the following operations:

1. Find the total sum of elements in the list.
2. Find the length of the list.
3. Find the output of `L[:3]`.

### Approach 1: Using Inbuilt Functions

```python
l = [12, 13, 14, 15, 21]
print(sum(l))
print(len(l))
```

### Approach 2: Using While Loop

```python
l = [12, 13, 14, 15, 21]
sum = 0
length = len(l)
index = 0

while index < length:
    sum += l[index]
    index += 1

print(sum)
```

### Approach 3: Using For Loop

```python
l = [12, 13, 14, 15, 21]

sum = 0
length = 0

for i in l:
    sum += i
    length += 1

print(sum)
print(length)
```

**Note:** For the third operation (`L[:3]`), only one possible answer can be provided.
