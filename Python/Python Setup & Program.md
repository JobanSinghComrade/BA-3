## 🔗 Links

1. [[#⚙️ Download Python & Run Program|Download Python & Run Program]]
2. [[#1. Hello World|Hello World]]
3. [[#2. Datatypes|Datatypes]]

---

## ⚙️ Download Python & Run Program

### Download Python

- Official Python: https://www.python.org/downloads/
- Microsoft Store (Windows): search "Python" in the Microsoft Store

### Run Steps

1. Install Python using one of the links above, then open your terminal (Command Prompt on Windows, or Terminal on Mac/Linux) and verify installation:

```bash
python --version
```

On some systems (mainly Mac/Linux) you may need to use `python3` instead of `python`:

```bash
python3 --version
```

2. Write your program in a file with a `.py` extension, e.g. `hello_world.py`.

3. Run the program directly — Python does not need a separate compile step, since it is interpreted:

```bash
python hello_world.py
```

or, on Mac/Linux:

```bash
python3 hello_world.py
```

That's it — no `.class` files, no separate compile command. Python reads and runs the file in one step.

---

## 1. Hello World

```python
# hello_world.py

print("Hello, World!")
```

Run it with:

```bash
python hello_world.py
```

---
## 2. Datatypes

```python
print("===== 1.INTEGER (int) =====")
rollNo = 3603
print("Value:", rollNo)
print("Type:", type(rollNo))
print("Whole numbers, no decimal point. Example: 1, 100, -5")
  
print()

print("===== 2.FLOAT (float) =====")
marks = 7.84
print("Value:", marks)
print("Type:", type(marks))
print("Numbers with a decimal point. Example: 3.14, -0.5")

print()

print("===== 3. STRING (str) =====")
name = 'Raman'
print("Single quotes:", name)

city = "Punjab"
print("Double quotes:", city)

message = """This is a
multi-line string
using triple quotes"""
print("Triple quotes:", message)

print("Type:", type(name))
print("Text data. You can use single ' ', double \" \", or triple ''' '''/\"\"\" \"\"\" quotes.")
print("Triple quotes are useful for writing text across multiple lines.")

print()

print("===== 4.BOOLEAN (bool) =====")
is_student = True
print("Value:", is_student)
print("Type:", type(is_student))
print("Only two values: True or False")

print()

print("===== 5.LIST (list) =====")
classes = ["BCA", "BSC", "BA", "BCOM"]
print("Value:", classes)
print("Type:", type(classes))
print("Ordered collection, can be changed. Example: [1, 2, 3]")

print()

print("===== 6.TUPLE (tuple) =====")
coordinates = (10, 20)
print("Value:", coordinates)
print("Type:", type(coordinates))
print("Ordered collection, CANNOT be changed. Example: (1, 2, 3)")

print()

print("===== 7.DICTIONARY (dict) =====")
student = {"name": "Raman", "class": "BA"}
print("Value:", student)
print("Type:", type(student))
print("Stores data as key-value pairs. Example: {'key': 'value'}")

print()

print("===== 8.SET (set) =====")
unique_number = {1, 2, 3, 3, 2, 4}
print("Value:", unique_number)
print("Type:", type(unique_number))
print("Collection of unique items, no duplicates allowed.")

print()

print("===== 9. COMPLEX NUMBER (complex) =====")
c = 2 + 3j
print("Value:", c)
print("Type:", type(c))
print("Numbers with a real and imaginary part. The 'j' means imaginary. Example: 2+3j")

print()

print("===== 10.NONE (NoneType) =====")
nothing = None
print("Value:", nothing)
print("Type:", type(nothing))
print("Represents 'no value' or empty.")
```