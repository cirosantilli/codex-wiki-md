<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use an [abstract syntax tree](../../../../../abstract-syntax-tree.md) with the following constructors. Here `Expr` denotes the separate [abstract syntax tree](../../../../../abstract-syntax-tree.md) type for a [program expression](../../../../../program-expression.md), `Name` identifies a [variable assignment](../../../../../variable-assignment.md) target, and the square brackets denote an ordered [list](../../../../../list-abstract-data-type.md).

```
Stmt = Assign(Name, Expr)
     | Seq(Stmt, Stmt)
     | Case(Expr, [(Expr, Stmt)])
```

The [list](../../../../../list-abstract-data-type.md) in `Case` must be nonempty. Its first field is the controlling [program expression](../../../../../program-expression.md); each pair contains a label [program expression](../../../../../program-expression.md) and the corresponding body. Keep the pairs in source order and keep repeated labels: this is an ordered search, with the first successful [equality](../../../../../equality-mathematics.md) test choosing the body. A label is an [abstract syntax tree](../../../../../abstract-syntax-tree.md) for a [program expression](../../../../../program-expression.md), not a previously evaluated [integer](../../../../../integer-split.md) or a key in a [map data structure](../../../../../associative-array.md). Evaluating or reordering labels during [compilation](../../../../../compilation.md) would change the specified [programming language semantics](../../../../../programming-language-semantics.md).

`Seq(s,t)` executes `s` before `t`. The delimiters `begin` and `end` need no surviving constructor: the [parser](../../../../../parser.md) uses them to determine the [abstract syntax tree](../../../../../abstract-syntax-tree.md)'s grouping and then returns the enclosed tree. There are no declarations in these blocks that would require a separate binding environment. A [list](../../../../../list-abstract-data-type.md) of statements could replace binary `Seq`; below we choose right-associated binary trees so that the [semantic actions](../../../../../semantic-action.md) are precise.

**The essential representation is an ordered, nonempty list of expression/body pairs, together with assignment and sequencing nodes.** In constructor notation,

$$
\boxed{\operatorname{Case}(e,[(e_1,s_1),\ldots,(e_n,s_n)]),\quad n\geq 1.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Compilers](../../../compilers-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
