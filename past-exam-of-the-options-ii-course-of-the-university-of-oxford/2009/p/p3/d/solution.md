<h1 id="p/p3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Every derivative of order $n+1$ of $\sin(2x)$ has absolute value at most $2^{n+1}$. The equally spaced nodes are symmetric about $1/2$. Pair each node $a\leq1/2$ with $1-a$; for $x\in[0,1]$,

$$
|(x-a)(x-(1-a))|=|(x-1/2)^2-(a-1/2)^2|\leq\frac14.
$$

If an unpaired middle node remains, its factor satisfies $|x-1/2|\leq1/2$. Consequently the complete nodal product is at most $2^{-(n+1)}$. The error formula actually gives the stronger estimate

$$
\|f-p_n\|_\infty\leq\frac1{(n+1)!}\leq\boxed{\frac{2^{\lfloor(n+1)/2\rfloor}}{(n+1)!}}.
$$

The first bound tends to zero, proving **[uniform convergence](../../../../../uniform-convergence.md)** on the whole interval. There is no appeal to a general claim that equispaced interpolation always converges; the derivative and symmetric-product bounds are particular to this [analytic function](../../../../../holomorphic-function-split.md) and these nodes.

## ↑ Ancestors (13)

1. [D](../d.md)
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
