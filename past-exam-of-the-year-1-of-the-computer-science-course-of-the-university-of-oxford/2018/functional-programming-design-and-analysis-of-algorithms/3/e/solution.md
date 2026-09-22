<h1 id="3/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Carry the eventual output tail as an accumulator, thereby avoiding repeated [list concatenation](../../../../../list-concatenation.md):

```
abs :: CatList a -> [a]
abs t = flatten t []
  where
    flatten Nil       zs = zs
    flatten (One x)   zs = x : zs
    flatten (Cat l r) zs = flatten l (flatten r zs)
```

The invariant is `flatten t zs = denotation t ++ zs`. It is immediate for `Nil` and `One`; at `Cat`, applying the two induction hypotheses and [associativity](../../../../../associative-property.md) of [list concatenation](../../../../../list-concatenation.md) proves it. In particular, the empty accumulator gives the required abstraction.

Each [concatenation tree](../../../../../concatenation-tree.md) constructor is processed once, and each `One` emits one result cons. Consequently full production takes **$\Theta(m)$ time**, where $m$ is the input constructor count, on every tree shape. This is a [difference list](../../../../../difference-list.md) calculation written with an explicit tail, an instance of [linear flattening of a binary tree](../../../../../linear-flattening-of-a-binary-tree.md). The [call stack](../../../../../call-stack.md) can have depth $m$ for a badly skewed input; a linear time bound does not imply logarithmic stack space.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [3](../../3.md)
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
