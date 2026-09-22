<h1 id="3/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For [functions](../../../../../../function-split.md) $f,g:\mathbb N\to\mathbb R$, [big O notation](../../../../../../big-o-notation.md) means

$$
\boxed{f=O(g)\iff\exists C>0\ \exists N\ \forall n\ge N:
|f(n)|\le C|g(n)|.}
$$

Using the [natural logarithm](../../../../../../natural-logarithm.md) and [exponential function](../../../../../../exponential-function.md), $3^{\log n}=n^{\log3}$. Since $\log3>1$, for every $n\ge1$ we have $n\le n^{\log3}$. The witnesses $C=1,N=1$ therefore prove

$$
\boxed{n=O(3^{\log n}).}
$$

## ↑ Ancestors (13)

1. [I](../i.md)
2. [A](../../a.md)
3. [3](../../../3.md)
4. [Discrete mathematics, continuous mathematics, and probability](../../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
5. [2015](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
