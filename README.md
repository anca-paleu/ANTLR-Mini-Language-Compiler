# Custom Mini-Language Compiler with ANTLR

A custom compiler frontend built using the ANTLR framework. This tool performs complete lexical analysis, parsing, and semantic validation for a custom mini-programming language, leveraging the Visitor design pattern for AST traversal.

## 📌 Features
* **Lexical & Syntactic Analysis:** Tokenizes source code (ignoring whitespaces and comments) and parses language constructs like loops, conditionals, variable declarations, and function definitions.
* **AST Traversal:** Uses a custom Visitor implementation to traverse the syntax tree and collect global variables, local variables, and control structures.
* **Strict Semantic Analyzer:** * Enforces scope rules and variable/function uniqueness.
  * Validates function calls (argument counts and type matching).
  * Checks type compatibility for assignments and return statements.
  * Ensures the presence of a valid, non-recursive entry point (`main` function).
* **Error Logging:** Captures and writes all lexical, syntactic, and semantic compilation errors to a dedicated output file.

## 🚀 How to Run
1. Generate the lexer and parser classes using ANTLR from the provided grammar file.
2. Compile the generated Java/C++ code along with the custom Semantic Analyzer logic.
3. Run the compiler by passing a source code file written in the custom mini-language.
4. Review the generated text files for token lists, symbol tables, and compilation logs.
