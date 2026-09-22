<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

`Tree` is a [type constructor](../../../../../type-constructor.md), taking the element [type parameter](../../../../../type-parameter.md) `a` to the [algebraic data type](../../../../../algebraic-data-type.md) `Tree a`. It is not a value and has no ordinary value-level [function type](../../../../../function-type.md); its [kind of a type](../../../../../kind-type-theory.md) is `* -> *`. The other names are [data constructors](../../../../../data-constructor.md) with [polymorphic](../../../../../programming-language-polymorphism.md) [type signatures](../../../../../type-signature.md):

```
One :: a -> Tree a
Two :: Tree a -> Tree a -> Tree a
```

`One` constructs a [leaf-labelled binary tree](../../../../../leaf-labelled-binary-tree.md) with one leaf; `Two` joins two such [trees](../../../../../tree-graph-theory-split.md) under a new internal node. Unlike a general [binary tree](../../../../../binary-tree.md) representation with empty child slots, this representation has no empty tree.[§4.1.1, kinds; §4.2.1, algebraic datatype declarations](../../../../../haskell-2010-language-report.md)

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2018](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
