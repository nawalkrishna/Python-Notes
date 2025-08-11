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

############################################################################################################


  
