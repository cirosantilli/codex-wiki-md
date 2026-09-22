<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Write $P(z)=\mathbb E[z^N]$, $F(z)=\mathbb E[z^{X_1}]$ and $G(z)=\mathbb E[z^{S_N}]$ for the three [probability generating functions](../../../../../probability-generating-function.md). Since both the claim count and every claim size are positive, $P(0)=F(0)=G(0)=0$. Conditioning on the count and using [independence](../../../../../independent-random-variables.md) gives the [random-sum transform identity](../../../../../random-sum-transform-identity.md)

$$
G(z)=\sum_{n\ge1}p_n F(z)^n=P(F(z)).
$$

The crucial point is that the count recurrence begins at $n=2$. Multiplying it by $n z^{n-1}$ and summing, we obtain

$$
\begin{aligned}
P'(z)-p_1
&=\sum_{n\ge2}(an+b)p_{n-1}z^{n-1}\\
&=\sum_{m\ge1}(a(m+1)+b)p_mz^m\\
&=azP'(z)+(a+b)P(z).
\end{aligned}
$$

Consequently $(1-az)P'(z)=(a+b)P(z)+p_1$. The [chain rule](../../../../../chain-rule.md) applied to the aggregate [probability generating function](../../../../../probability-generating-function.md) therefore gives

$$
(1-aF(z))G'(z)=\big((a+b)G(z)+p_1\big)F'(z).
$$

These identities hold inside the unit disk, or as identities of [formal power series](../../../../../formal-power-series.md). Since $F(0)=0$, every coefficient of the composition depends on only finitely many count probabilities.

Compare the coefficient of $z^{k-1}$. The product $FG'$ contributes $\sum_{j=1}^{k-1}(k-j)f_jg_{k-j}$, and $F'G$ contributes $\sum_{j=1}^{k-1}j f_jg_{k-j}$. Hence

$$
k g_k=p_1 k f_k+\sum_{j=1}^{k-1}\big(a(k-j)+(a+b)j\big)f_jg_{k-j}.
$$

The required [aggregate recursion for zero-truncated Panjer counts](../../../../../aggregate-recursion-for-zero-truncated-panjer-counts.md) is **initialized by $g_0=0$ and $g_1=p_1f_1$**, and for every $k\ge1$ it is

$$
\boxed{g_k=p_1f_k+\sum_{j=1}^{k-1}\left(a+\frac{bj}{k}\right)f_jg_{k-j}.}
$$

The empty sum at $k=1$ is zero. Every term on the right is known or has a smaller aggregate index. Omitting $p_1f_k$ would incorrectly apply the usual [Panjer recursion](../../../../../panjer-recursion.md) with a zero initial value, producing zero for every aggregate probability.

For the [zero-truncated Poisson distribution](../../../../../zero-truncated-poisson-distribution.md), $p_n/p_{n-1}=\lambda/n$ for $n\ge2$, so $a=0$, $b=\lambda$ and $p_1=\lambda/(e^\lambda-1)$, with $\lambda>0$. Thus

$$
\boxed{g_k=\frac{\lambda}{e^\lambda-1}f_k+\frac{\lambda}{k}\sum_{j=1}^{k-1}j f_jg_{k-j},\qquad k\ge1.}
$$

As a direct [probability generating function](../../../../../probability-generating-function.md) check, $P(z)=(e^{\lambda z}-1)/(e^\lambda-1)$ and therefore $G(z)=(e^{\lambda F(z)}-1)/(e^\lambda-1)$; differentiation reproduces this recursion.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 43](../../paper-43-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
