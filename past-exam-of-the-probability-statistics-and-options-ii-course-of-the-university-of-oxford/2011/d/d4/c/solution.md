<h1 id="d/d4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Substitute $x=e^{-t}$ to get

$$
\int_0^1(x\log x)^k\,dx=(-1)^k\int_0^\infty t^ke^{-(k+1)t}\,dt
=\boxed{\frac{(-1)^kk!}{(k+1)^{k+1}}},
$$

where the second substitution $u=(k+1)t$ reduces the integral to the supplied gamma integral.

On $(0,1)$, $-x\log x\geq0$. Expand $x^{-x}=e^{-x\log x}=\sum_{j=0}^\infty(-x\log x)^j/j!$. The partial sums increase, so the [monotone convergence theorem](../../../../../monotone-convergence-theorem.md) permits termwise integration. The integral of the $j$-th term is $1/(j+1)^{j+1}$, including $j=0$. Reindexing gives

$$
\boxed{\int_0^1x^{-x}\,dx=\sum_{k=1}^\infty\frac1{k^k}.}
$$

This is finite, for instance because the summands with $k\geq2$ are bounded by $2^{-k}$.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [D4](../../d4.md)
3. [D](../../../d.md)
4. [2011](../../../../2011-split.md)
5. [Past exam of the Probability, statistics and options II course of the University of Oxford](../../../../split.md)
6. [Probability, statistics and options II course of the University of Oxford](../../../../../probability-statistics-and-options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Mathematics and statistics course of the University of Oxford](../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
