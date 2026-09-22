<h1 id="12g/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $S(n)=n+1$ be the [successor function](../../../../../../successor-function.md). Define $f$ by [primitive recursion](../../../../../../primitive-recursion.md)

$$
f(0)=0,\qquad f(n+1)=S(S(f(n))).
$$

Induction gives $f(n)=2n$. Then define

$$
g(n)=S(f(n))=2n+1
$$

by composition. Initial functions, composition, and primitive recursion produce [primitive recursive functions](../../../../../../primitive-recursive-function.md), so $f$ and $g$ are [partial recursive functions](../../../../../../computable-function.md) and are visibly defined for every $n$. **Both functions are total.**

## ↑ Ancestors (11)

1. [C](../c.md)
2. [12G](../../12g.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
