<h1 id="p/p3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Every [derivative](../../../../../derivative.md) of order $n+1$ of $\sin2x$ has magnitude at most $2^{n+1}$. Pair the [symmetric nodes](../../../../../symmetric-node-pairing-bound-for-interpolation-on-the-unit-interval.md) $a=i/n$ and $1-a$. For $0\le x,a\le1$,

$$
|(x-a)(x-(1-a))|=|(x-1/2)^2-(a-1/2)^2|\le1/4.
$$

If there is an unpaired middle node, its factor has magnitude at most $1/2$. Thus the full nodal product is at most $2^{-(n+1)}$, giving the stronger bound $\|f-p_n\|_\infty\le1/(n+1)!$. In particular this implies the requested

$$
\boxed{\|f-p_n\|_\infty\le\frac{2^{\lfloor(n+1)/2\rfloor}}{(n+1)!}.}
$$

The bound tends to zero by factorial growth, so $\boxed{p_n\to f\text{ uniformly on }[0,1]}$. This conclusion uses smoothness of this particular function and does not assert [uniform convergence](../../../../../uniform-convergence.md) of equispaced interpolation for arbitrary [continuous](../../../../../continuous-function.md) data.

## ↑ Ancestors (13)

1. [D](../d.md)
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
