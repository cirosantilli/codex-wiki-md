<h1 id="12f/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The matrix recurrence gives $p_{n+1}q_n-p_nq_{n+1}=(-1)^n$ and $q_{n+1}=a_{n+1}q_n+q_{n-1}$. Successive [continued fraction convergents](../../../../../../continued-fraction-convergent.md) bracket $x$, hence

$$
\boxed{\left|x-\frac{p_n}{q_n}\right|\leq\left|\frac{p_{n+1}}{q_{n+1}}-\frac{p_n}{q_n}\right|=\frac1{q_nq_{n+1}}\leq\frac1{a_{n+1}q_n^2}.}
$$

The infinite [continued fraction](../../../../../../continued-fraction.md) is irrational: if $x=p/q$ were rational, a distinct convergent would be at distance at least $1/(qq_n)$, contradicting the first bound once $q_{n+1}>q$. If $x^2$ were rational, this irrational $x$ would have degree two. The [Liouville approximation theorem](../../../../../../liouville-approximation-theorem.md) would then give $|x-p_n/q_n|\geq C/q_n^2$. Comparing with the displayed bound would force $a_{n+1}\leq1/C$ for every $n$, contrary to the unbounded coefficients. Thus **$x^2$ is irrational**, by the [unbounded continued-fraction coefficients exclude quadratic irrationality](../../../../../../unbounded-continued-fraction-coefficients-exclude-quadratic-irrationality.md) argument.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [12F](../../12f.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
