<h1 id="12f/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Given $X_n=k$, the next size is a sum of $k$ independent reproduction counts. Multiplication of their [probability generating functions](../../../../../../probability-generating-function.md) gives $\mathbb E[s^{X_{n+1}}\mid X_n=k]=G(s)^k$. Averaging this [conditional expectation](../../../../../../conditional-expectation.md) proves

$$
\boxed{G_{n+1}(s)=\mathbb E[G(s)^{X_n}]=G_n(G(s)).}
$$

With one initial individual, $G_0(s)=s$ and $G_1(s)=G(s)$, so $G_n$ is the $n$-fold composition of $G$ with itself.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [12F](../../12f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
