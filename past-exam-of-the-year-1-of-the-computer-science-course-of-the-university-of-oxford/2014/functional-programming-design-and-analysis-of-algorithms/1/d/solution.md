<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

A [natural-number fold](../../../../../natural-number-fold.md) iterates its first argument once per successor. For [addition](../../../../../addition.md), iterate `Succ` starting at the other operand; for [multiplication](../../../../../multiplication.md), iterate [addition](../../../../../addition.md) starting at zero; for [exponentiation](../../../../../exponentiation.md), iterate [multiplication](../../../../../multiplication.md) starting at one:

```
addF :: Natural -> Natural -> Natural
addF m n = foldNat Succ n m

mulF :: Natural -> Natural -> Natural
mulF m n = foldNat (addF n) Zero m

powerF :: Natural -> Natural -> Natural
powerF m n = foldNat (mulF m) (Succ Zero) n
```

The common identity is $\boxed{\operatorname{foldNat}\ f\ e\ n=f^n(e)}$, with $n$ interpreted through `convert`. Substituting each step and seed reproduces the recursive arithmetic equations of part (b).

## ↑ Ancestors (12)

1. [D](../d.md)
2. [1](../../1.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2014](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
