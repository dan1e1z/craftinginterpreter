# Lexical Analysis (Tokenisation)

Breaks source code into tokens (keywords, operators, identifiers, etc.).
Removes unnecessary whitespace and comments.

# Syntax Analysis (Parsing)

Checks if the token sequence follows the language’s grammar.
Constructs a parse tree or abstract syntax tree (AST).

## A parser really has two jobs:

1. Given a valid sequence of tokens, produce a corresponding syntax tree.

2. Given an invalid sequence of tokens, detect any errors and tell the user about their mistakes.

# Semantic Analysis

Ensures meaningful use of variables, types, and operations.
Detects errors like using an undefined variable or type mismatches.
