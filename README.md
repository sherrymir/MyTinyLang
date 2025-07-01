# MyTinyLang 🧠💬

A tiny interpreted programming language built in Python. Designed from scratch with basic variable manipulation, arithmetic operations, conditional logic, and jump-based flow control.

## 🚀 Features
- `MOV`, `ADD`, `SUB`, `MUL` — basic arithmetic
- `PRINT` — output variable value
- `JUMP [label]` — unconditional jump
- `IF A < B JUMP label` — conditional branching
- Labels with `label_name:` syntax

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
