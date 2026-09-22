<h1 id="1/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [multiplicative order](../../../../../../../multiplicative-order.md) $r$ makes the states $|a^k\bmod N\rangle$, $0\leq k<r$, distinct and cyclic under $U_a$. Therefore

$$
\begin{aligned}
U_a|\psi_s\rangle
&=\frac1{\sqrt r}\sum_{k=0}^{r-1}
e^{-2\pi isk/r}|a^{k+1}\bmod N\rangle\\
&=e^{2\pi is/r}\frac1{\sqrt r}\sum_{j=0}^{r-1}
e^{-2\pi isj/r}|a^j\bmod N\rangle.
\end{aligned}
$$

Thus each $|\psi_s\rangle$ is an [eigenvector](../../../../../../../eigenvector.md) with

$$
\boxed{U_a|\psi_s\rangle=e^{2\pi is/r}|\psi_s\rangle}.
$$

These are the Fourier eigenvectors of the cyclic modular-multiplication orbit.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [Paper 324](../../../../paper-324-split.md)
5. [Iii](../../../../split.md)
6. [2025](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
