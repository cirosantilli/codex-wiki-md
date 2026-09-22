<h1 id="28k/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Conditionally on $T=t$, $N_T$ is Poisson with mean $\lambda t$. Mixing over the exponential density gives

$$
P(N_T=n)=\int_0^\infty e^{-\lambda t}\frac{(\lambda t)^n}{n!}\nu e^{-\nu t}\,dt
=\frac{\nu\lambda^n}{(\lambda+\nu)^{n+1}}.
$$

**Thus it is geometric on $\{0,1,\ldots\}$ with success probability $\nu/(\lambda+\nu)$.**

## ↑ Ancestors (11)

1. [B](../b.md)
2. [28K](../../28k.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
