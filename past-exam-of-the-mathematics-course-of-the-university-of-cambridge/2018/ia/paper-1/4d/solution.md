<h1 id="4d/solution">Solution</h1>

↑ **Parent:** [4D](../4d.md)

The [radius of convergence](../../../../../radius-of-convergence.md) of the [power series](../../../../../power-series.md) $\sum_{n\geq0}a_nz^n$ is

$$
R=\sup\{r\geq0:\text{the series converges for every }|z|<r\}.
$$

If $|z|<R$, choose $w$ with $|z|<|w|<R$. Since $a_nw^n\to0$, those terms are [bounded](../../../../../bounded-sequence.md), say $|a_nw^n|\leq M$. Therefore

$$
|a_nz^n|\leq M\left|\frac zw\right|^n,
$$

and comparison with a [geometric series](../../../../../geometric-series.md) proves [absolute convergence](../../../../../absolute-convergence.md). If $|z|>R$, convergence would imply absolute convergence at every smaller modulus by the same argument, contradicting the definition of $R$.

If $|a_n|\leq|b_n|$, convergence of $\sum b_nw^n$ implies absolute convergence of $\sum a_nz^n$ whenever $|z|<|w|$. Letting $|w|$ approach the radius of the $b$-series shows that **$R_a\geq R_b$**.

## ↑ Ancestors (10)

1. [4D](../4d.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ia](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
