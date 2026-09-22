<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Write $m_X=\mathbb E X_1$ and $v_X=\operatorname{Var}(X_1)$. For the [random sum of independent claims](../../../../../random-sum-of-independent-claims.md), conditioning on $N$ gives

$$
\mathbb E[S\mid N]=Nm_X,\qquad \operatorname{Var}(S\mid N)=Nv_X.
$$

The [law of total expectation](../../../../../law-of-total-expectation.md) and the [law of total variance](../../../../../law-of-total-variance.md) therefore give **the aggregate moments**

$$
\boxed{\mathbb ES=(\mathbb EN)m_X,\qquad
\operatorname{Var}(S)=(\mathbb EN)v_X+\operatorname{Var}(N)m_X^2.}
$$

The first term in the [variance](../../../../../variance-split.md) measures variation of the individual claims at a fixed count; the second measures variation of the count itself. These formulas require the indicated moments to be finite.

For the [moment-generating function](../../../../../moment-generating-function.md), [independent random variables](../../../../../independent-random-variables.md) give

$$
\mathbb E[e^{tS}\mid N]=M_X(t)^N,
\qquad
\boxed{M_S(t)=G_N(M_X(t)),}
$$

where $G_N(z)=\mathbb E[z^N]$ is the [probability generating function](../../../../../probability-generating-function.md). This identity holds wherever the expectations are finite; in particular a [moment-generating function](../../../../../moment-generating-function.md) need not exist for positive $t$ for an arbitrary positive claim distribution. The empty sum for $N=0$ is zero.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 34](../../paper-34-split.md)
3. [Iii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
