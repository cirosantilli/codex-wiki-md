<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For $S_n\sim\operatorname{Pois}(n)$,

$$
\begin{aligned}
\mathbb E[(n-S_n)^+]
&=\sum_{k=0}^{n-1}(n-k)e^{-n}\frac{n^k}{k!}\\
&=n\mathbb P(S_n=n-1)
=e^{-n}\frac{n^{n+1}}{n!}.
\end{aligned}
$$

Consequently

$$
\mathbb E[Y_n^-]
=\frac1{\sqrt n}\mathbb E[(n-S_n)^+]
=\frac{e^{-n}n^{n+1/2}}{n!}.
$$

Part c says that this tends to $1/\sqrt{2\pi}$. Rearranging gives the [Stirling formula](../../../../../../stirling-formula.md)

$$
\boxed{n!\sim\sqrt{2\pi n}\left(\frac ne\right)^n.}
$$

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 201](../../../paper-201-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
