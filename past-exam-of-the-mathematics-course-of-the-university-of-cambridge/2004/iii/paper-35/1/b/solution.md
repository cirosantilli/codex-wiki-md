<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $d=\mu-r\mathbf1$ and let $x$ denote the risky holdings as fractions of total wealth. The remaining fraction $1-\mathbf1^Tx$ is in the risk-free asset. Consequently their excess [expected return](../../../../../../expected-return.md) is $d^Tx$ and their [variance](../../../../../../variance-split.md) is $x^T\Sigma x$. The [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) in the [inner product](../../../../../../inner-product.md) defined by $\Sigma$ gives

$$
d^Tx=(\Sigma^{-1}d)^T\Sigma x
\leq\sqrt{d^T\Sigma^{-1}d}\sqrt{x^T\Sigma x}.
$$

Equality with positive excess return holds precisely for $x=cz$, $c>0$, where $z=\Sigma^{-1}d$. Thus solving $\Sigma z=d$ determines both the efficient risky direction and the upper [capital market line](../../../../../../capital-market-line.md) slope. Provided $s=\mathbf1^Tz>0$, the normalized [market portfolio](../../../../../../market-portfolio.md) and its [Sharpe ratio](../../../../../../sharpe-ratio.md) are

$$
\boxed{w_M=\frac{z}{s},\qquad \theta=\sqrt{d^Tz}.}
$$

Here the excess means are $(7,14,21)^T$, so the required equations are

$$
4z_1+z_2+z_3=7,\quad z_1+9z_2+2z_3=14,\quad z_1+2z_2+16z_3=21.
$$

The leading principal minors of $\Sigma$ are $4$, $35$ and $539$, so [Sylvester's criterion](../../../../../../sylvester-s-criterion.md) verifies positive definiteness and the solution is unique.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 35](../../../paper-35-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
