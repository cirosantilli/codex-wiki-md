<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a deterministic $t\le T$, conditional symmetry makes the [conditional characteristic function](../../../../../../conditional-characteristic-function.md) of $X_T-X_t$ invariant under $\theta\mapsto-\theta$. The bounded real and imaginary parts of the exponential are legitimate test functions. Hence

$$
e^{-2i\theta X_t}M_t=e^{-i\theta X_t}\mathbb E[e^{i\theta(X_T-X_t)}\mid\mathcal F_t]=e^{-i\theta X_t}\mathbb E[e^{-i\theta(X_T-X_t)}\mid\mathcal F_t]=\mathbb E[e^{-i\theta X_T}\mid\mathcal F_t].
$$

The right side is a bounded complex martingale. Both sides have continuous versions by the assumptions; equality on rational times and continuity make them indistinguishable. Thus **$e^{-2i\theta X_t}M_t$ is a martingale** on $[0,T]$. Complex martingale assertions mean the corresponding assertions for both real and imaginary parts.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 25](../../../paper-25-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
