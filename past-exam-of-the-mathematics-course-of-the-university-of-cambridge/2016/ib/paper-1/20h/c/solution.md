<h1 id="20h/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $u_n=\mathbb P_0(X_n=0)$ and $f_n=\mathbb P_0(T=n)$. Decomposing at the first return and using the [Markov property](../../../../../../markov-property.md) gives the [renewal equation](../../../../../../renewal-equation.md)

$$
u_0=1,\qquad u_n=\sum_{k=1}^n f_k u_{n-k}\quad(n\geq1).
$$

For $0<s<1$, define the [probability generating functions](../../../../../../probability-generating-function.md) $U(s)=\sum_{n\geq0}u_ns^n$ and $F(s)=\sum_{n\geq1}f_ns^n=\mathbb E_0[s^T]$. Absolute convergence, or nonnegative summation, justifies the convolution identity $U=1+FU$. The [binomial series](../../../../../../binomial-series.md) gives

$$
U(s)=\sum_{k\geq0}\binom{2k}{k}\left(\frac{s^2}{4}\right)^k=\frac1{\sqrt{1-s^2}}.
$$

Solving the renewal identity gives **the [first-return generating function of the simple symmetric random walk](../../../../../../first-return-generating-function-of-the-simple-symmetric-random-walk.md)**

$$
\boxed{\mathbb E_0[s^T]=F(s)=1-\sqrt{1-s^2},\qquad 0<s<1.}
$$

As consistency checks, $F(s)\to1$ as $s\uparrow1$, confirming recurrence, while $F'(s)=s/\sqrt{1-s^2}\to\infty$. By monotone convergence of $\sum_n n f_n s^{n-1}$, this last limit is $\mathbb E_0T=\infty$, confirming [null recurrent states](../../../../../../null-recurrent-state.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [20H](../../20h.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
