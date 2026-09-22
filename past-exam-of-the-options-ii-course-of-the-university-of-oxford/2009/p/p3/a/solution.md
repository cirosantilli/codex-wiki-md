<h1 id="p/p3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Interpolation means $p_n(x_i)=f(x_i)$ for every node. Define the [Lagrange basis polynomials](../../../../../lagrange-cardinal-polynomial.md)

$$
\ell_i(x)=\prod_{j\ne i}\frac{x-x_j}{x_i-x_j}.
$$

Distinctness of the nodes makes every denominator nonzero, and $\ell_i(x_j)=\delta_{ij}$. Thus

$$
\boxed{p_n(x)=\sum_{i=0}^nf(x_i)\ell_i(x)}
$$

is a [polynomial](../../../../../polynomial-split.md) of degree at most $n$ with the required values. If two such polynomials existed, their difference would have $n+1$ distinct roots while having degree at most $n$; the [polynomial](../../../../../polynomial-split.md) root bound makes it identically zero. Hence existence and uniqueness hold. The actual degree can be smaller than $n$, despite the conventional name.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [P3](../../p3.md)
3. [P](../../../p.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the options II course of the University of Oxford](../../../../split.md)
6. [Options II course of the University of Oxford](../../../../../options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
