<h1 id="3f/solution">Solution</h1>

↑ **Parent:** [3F](../3f.md)

[Uniform convergence](../../../../../uniform-convergence.md) of $f_n$ to $f$ on an interval $I$ means that for every $\epsilon>0$ there is $N$ such that $|f_n(x)-f(x)|<\epsilon$ for all $n\geq N$ and every $x\in I$. Equivalently $\sup_{x\in I}|f_n(x)-f(x)|\to0$. The same $N$ must work throughout the interval, unlike [pointwise convergence](../../../../../pointwise-convergence.md).

For completeness, [continuity](../../../../../continuous-function.md) is preserved: choose $N$ with uniform error below $\epsilon/3$, and use [continuity](../../../../../continuous-function.md) of $f_N$ at a given $x$ to make $|f_N(y)-f_N(x)|<\epsilon/3$. The [triangle inequality](../../../../../triangle-inequality.md) then gives $|f(y)-f(x)|<\epsilon$. Thus each function involved in the [integral](../../../../../integral.md) is continuous on the closed interval and Riemann integrable. The estimate

$$
\left|\int_a^b f_n(x)dx-\int_a^b f(x)dx\right|\leq\int_a^b|f_n-f|dx\leq(b-a)\sup_{[a,b]}|f_n-f|
$$

proves **convergence of the [integrals](../../../../../integral.md)** by [uniform convergence](../../../../../uniform-convergence.md). When $a=b$ both [integrals](../../../../../integral.md) are zero.

## ↑ Ancestors (10)

1. [3F](../3f.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
