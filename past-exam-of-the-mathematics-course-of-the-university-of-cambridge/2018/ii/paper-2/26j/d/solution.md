<h1 id="26j/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Set

$$
m_N=\mathbb EY_N=\frac1N\sum_{k=1}^N\mathbb EX_k.
$$

By [variance additivity for independent random variables](../../../../../../variance-additivity-for-independent-random-variables.md),

$$
\lVert Y_N-m_N\rVert_2^2
=\operatorname{Var}(Y_N)
=\frac1{N^2}\sum_{k=1}^N\operatorname{Var}(X_k)
\leq\frac1N\longrightarrow0.
$$

Thus $Y_N$ differs in $L^2$ by $o(1)$ from the deterministic scalar $m_N$. The [L2 convergence of averages of independent variables with bounded second moments](../../../../../../l2-convergence-of-averages-of-independent-variables-with-bounded-second-moments.md) gives the necessary and sufficient condition

$$
\boxed{
Y_N\text{ converges in }L^2
\Longleftrightarrow
\frac1N\sum_{k=1}^N\mathbb EX_k
\text{ converges}.}
$$

## ↑ Ancestors (11)

1. [D](../d.md)
2. [26J](../../26j.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
