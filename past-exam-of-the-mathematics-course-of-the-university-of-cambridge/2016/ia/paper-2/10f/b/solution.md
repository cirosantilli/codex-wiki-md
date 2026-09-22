<h1 id="10f/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Express the three counts as sums of [indicator variables](../../../../../../indicator-variable.md) for $B_i=0$, $B_i=1$ and $B_i\geq2$. The [linearity of expectation](../../../../../../linearity-of-expectation.md) applies even though the bin counts are dependent. The [binomial distribution](../../../../../../binomial-distribution.md) gives

$$
p_0=(1-1/m)^n,\qquad p_1=\frac nm(1-1/m)^{n-1}.
$$

Thus

$$
\boxed{\mathbb E[E]=m(1-1/m)^n,\qquad \mathbb E[S]=n(1-1/m)^{n-1},}
$$



$$
\boxed{\mathbb E[C]=m\left[1-(1-1/m)^n-\frac nm(1-1/m)^{n-1}\right].}
$$

The relation $E+S+C=m$ checks the sum of these [expectations](../../../../../../expected-value.md). For $m=1$, use the direct deterministic occupancies, or the usual binomial convention $0^0=1$ when $n=1$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [10F](../../10f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
