---
{"dg-publish":true,"permalink":"/lectures/lecture-1/"}
---


# Variable Assignment and Data Types in Python

Matthew J. Crossley  

2024

- [[Lectures/Lecture 1#Introduction to Variables in Python\|Introduction to Variables in Python]]
- [[Lectures/Lecture 1#Assigning Variables in Python\|Assigning Variables in Python]]
- [[Lectures/Lecture 1#Data Types in Python\|Data Types in Python]]
- [[Lectures/Lecture 1#Checking Data Types\|Checking Data Types]]
- [[Lectures/Lecture 1#Mutable vs Immutable Data Types\|Mutable vs Immutable Data Types]]
- [[Lectures/Lecture 1#Numeric Types: Integers and Floats\|Numeric Types: Integers and Floats]]
		- [[Lectures/Lecture 1#Integers\|Integers]]
		- [[Lectures/Lecture 1#Floats\|Floats]]
- [[Lectures/Lecture 1#Strings\|Strings]]
- [[Lectures/Lecture 1#Booleans\|Booleans]]
- [[Lectures/Lecture 1#Lists\|Lists]]
- [[Lectures/Lecture 1#Dictionaries\|Dictionaries]]
- [[Lectures/Lecture 1#Quiz: Variable Assignment in Python\|Quiz: Variable Assignment in Python]]
	- [[Lectures/Lecture 1#Quiz: Variable Assignment in Python\|Answer]]
- [[Lectures/Lecture 1#Quiz: Data Types in Python\|Quiz: Data Types in Python]]
	- [[Lectures/Lecture 1#Quiz: Data Types in Python\|Answer]]
- [[Lectures/Lecture 1#Quiz: Mutable and Immutable Types\|Quiz: Mutable and Immutable Types]]
	- [[Lectures/Lecture 1#Quiz: Mutable and Immutable Types\|Answer]]
- [[Lectures/Lecture 1#Quiz: Understanding Lists\|Quiz: Understanding Lists]]
	- [[Lectures/Lecture 1#Quiz: Understanding Lists\|Answer]]


---
## Introduction to Variables in Python

Variables are the building blocks of any programming language, allowing you to store data that can be manipulated and accessed throughout your program.

---
## Assigning Variables in Python

In Python, variables are assigned with a simple `=` operator, and the variable’s type is inferred from the value it is assigned.

```python
x = 5
name = "Alice"
is_valid = True
```

---
## Data Types in Python

Python has several built-in data types, including:

- **Integers**: Whole numbers
- **Floats**: Decimal numbers
- **Strings**: Collections of characters
- **Booleans**: True or False values

---
## Checking Data Types

Use the `type()` function to check the data type of a variable.

```python
print(type(x))
print(type(name))
print(type(is_valid))
```

---
## Mutable vs Immutable Data Types

- **Immutable**: Integer, Float, String, Tuple
    
- **Mutable**: List, Dictionary, Set
    

Understanding the mutability of data types is crucial for managing and manipulating data in Python effectively.

---
## Numeric Types: Integers and Floats

#### Integers

Whole numbers without a decimal point.

`age = 30`

#### Floats

Numbers with a decimal point.

`temperature = 98.6`

---
## Strings

Text data enclosed in quotes. Strings are immutable.

`greeting = "Hello, World!"`

---
## Booleans

Represented by the `True` and `False` values.

`is_student = True`

---
## Lists

Ordered collections of items that can be of mixed types. Lists are mutable.

`colors = ["red", "green", "blue"]`

---
## Dictionaries

Key-value pairs stored in a mutable collection.

person = {"name": "Alice", "age": 30}

---
## Quiz: Variable Assignment in Python

What will be the output of the following code?

```python [1-2|3]
x = 10
y = x + 5
print(y)
```

**Options**

	1. 10
	2. 15
	3. x + 5
	4. Error

### Answer

<details>
  <summary>Click me</summary>
The correct answer is <b>2. 15</b>. The variable <i>y</i> is assigned the value of <i>x + 5</i>, which equals 15.
</details>

---

## Quiz: Data Types in Python

Which data type would you use to store a person’s age in Python?

**Options**

	1. String
	2. Integer
	3. Float
	4. List

### Answer
<details>
  <summary>Click me</summary>
The correct answer is <b>2</b>. Integer. An age is typically represented as a whole number, making the integer data type the most appropriate choice.
</details>

---

## Quiz: Mutable and Immutable Types

Which of the following data types is immutable?

**Options**

	1. List
	2. Dictionary
	3. Tuple
	4. All of the above

### Answer
<details>
  <summary>Click me</summary>
The correct answer is <b>3. Tuple</b>. Tuples are immutable, meaning their contents cannot be changed after creation.
</details>
 
---


## Quiz: Understanding Lists

How do you add an element to the end of a list named `colors`?

```python
colors.add("purple") # 1
colors.append("purple") # 2
colors.insert("purple") # 3
colors += ["purple"] # 4
```

### Answer
<details>
  <summary>Click me</summary>
The correct answer is <b>2. `colors.append("purple")</b>. The <b>append()</b> method adds an element to the end of a list.
</details>