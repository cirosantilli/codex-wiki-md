<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

All three denote **`iterate :: (a -> a) -> a -> [a]`**, producing $x,g(x),g^2(x),\ldots$. With [lazy evaluation](../../../../../lazy-evaluation.md), demanding and fully evaluating the first $n$ elements costs **$\Theta(n)$ for `f1` and `f2`, and $\Theta(n^2)$ worst-case for `f3`**, under the unit-cost application assumption.

In `f1` the next state is obtained with one new application of `g`. In `f2`, the shared binding `xs` points back to the already generated [list](../../../../../list-abstract-data-type.md); each new element maps `g` over a shared predecessor once. In `f3`, the recursive `f3 g x` is a fresh computation. Producing output position $j$ passes through $j$ separately constructed map layers, so a strict `g` causes $0+1+\cdots+(n-1)$ applications. A non-strict function such as `const 0` can avoid work, so the quadratic statement is a worst-case evaluation bound, not a lower bound for every possible `g`. Merely demanding the outer list spine without its elements is a different cost question.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [2](../../2.md)
3. [Functional programming, design and analysis of algorithms (resit)](../../../functional-programming-design-and-analysis-of-algorithms-resit-split.md)
4. [2016](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
