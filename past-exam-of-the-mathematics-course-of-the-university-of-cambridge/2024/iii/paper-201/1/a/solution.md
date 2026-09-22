<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For the [simple symmetric random walk](../../../../../../simple-symmetric-random-walk.md), $S_n$ is a martingale and the [square-minus-time martingale of a simple symmetric random walk](../../../../../../square-minus-time-martingale-of-a-simple-symmetric-random-walk.md) is

$$
M_n=S_n^2-n
$$

Indeed, conditioning on $\mathcal F_n$ and using $\mathbb E[X_{n+1}]=0$ and $X_{n+1}^2=1$ gives $\mathbb E[S_{n+1}^2\mid\mathcal F_n]=S_n^2+1$.

Apply the [optional sampling theorem for a supermartingale](../../../../../../optional-sampling-theorem-for-a-supermartingale.md) to the bounded [stopping time](../../../../../../stopping-time.md) $T\wedge n$:

$$
\mathbb E[S_{T\wedge n}^2]=\mathbb E[T\wedge n]\leq\mathbb E[T].
$$

Thus the stopped martingale $(S_{T\wedge n})$ is bounded in $L^2$. The [L2 martingale convergence theorem](../../../../../../l2-martingale-convergence-theorem.md) gives convergence in $L^2$, and because $T<\infty$ almost surely its limit is $S_T$. Meanwhile the [monotone convergence theorem](../../../../../../monotone-convergence-theorem.md) gives $\mathbb E[T\wedge n]\to\mathbb E[T]$. Therefore

$$
\mathbb E[S_T^2]=\mathbb E[T].
$$

Finite mean is essential. Let $T=\inf\{n\geq1:S_n=0\}$ be the first return to zero. The one-dimensional [simple symmetric random walk](../../../../../../simple-symmetric-random-walk.md) is recurrent, so $T<\infty$ almost surely, but its first-return time has infinite mean. Since $S_T=0$,

$$
\boxed{\mathbb E[S_T^2]=0\ne\infty=\mathbb E[T].}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 201](../../../paper-201-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
