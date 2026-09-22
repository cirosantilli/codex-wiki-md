# Abstract syntax tree

↑ **Parent:** [Programming language](programming-language.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Abstract_syntax_tree)

An [abstract syntax tree](abstract-syntax-tree.md) is a [rooted tree](rooted-tree.md) recording the meaningful syntactic pieces of a program and how they fit together. A [program identifier](program-identifier.md) such as `x`, a [literal value](literal-value.md) such as `2`, and a node representing [addition](addition.md) have different roles. Their arrangement answers structural questions: which [program expression](program-expression.md) supplies an operand, which name is a [variable assignment](variable-assignment.md) target, and which construct encloses another. This makes an [abstract syntax tree](abstract-syntax-tree.md) useful to a [compiler](compiler.md), an [interpreter](interpreter-computing.md), and the [type system](type-system.md) that checks a program.

The word "abstract" describes what is omitted. [Lexical analysis](lexical-analysis.md) first recognizes [lexical tokens](lexical-token.md), such as `x`, `=`, `2`, `+`, `3`, `*`, `4`. A concrete [parse tree](parse-tree.md) can retain [grammar derivation](grammar-derivation.md) structure, including punctuation and intermediate [context-free grammar](context-free-grammar.md) categories such as expression, term and factor. An [abstract syntax tree](abstract-syntax-tree.md) usually keeps the operation and its operands without all those grammar scaffolds. Parentheses can determine its shape without surviving as separate nodes. A [parser](parser.md) may construct the [abstract syntax tree](abstract-syntax-tree.md) directly; it need not first allocate a concrete [parse tree](parse-tree.md).

An [abstract syntax tree](abstract-syntax-tree.md) records [programming language syntax](programming-language-syntax.md), but does not by itself supply all [programming language semantics](programming-language-semantics.md). In `a+b`, the names do not reveal their current values, and `+` might perform [addition](addition.md) of [integers](integer.md) or concatenate strings. The [programming language](programming-language.md) rules, name bindings, and operand types determine the meaning. In [Python](python-programming-language.md), successfully calling `ast.parse` also does not guarantee that later [compilation](compilation.md) will accept the result: parsing `return 42` succeeds, but compiling that statement outside a function fails. [ast.parse: parsing performs no scoping checks; the return 42 example](python-3-14-documentation/ast-abstract-syntax-trees-python-3-14-documentation.md)

An [abstract syntax tree](abstract-syntax-tree.md) is not [machine code](machine-code.md). Its nodes describe language constructs. A [compiler](compiler.md) can check and transform this structure before translating it into executable instructions; an [interpreter](interpreter-computing.md) can evaluate an appropriate tree directly. The little evaluator below demonstrates this distinction without pretending to implement an entire [programming language](programming-language.md).

**Table of contents**

- [Abstract syntax tree precedence example](abstract-syntax-tree-precedence-example.md)
- [Abstract syntax tree traversal](abstract-syntax-tree-traversal.md)
- [Abstract syntax tree transformation](abstract-syntax-tree-transformation.md)
  - [Constant folding](constant-folding.md)
- [Abstract syntax tree source location](abstract-syntax-tree-source-location.md)

## ↑ Ancestors (3)

1. [Programming language](programming-language.md)
2. [Computer science](computer-science-split.md)
3. [Codex Wiki](split.md)

## ← Incoming links (22)

- [Abstract syntax tree](abstract-syntax-tree.md)
- [Abstract syntax tree precedence example](abstract-syntax-tree-precedence-example.md)
- [Abstract syntax tree source location](abstract-syntax-tree-source-location.md)
- [Abstract syntax tree transformation](abstract-syntax-tree-transformation.md)
- [Abstract syntax tree traversal](abstract-syntax-tree-traversal.md)
- [Algorithm W](algorithm-w.md)
- [Compilation](compilation.md)
- [Compiler](compiler.md)
- [Interpreter (computing)](interpreter-computing.md)
- [Machine code](machine-code.md)
- [Occurs check](occurs-check.md)
- [Operator precedence](operator-precedence.md)
- [Parser](parser.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ia/paper-5/10/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ia/paper-5/10/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ia/paper-5/10/c/solution.md)
- [Program expression](program-expression.md)
- [Program identifier](program-identifier.md)
- [Programming language](programming-language.md)
- [Programming language syntax](programming-language-syntax.md)
- [Propositional logic](propositional-logic.md)
- [Python (programming language)](python-programming-language.md)
