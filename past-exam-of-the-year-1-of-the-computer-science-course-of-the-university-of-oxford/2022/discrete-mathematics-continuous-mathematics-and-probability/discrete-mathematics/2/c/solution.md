<h1 id="discrete-mathematics/2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

In [big O notation](../../../../../../big-o-notation.md), $f(n)=O(g(n))$ means that there exist $C>0$ and $n_0$ such that $|f(n)|\le C|g(n)|$ for every integer $n\ge n_0$. For the required [polynomial versus exponential growth](../../../../../../polynomial-versus-exponential-growth.md) comparison, $3^3=3^3$. If $n^3\le3^n$ and $n\ge3$, then

$$
(n+1)^3=n^3\left(1+\frac1n\right)^3\le3^n\left(\frac43\right)^3<3^{n+1}.
$$

By [mathematical induction](../../../../../../mathematical-induction.md), $n^3\le3^n$ for all $n\ge3$. Thus **$n^3=O(3^n)$**, with $C=1$ and $n_0=3$.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [2](../../2.md)
3. [Discrete mathematics](../../../discrete-mathematics.md)
4. [Discrete mathematics, continuous mathematics, and probability](../../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
5. [2022](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
