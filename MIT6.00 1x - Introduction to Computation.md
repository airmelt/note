# Lecture 1
## Goal:
- computational thinking
- understand code
- understand ability&limit
- map problem into computation

### Declarative knowledge
statements of fact

### Imperative knowledge
- "how to" methods or recipes
- a description of a set of steps
- a sequence of specific instructions in order which can be tested for changing the value we get and an end test to return answer

### Primitive
- Right: Move the Machine’s head to the right of the current square
- Left: Move the Machine’s head to the left of the current square
- Print: Print a symbol on the current square
- Scan: Identify any symbols on the current square
- Erase: Erase any symbols presented on the current square
- Nothing/halt: Do nothing

### Program
- syntax
- static semantics
- semantics

# Lecture 2
## Introduction to Python
- operators and operands;
- statements
- branching
- conditionals
- iteration

# Lecture 3
## Python For Loop
- common code patterns: iterative programs

# Lecture 4
## Python def function and recursion
- decomposition and abstraction through functions
- introduction to recursion
The __Best__ way to show recursion with Python:
```
unit = '    '
def isPalindrome(s, depth):
    indent = unit * depth
    print indent, 'func called with', s
    if len(s) < 2:
        print indent, 'about to return True from base'
        return True
    else:
        ans = s[0]==s[-1] and isPalindrome(s[1:-1], depth+1)
        print indent, 'about to return True from base'
        return ans

isPalindrome('abcdedcba', 0)
```

# Lecture 5
## Float and Dichotomy
- floating point numbers
- successive refinement
- finding roots
