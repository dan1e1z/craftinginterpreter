# Lox Interpreter

This is an implementation of the Lox programming language, based on the book "Crafting Interpreters" by Robert Nystrom.

## 📜 Features

- A tree-walk interpreter for Lox.
- Supports variables, functions, classes, and basic control flow.
- Implements the Lox language as described in "Crafting Interpreters."

---

## 🛠️ Setup

### **1. Clone the repository**

```sh
git clone <your-repo-url>
cd <your-repo-folder>
```

### **2. Compile the Lox interpreter**

```sh
javac lox/*.java
```

If there are no errors, the interpreter is ready to run.

### **3. Run Lox in REPL mode**

To start an interactive session, run:

```sh
java com.craftinginterpreters.lox.Lox
```

Example usage:

```
> print "Hello, Lox!";
Hello, Lox!
```

To exit, press **Ctrl + C**.

### **4. Run a Lox script**

You can also execute Lox scripts from a file:

```sh
java com.craftinginterpreters.lox.Lox scripts/example.lox
```

Example `scripts/example.lox`:

```lox
var name = "Alice";
print "Hello, " + name + "!";
```

Expected output:

```
Hello, Alice!
```

---

## 🔧 Regenerating AST Classes

If you modify `GenerateAst.java`, you must regenerate the AST classes before compiling:

```sh
java tool.GenerateAst lox
javac lox/*.java
```

---

## ✅ Testing Your Interpreter

Try running the following Lox script to test variable scoping and loops:

```lox
var a = 10;
while (a > 0) {
    print a;
    a = a - 1;
}
```

Expected output:

```
10
9
8
7
6
5
4
3
2
1
```

---

## 📝 Notes

- Ensure you have **Java 11 or later** installed.

---

## 📌 References

This interpreter follows the Lox language as described in the book [Crafting Interpreters](https://craftinginterpreters.com/).
