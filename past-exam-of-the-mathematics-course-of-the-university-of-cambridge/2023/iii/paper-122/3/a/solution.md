<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

[Markov inequality](../../../../../../markov-inequality.md) says that a nonnegative random variable $Y$ satisfies

$$
\mathbb P(Y\geq a)\leq\frac{\mathbb EY}{a}
\qquad(a>0).
$$

[Chebyshev inequality](../../../../../../chebyshev-inequality.md) says that a random variable with finite [variance](../../../../../../variance-split.md) satisfies

$$
\mathbb P(|Y-\mathbb EY|\geq a)
\leq\frac{\operatorname{var}Y}{a^2}.
$$

Let $X$ count triangles in $G(n,p)$. The [triangle count in a binomial random graph](../../../../../../triangle-count-in-a-binomial-random-graph.md) calculation gives

$$
\mu=\mathbb EX=\Theta(n^3p^3),
\qquad
\operatorname{var}X=O(n^3p^3+n^4p^5).
$$

Since $p\gg n^{-1}$,

$$
\mu\longrightarrow\infty,
\qquad
\frac{\operatorname{var}X}{\mu^2}
=O\left(\frac1{n^3p^3}+\frac1{n^2p}\right)
\longrightarrow0.
$$

For sufficiently large $n$, $\mu>200$, and [Chebyshev inequality](../../../../../../chebyshev-inequality.md) gives

$$
\boxed{\mathbb P(X<100)
\leq\mathbb P(|X-\mu|>\mu/2)
\leq\frac{4\operatorname{var}X}{\mu^2}
\longrightarrow0.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 122](../../../paper-122-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
