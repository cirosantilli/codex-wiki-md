# Compilation arithmetic example

↑ **Parent:** [Compilation](compilation.md)

Consider the [program expression](program-expression.md) `x*(2+3)-4` in a deliberately small [programming language](programming-language-split.md). Its only [program identifier](program-identifier.md) is `x`, supplied as an [integer](integer-split.md) input. Its [literal values](literal-value.md) are nonnegative decimal numerals, interpreted as [integers](integer-split.md). Whitespace is ignored between [lexical tokens](lexical-token.md). Its [context-free grammar](context-free-grammar.md) is:

```
expression ::= term (("+" | "-") term)*
term       ::= factor ("*" factor)*
factor     ::= numeral | "x" | "(" expression ")"
numeral    ::= digit digit*
digit      ::= "0" | "1" | "2" | "3" | "4"
             | "5" | "6" | "7" | "8" | "9"
```

Here `*` outside quotation marks means zero or more repetitions. Repeated operators are grouped to the left, specifying [operator associativity](operator-associativity.md); `term` gives [multiplication](multiplication.md) higher [operator precedence](operator-precedence.md) than [addition](addition.md) and [subtraction](subtraction.md). Parentheses override that grouping. There is no unary minus, [variable assignment](variable-assignment.md), function call, or [side effect](side-effect-computer-science.md) in this language. Evaluation obtains each left operand before its right operand and uses exact [integer arithmetic](integer-arithmetic.md), with no fixed-width overflow.

[Lexical analysis](lexical-analysis.md) recognizes `x`, `*`, `(`, `2`, `+`, `3`, `)`, `-`, `4`. [Parsing](parsing.md) constructs the concrete [abstract syntax tree](abstract-syntax-tree.md) `Sub(Mul(Name(x), Add(Int(2), Int(3))), Int(4))`. Parentheses have done their work by making `Add` a child of `Mul`; they need not survive as nodes. [Constant folding](constant-folding.md) changes this to `Sub(Mul(Name(x), Int(5)), Int(4))`. It cannot replace `Name(x)` by a [literal value](literal-value.md) because the input is supplied at execution. The resulting [function](function-split.md) of the input is $f(x)=5x-4$.

A [compiler](compiler.md) for our [stack machine](stack-machine.md) emits `LOAD x; PUSH 5; MUL; PUSH 4; SUB`. `LOAD x` pushes the current input; `PUSH n` pushes the [integer](integer-split.md) [literal value](literal-value.md) `n`. Each binary instruction removes the top item as its right operand, then the next item as its left operand, and pushes the result. The instruction sequence is an [intermediate representation](intermediate-representation.md) that an [interpreter](interpreter-computing.md) can execute; no [machine code](machine-code.md) has been emitted. A compact binary encoding could make it [bytecode](bytecode.md), but these printed instruction names are only a readable notation.

Why does this [compilation](compilation.md) preserve the result? A [structural induction](structural-induction.md) supplies a short proof outline. Translating a [literal value](literal-value.md) or `x` appends its value to any initial [stack](stack-data-structure.md). For a binary [abstract syntax tree](abstract-syntax-tree.md) node, first translating the left child and then the right child appends the two operand values; the matching instruction replaces them by exactly the original operation's result. Previously present [stack](stack-data-structure.md) items remain intact. [Constant folding](constant-folding.md) also preserves the result because $2+3=5$ in the specified [integer arithmetic](integer-arithmetic.md). Together these facts explain agreement for every [integer](integer-split.md) input, rather than merely agreement for one trial.

## ↑ Ancestors (5)

1. [Compilation](compilation.md)
2. [Compiler](compiler.md)
3. [Programming language](programming-language-split.md)
4. [Computer science](computer-science-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Interpreter arithmetic trace](interpreter-arithmetic-trace.md)
