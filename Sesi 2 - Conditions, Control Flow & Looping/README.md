# Session 2 - Conditions, Control Flow & Looping
## Conditional
Python supports logical conditions that commonly used in mathematics:
1. Equals; a==b
2. Not equals; a!=b
3. Less than; a<b
4. Less than or equal to; a<=b
5. Greater than; a>b
6. Greater than or equal to; a>=b
7. These conditions can be used in several ways, most commonly in "if statements" and loops.

## If Statement
"If Statement" conditions is decision making that might excecuting conditional statement based on expression value.

```Python
if expr:
  statement
```
description:
1. `expr` is an expression evaluated in Boolean context.
2. `statement` is a valid Python statement, which must be indented.

If `expr` is True, then `statement` will excecuting the program.

If `expr` is False, then `statement` will passed or no excecution.

## Indentation
Python indentation is a way of telling a Python interpreter that the group of statements belongs to a particular block of code. A block is a combination of all these statements.
```Python
if expr:
  statement
  statement
  ...
  statement
following_statement
```

### Else Clauses
```Python
if expr:
  statementsA
else:
  statementsB
```

### Elif Clauses
When needed more than two expressions
```Python
if expr:
  statementsA
elif expr:
  statementsB
elif expr:
  statementsC
  ...
else:
  statementsZ
```

### One-Line If Statement
```
Python
if expr: statement_1; statement_2; ...; statement_k
```

### Conditional Expressions
```Python
expr1 if conditional_expr else expr2
```

## "While" Loops
```Python
while expr:
  statementsA
statementsB
```

### "Break & Continue" Statement
When excecuting Python break statement, it will immediately stop all the looping. Excecuting program will continue to first statement after the body loop.
```Python
n = 4
while n > 0:
  n -=1
  if n==2:
    break #Break Statement
  print(n)
print('Iteration end.')
```
```
3
Iteration end.
```
When excecuting Python continue statement, it will stop the iteration. Excecution will jump to the first loop, and controlling expression will be reevaluated to define if loop will excecuting again or not.
```Python
n = 4
while n > 0:
  n -=1
  if n==2:
    continue #Continue Statement
  print(n)
print('Iteration end.')
```
```
3
1
0
Iteration end.
```
### Else Clause
```Python
while expr:
  statementA
else:
  statementsB
```

### Infinite Loops
Infinite loops means write while loop that has never ending.
```Python
while True:
  print("statement")
```

### Nested While Loops
In general, control structure Python can be nested each other, such as if/elif/else can be nested.

### One-Line While Loops
```Python
n = 10
while n > 0: n -= 1; print(n)
```
### Numeric Range Loop
```Python
for i = 1 to 5
  print('Number')
```

Basically, there are three-expression loop:
1. An innitialization
2. An expression specifying an ending condition
3. An action to be performed at the end of each iteration

### Collection-Based or Iteration-Based Loop
```Python
for var in iterable:
  statements
```
