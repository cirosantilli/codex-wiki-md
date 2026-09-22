<h1 id="p/p3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Interpolation means $p_n(x_i)=f(x_i)$ for every node. Define the cardinal [polynomials](../../../../../polynomial-split.md) $\ell_i(x)=\prod_{j\ne i}(x-x_j)/(x_i-x_j)$, which are well defined because the nodes are distinct. They have [degree](../../../../../degree-of-a-polynomial.md) $n$ and satisfy $\ell_i(x_j)=\delta_{ij}$. Hence

$$
\boxed{p_n(x)=\sum_{i=0}^nf(x_i)\ell_i(x)}
$$

belongs to $\Pi_n$ and interpolates. If two [polynomials](../../../../../polynomial-split.md) in $\Pi_n$ interpolate the same data, their difference has $n+1$ distinct zeros but [degree](../../../../../degree-of-a-polynomial.md) at most $n$, so it is zero. This proves uniqueness. The phrase “of [degree](../../../../../degree-of-a-polynomial.md) $n$” denotes membership in $\Pi_n$ here: the actual [degree](../../../../../degree-of-a-polynomial.md) may be smaller, for example for constant data.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [P3](../../p3.md)
3. [P](../../../p.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the Probability, statistics and options II course of the University of Oxford](../../../../split.md)
6. [Probability, statistics and options II course of the University of Oxford](../../../../../probability-statistics-and-options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Mathematics and statistics course of the University of Oxford](../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
