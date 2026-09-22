<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [strong law of large numbers](../../../../../../strong-law-of-large-numbers.md) gives $S_n/n\to-1$ almost surely, so $S_n\to-\infty$. Therefore the infinite-horizon maximum $Z$ is finite and attained almost surely; also $Z\geq0$ because $S_0=0$.

Apply the [Doob maximal inequality](../../../../../../doob-maximal-inequality-for-a-nonnegative-submartingale.md) to $M_k=e^{2S_k}$ through time $n$. Since $\mathbb E M_n=1$,

$$
\mathbb P\left(\max_{0\leq k\leq n}S_k>t\right)\leq e^{-2t}\qquad(t\geq0).
$$

These finite-horizon events increase to $\{Z>t\}$. Continuity of [probability](../../../../../../probability.md) under increasing unions gives

$$
\boxed{\mathbb P(Z>t)\leq e^{-2t}=e^{-\lambda t}.}
$$

For $t<0$ the same bound is trivial, because its right side exceeds $1$. Only bounded-horizon maximal inequalities were used before passing to the limit; no unjustified stopping at an infinite-horizon crossing time is needed.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 33](../../../paper-33-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
