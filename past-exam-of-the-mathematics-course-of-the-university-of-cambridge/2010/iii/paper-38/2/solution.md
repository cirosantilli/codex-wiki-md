<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Let $P(z)$, $F(z)$ and $G(z)$ be the [probability generating functions](../../../../../probability-generating-function.md) of $N$, one severity, and $S$, respectively. Positivity of the severities gives $F(0)=0$ and $g_0=p_0$; the [random-sum transform identity](../../../../../random-sum-transform-identity.md) gives $G=P\circ F$. The count recurrence in the [Panjer claim-count class](../../../../../panjer-claim-count-class.md) implies

$$
P'(z)=\sum_{n\ge1}np_nz^{n-1}
=\sum_{n\ge1}(an+b)p_{n-1}z^{n-1}
=azP'(z)+(a+b)P(z).
$$

Use the [chain rule](../../../../../chain-rule.md) and substitute $F(z)$ to obtain

$$
(1-aF(z))G'(z)=(a+b)F'(z)G(z).
$$

Equating the coefficient of $z^{r-1}$ gives

$$
r g_r-a\sum_{j=1}^r(r-j)f_jg_{r-j}
=(a+b)\sum_{j=1}^rj f_jg_{r-j}.
$$

The factor multiplying $f_jg_{r-j}$ after rearrangement is $a(r-j)+(a+b)j=ar+bj$. Therefore the [Panjer recursion](../../../../../panjer-recursion.md) is

$$
\boxed{g_0=p_0,\qquad g_r=\sum_{j=1}^r\left(a+\frac{bj}{r}\right)f_jg_{r-j}\quad(r\ge1).}
$$

These power-series calculations are valid inside the convergence discs of the [probability generating functions](../../../../../probability-generating-function.md), and hence justify the coefficient identities without assumptions about positive [exponential moments](../../../../../exponential-moment.md).

For a [Poisson distribution](../../../../../poisson-distribution.md) count, $p_n/p_{n-1}=\lambda/n$, so $a=0$ and $b=\lambda$. The aggregate recursion becomes

$$
\boxed{g_0=e^{-\lambda},\qquad g_r=\frac\lambda r\sum_{j=1}^rj f_jg_{r-j}.}
$$

To obtain a [moment](../../../../../moment.md) recursion, write $\mu_j=\mathbb E X^j$, $m_j=\mathbb E S^j$, and $m_0=1$. For nonnegative measurable $h$, conditioning on $N=n$ and using exchangeability of the severities gives

$$
\begin{aligned}
\mathbb E[S h(S)]
&=\sum_{n\ge1}p_n n\,\mathbb E\left[X_1h\left(X_1+\sum_{j=2}^nX_j\right)\right]\\
&=\lambda\sum_{m\ge0}p_m\,\mathbb E\left[Xh\left(X+\sum_{j=1}^mX_j\right)\right]
=\lambda\mathbb E[Xh(X+S)],
\end{aligned}
$$

where $X$ on the right is independent of $S$. The second equality uses $np_n=\lambda p_{n-1}$, the [Poisson size-bias identity](../../../../../poisson-size-bias-identity.md). Choosing $h(s)=s^{k-1}$, applying the [binomial theorem](../../../../../binomial-theorem.md), and using [independence](../../../../../independent-random-variables.md) proves the [raw moment recursion for a compound Poisson distribution](../../../../../raw-moment-recursion-for-a-compound-poisson-distribution.md):

$$
\boxed{m_k=\lambda\sum_{j=0}^{k-1}\binom{k-1}{j}\mu_{j+1}m_{k-1-j},\qquad k\ge1.}
$$

For any particular $k$, a finite severity $k$th [moment](../../../../../moment.md) suffices: $(\sum_{i=1}^nX_i)^k\le n^{k-1}\sum_{i=1}^nX_i^k$, and the [Poisson distribution](../../../../../poisson-distribution.md) has finite [moments](../../../../../moment.md) of every order. No positive [moment-generating function](../../../../../moment-generating-function.md) domain is required.

The first three iterations give

$$
m_1=\lambda\mu_1,\qquad
m_2=\lambda\mu_2+\lambda^2\mu_1^2,\qquad
m_3=\lambda\mu_3+3\lambda^2\mu_1\mu_2+\lambda^3\mu_1^3.
$$

Subtracting the appropriate powers of the [expected value](../../../../../expected-value.md) yields

$$
\boxed{\mathbb ES=\lambda\mu_1,\qquad
\operatorname{Var}(S)=\lambda\mu_2,\qquad
\mathbb E[(S-\mathbb ES)^3]=\lambda\mu_3.}
$$

In particular, the aggregate [variance](../../../../../variance-split.md) and third [central moment](../../../../../central-moment.md) involve the raw second and third severity [moments](../../../../../moment.md), rather than their centered counterparts.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 38](../../paper-38-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
