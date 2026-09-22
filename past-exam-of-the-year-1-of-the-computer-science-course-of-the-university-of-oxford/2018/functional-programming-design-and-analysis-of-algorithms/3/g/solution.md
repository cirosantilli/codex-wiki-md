<h1 id="3/g/solution">Solution</h1>

↑ **Parent:** [G](../g.md)

Reverse the children and recursively reverse each child:

```
rev :: CatList a -> CatList a
rev Nil       = Nil
rev (One x)   = One x
rev (Cat l r) = Cat (rev r) (rev l)
```

The proof uses $\operatorname{reverse}(xs\mathbin{++}ys)=\operatorname{reverse}(ys)\mathbin{++}\operatorname{reverse}(xs)$ and [structural induction](../../../../../structural-induction.md). The complete representation is processed and reconstructed in **$\Theta(m)$ time**. This is worst-case optimal for fully processing arbitrary explicit input representations with $m$ constructors; the datatype allows output information to be hidden at any leaf. [Lazy evaluation](../../../../../lazy-evaluation.md) can expose only an initial part of a result sooner, and this statement does not assert that every partial observation costs $m$.

## ↑ Ancestors (12)

1. [G](../g.md)
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
