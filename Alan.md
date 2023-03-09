Challenge: Design and implement a simple Turing-complete programming language.

EXTRA HELP AVAILABLE PLEASE AS
```
SYNTAX:

<program> ::= <statement> | <statement> <program>

<statement> ::= <expression> ";" | <assignment> ";" | <control>

<expression> ::= <term> | <term> <add_op> <expression>

<term> ::= <factor> | <factor> <mult_op> <term>

<factor> ::= <number> | <identifier> | "(" <expression> ")" | <function_call>

<assignment> ::= <identifier> "=" <expression>

<control> ::= <if_statement> | <while_statement>

<if_statement> ::= "if" "(" <expression> ")" "{" <program> "}" [ "else" "{" <program> "}" ]

<while_statement> ::= "while" "(" <expression> ")" "{" <program> "}"

<function_call> ::= <identifier> "(" [ <expression> { "," <expression> } ] ")"

<number> ::= <digit>+

<identifier> ::= <letter> { <letter> | <digit> }

<add_op> ::= "+" | "-"

<mult_op> ::= "*" | "/"

<letter> ::= "a" | "b" | ... | "z" | "A" | "B" | ... | "Z"

<digit> ::= "0" | "1" | ... | "9"

GRAMMAR:

A program is one or more statements.
A statement is either an expression, an assignment, or a control statement.
An expression is a term or a term followed by an addition or subtraction operator and another expression.
A term is a factor or a factor followed by a multiplication or division operator and another term.
A factor is a number, an identifier, a function call, or an expression in parentheses.
An assignment is an identifier followed by an equals sign and an expression.
A control statement is either an if statement or a while statement.
An if statement is the keyword if, followed by an expression in parentheses, followed by a program in curly braces, and optionally followed by the keyword else and another program in curly braces.
A while statement is the keyword while, followed by an expression in parentheses, followed by a program in curly braces.
A function call is an identifier followed by a left parenthesis, followed by zero or more comma-separated expressions, followed by a right parenthesis.
A number is one or more digits.
An identifier is a letter followed by zero or more letters or digits.
An addition or subtraction operator is either a plus or a minus sign.
A multiplication or division operator is either an asterisk or a forward slash.
```

Sub-tasks:

1. Implement a lexer and parser to convert source code into an abstract syntax tree (AST). (20 minutes)
1. Implement an interpreter that can execute programs represented by the AST. (30 minutes)
1. Add support for basic arithmetic and logical operations. (10 minutes)
1. Add support for control structures like loops and conditional statements. (10 minutes)
1. Add support for functions and recursion. (20 minutes)
1. Implement an optional feature such as input/output or error handling. (optional - 20 minutes)