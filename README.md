# MyTinyLang 🧠💬

A tiny interpreted programming language built in Python. Designed from scratch with basic variable manipulation, arithmetic operations, conditional logic, and jump-based flow control.

## 🚀 Features
- `MOV`, `ADD`, `SUB`, `MUL` — basic arithmetic  
- `PRINT` — output variable value  
- `JUMP [label]` — unconditional jump  
- `IF A < B JUMP label` — conditional branching  
- Labels with `label_name:` syntax  

## 🎮 Try It Yourself

You can write your own programs in the same style! Just add instructions to the program list and run the interpreter:
program = [
    "MOV A 10",
    "SUB A 3",
    "PRINT A",
    "END"
]

🔭 Coming Soon
Here’s what’s in the pipeline (or in your hands if you wanna build it yourself):

DIV, MOD, and maybe POW

Support for user input via READ

Built-in LOOP syntax for sweet iteration

File-based execution: run from .txt programs

Debug trace mode to see each instruction step-by-step

Syntax errors & crash protection (a.k.a. safety net)

## 🧠 Sample Program

```plaintext
MOV A 1
ADD A 2
SUB A 1
MUL A 5
MOV B 15
IF A < B JUMP less_than
MOV C 999
PRINT C
less_than:
ADD A 1
IF A == 11 JUMP match
SUB A 100
match:
IF A != 0 JUMP end_early
MOV Z 123
PRINT Z
end_early:
PRINT A
END

