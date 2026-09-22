<h1 id="4d/solution">Solution</h1>

↑ **Parent:** [4D](../4d.md)

First establish a comparison fact for a [power series](../../../../../power-series.md). If it converges at $w\ne0$, its terms $a_nw^n$ are bounded, say $|a_nw^n|\leq C$. For $|z|<|w|$,

$$
\sum_{n=0}^\infty|a_nz^n|\leq C\sum_{n=0}^\infty\left(\frac{|z|}{|w|}\right)^n<\infty
$$

by the [geometric series](../../../../../geometric-series.md). Thus convergence at one point implies [absolute convergence](../../../../../absolute-convergence.md) at every point of smaller modulus.

Let $S$ be the set of moduli of points at which the [power series](../../../../../power-series.md) converges. It contains zero. Define the [radius of convergence](../../../../../radius-of-convergence.md) $R=\sup S\in[0,\infty]$. If $|z|<R$, the definition of [supremum](../../../../../supremum.md) gives a convergent point $w$ with $|w|>|z|$; the comparison just proved gives [absolute convergence](../../../../../absolute-convergence.md) at $z$. This reasoning also applies when $R=\infty$. If $|z|>R$ and the [power series](../../../../../power-series.md) converged there, its modulus would belong to $S$, contradicting the definition of $R$. Therefore

$$
\boxed{\text{convergence for }|z|<R,\qquad\text{divergence for }|z|>R.}
$$

The boundary $|z|=R$ is intentionally undecided by this argument. If $R=0$, only the exterior assertion is nonvacuous.

For the particular coefficients $a_n=1/n$ for $n\geq1$, comparison with $\sum |z|^n$ gives [absolute convergence](../../../../../absolute-convergence.md) whenever $|z|<1$. If $|z|=r>1$, then $r^n/n$ fails to tend to zero: its successive ratio is $rn/(n+1)$, eventually greater than a fixed number bigger than one. The necessary term condition for convergence of a [series](../../../../../series-mathematics.md) therefore fails. Hence

$$
\boxed{R=1.}
$$

For instance the positive boundary point gives the divergent [harmonic series](../../../../../harmonic-series.md); no assertion of universal boundary convergence is needed.

## ↑ Ancestors (10)

1. [4D](../4d.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ia](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
