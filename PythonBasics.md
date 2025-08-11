First Python Program – "Hello World"

Why "Hello World"?
Traditional first step in any programming language.

Checks if Python is working and you can run a program.

Code:
print("Hello, World!")

Explanation:
print → Built-in function to display text.
"Hello, World!" → Text (string) inside quotes.
Parentheses () → Required in Python 3.

Output:
Hello, World!

✅ Always use quotes & correct print().

######################################################################################################

Comments, Variables, Datatypes, and User Inputs

Comments

Comments explain WHY your code does something, help others, and temporarily
disable lines while debugging. - Single-line: start with # (Example: # This is a comment) -
Multi-line/docstring: triple quotes """...""" used for documentation or long comments. Best Practices:
Explain why, not what; keep up-to-date; use TODO/FIXME tags. Common Mistakes: Using // or
/*...*/; leaving unused commented code.


Variables

Variables are names pointing to values (objects). Python is dynamically typed: types
are attached to values, not names. - Assignment: x = 10, name = "Nawal", pi = 3.14 - Naming rules:
letters/digits/underscore, no starting digit, case-sensitive, avoid keywords. - Multiple assignment: a
= b = 0; x, y = 1, 2 - Dynamic typing: v = 5; v = "five" - Scope: local vs global. Avoid overusing
globals. - Aliasing: a = [1, 2]; b = a; b.append(3) → a is now [1, 2, 3].


Datatypes

Core simple types: - int: 5, -3 - float: 3.14 - str: "hello" - bool: True/False - NoneType:None
Strings: immutable, index/slice with [ ], concatenate with +, f-strings for formatting, escape
sequences like \n, raw strings with r"...". Numbers: +, -, *, / (float), // (floor), % (remainder), **
(power). Booleans: truthiness — empty/zero/None → False, others → True. Containers: - list:
ordered, mutable [1,2,3] - tuple: ordered, immutable (1,2) - set: unordered, unique {1,2,3} - dict:
mapping {"key":"value"} Type checking: type(x), isinstance(x, int). Conversions: int("10"),
float("2.5"), str(123). Mutability: mutable (list/dict/set) vs immutable (int/float/str/tuple).


User Inputs 

input(prompt) returns a string. Example: name = input("Enter name: "); print(f"Hello,
{name}!") Convert to number: age = int(input("Enter age: ")) — may raise ValueError. Validation
loop: while True: s = input("Enter integer: ").strip() try: n = int(s); break except ValueError:
print("Invalid number.") Split multiple values: parts = input().split(); nums = [int(x) for x in parts].
Tips: strip() to remove spaces, lower() to normalize, f-strings for formatted output. Security: never
eval() input; validate ranges.

Common mistakes checklist: - Missing quotes for strings - Forgetting int()/float() before arithmetic
- Shadowing built-ins like list or str - Not handling invalid input - Outdated comments

##########################################################################################################

Type Casting in Python

1. What is Type Casting?
Type casting means converting a value from one data type to another.
In Python, this is usually done using built-in functions like int(), float(), str(), etc.
Since Python is dynamically typed, the variable’s type can change after reassignment.

2. Types of Casting


A. Implicit Type Casting (Type Conversion)

Done automatically by Python.
Usually happens when combining different numeric types.
No data loss for safe conversions.
Example:
x = 5  # int
y = 2.5  # float
z = x + y  # int + float → float
Now z is 7.5 (float).

B. Explicit Type Casting

Done manually using casting functions.
You control the conversion.
Can lead to data loss if not careful.

3. Common Casting Functions

int(x) → Converts to integer.
Floats are truncated (no rounding): int(3.9) → 3
Strings must contain valid integers: int("10") → 10
float(x) → Converts to float.
Example: float(3) → 3.0
str(x) → Converts to string.
Example: str(123) → "123"
bool(x) → Converts to Boolean.
Empty values (0, "", [], None) → False
Others → True
list(x) → Converts to list.
Example: list("abc") → ['a', 'b', 'c']

tuple(x), set(x), dict(x) → Convert to other collections (must have compatible structure).

4. Practical Examples

age_str = "25"
age_int = int(age_str) # "25" → 25
price = 99
price_str = str(price) # 99 → "99"
marks = 85.6
marks_int = int(marks) # 85.6 → 85 (truncated)

Common Mistakes
Trying to convert invalid strings: int("abc") → ValueError

Forgetting that int() truncates instead of rounding.

Assuming bool(0.0) is True (it’s False because 0 is considered empty).
  
###############################################################################################
