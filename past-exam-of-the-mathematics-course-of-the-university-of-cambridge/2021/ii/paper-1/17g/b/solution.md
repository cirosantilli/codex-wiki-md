<h1 id="17g/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

[Chebyshev inequality](../../../../../../chebyshev-inequality.md) states that, for a random variable $Y$ of finite [variance](../../../../../../variance-split.md) and any $a>0$,

$$
\mathbb P(|Y-\mathbb EY|\geq a)
\leq\frac{\operatorname{var}Y}{a^2}.
$$

Let $X=\sum_T I_T$ count [triangles](../../../../../../triangle-in-a-graph.md), where $T$ ranges over the three-element vertex sets and $I_T$ is the corresponding [indicator random variable](../../../../../../indicator-random-variable.md). Then

$$
\mu=\mathbb EX=\binom n3p^3.
$$

Two distinct triangle indicators are independent unless their triangles share an edge. There are

$$
\binom n2\binom{n-2}2
$$

unordered pairs sharing an edge, and each covariance is

$$
p^5-p^6\leq p^5.
$$

Therefore

$$
\operatorname{var}X
\leq\binom n3p^3
+2\binom n2\binom{n-2}2p^5.
$$

It follows that

$$
\frac{\operatorname{var}X}{\mu^2}
=O\left(\frac1{n^3p^3}+\frac1{n^2p}\right)
\longrightarrow0
$$

when $np\to\infty$. Chebyshev's inequality now gives

$$
\mathbb P(X=0)
\leq\mathbb P(|X-\mu|\geq\mu)
\leq\frac{\operatorname{var}X}{\mu^2}
\longrightarrow0.
$$

Hence

$$
\boxed{\mathbb P(E_3)\longrightarrow1},
$$

as summarized by the [triangle count in a binomial random graph](../../../../../../triangle-count-in-a-binomial-random-graph.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [17G](../../17g.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
