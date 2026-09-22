# Interpreter arithmetic trace

↑ **Parent:** [Interpreter (computing)](interpreter-computing.md)

Use the [compilation arithmetic example](compilation-arithmetic-example.md) with input $x=7$. An [abstract syntax tree](abstract-syntax-tree.md) [interpreter](interpreter-computing.md) first reads `x`, obtains $2+3=5$, forms $7\cdot5=35$, and finally computes $35-4=31$. Interpreting the folded [abstract syntax tree](abstract-syntax-tree.md) skips the [addition](addition.md) but gives the same result. The compiled [stack machine](stack-machine.md) instructions instead produce the following trace; the top of the [stack](stack-data-structure.md) is written on the right:

```
instruction    stack after instruction
initial        []
LOAD x         [7]
PUSH 5         [7, 5]
MUL            [35]
PUSH 4         [35, 4]
SUB            [31]
```

<a id="image-interpreter-tree-stack-trace"></a>
![](interpreter-tree-stack-trace.png)

**[Figure 4](#image-interpreter-tree-stack-trace). Execution of `x*(2+3)-4` at $x=7$: the original abstract syntax tree and the folded stack machine instructions both give $31$**.

The order in `SUB` is essential: reversing its two popped operands would give $4-35=-31$. The same stored instruction sequence works for input $x=-2$, yielding $(-2)\cdot5-4=-14$, without repeating [parsing](parsing.md) or [constant folding](constant-folding.md). An [abstract syntax tree](abstract-syntax-tree.md) [interpreter](interpreter-computing.md) can likewise reuse its already-parsed tree. Reusing a representation is therefore useful to both approaches; it does not itself distinguish [compilation](compilation.md) from interpretation.

The pleasing part is that a nested [rooted tree](rooted-tree.md) and a flat instruction sequence express the same computation. The [structural induction](structural-induction.md) in the [compilation arithmetic example](compilation-arithmetic-example.md) connects them by a precise [stack](stack-data-structure.md) property. This tiny language always terminates and has no [side effects](side-effect-computer-science.md); richer [programming language semantics](programming-language-semantics.md) require a correctness argument that also accounts for failures, externally visible actions, and possible nontermination.

## ↑ Ancestors (4)

1. [Interpreter (computing)](interpreter-computing.md)
2. [Programming language](programming-language-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)
