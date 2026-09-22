<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For a [simple predictable process](../../../../../../simple-predictable-process.md), define its [stochastic integral](../../../../../../stochastic-integral.md) by

$$
(H\cdot M)_t=\sum_{k=0}^{n-1}Z_k\bigl(M_{t\wedge t_{k+1}}-M_{t\wedge t_k}\bigr).
$$

It is constant after $t_n$, so the symbol $(H\cdot M)_\infty$ means its value there. Put $\Delta_kM=M_{t_{k+1}}-M_{t_k}$. If $k<\ell$, then $Z_k\Delta_kM Z_\ell$ is $\mathcal F_{t_\ell}$-measurable, and the [conditional expectation](../../../../../../conditional-expectation.md) of $\Delta_\ell M$ given that [sigma-algebra](../../../../../../sigma-algebra.md) is zero. Boundedness of the coefficients and square-integrability of $M$ justify the expectations, so all cross terms vanish:

$$
\mathbb E[(H\cdot M)_\infty^2]
=\sum_k\mathbb E[Z_k^2(\Delta_kM)^2].
$$

For each diagonal term, the [martingale](../../../../../../martingale-split.md) increment identity also gives

$$
\mathbb E[Z_k^2(\Delta_kM)^2]
=\mathbb E[Z_k^2(M_{t_{k+1}}^2-M_{t_k}^2)].
$$

Indeed, the omitted term $2Z_k^2M_{t_k}\Delta_kM$ has expectation zero. Apply the assumed [martingale](../../../../../../martingale-split.md) property of $M^2-[M]$ to replace this difference of squares by the corresponding [quadratic variation](../../../../../../quadratic-variation.md) increment. Thus

$$
\boxed{\mathbb E[(H\cdot M)_\infty^2]
=\sum_k\mathbb E[Z_k^2([M]_{t_{k+1}}-[M]_{t_k})]
=\mathbb E[(H^2\cdot[M])_\infty].}
$$

The intervals $(t_k,t_{k+1}]$ in the Lebesgue–Stieltjes integral exactly match these increments, including possible jumps of $M$.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 35](../../../paper-35-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
