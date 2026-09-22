<h1 id="4/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

If $\varepsilon=0$, then $\rho_{AB}=\sigma_{AB}$ and the desired continuity bound is immediate, so assume $\varepsilon>0$. Apply the [positive-negative decomposition of a Hermitian operator](../../../../../../../positive-negative-decomposition-of-a-hermitian-operator.md) to

$$
X=\rho_{AB}-\sigma_{AB}=X_+-X_-.
$$

Because $\operatorname{Tr}X=0$ and $\lVert X\rVert_1=2\varepsilon$, one has

$$
\operatorname{Tr}X_+=\operatorname{Tr}X_-=\varepsilon.
$$

Thus $\Delta_{AB}=X_+/\varepsilon$ is positive with trace one, hence is a [density operator](../../../../../../../density-matrix.md). Define

$$
\omega_{AB}=\frac{\sigma_{AB}+\varepsilon\Delta_{AB}}{1+\varepsilon}
=\frac{\sigma_{AB}+X_+}{1+\varepsilon}
=\frac{\rho_{AB}+X_-}{1+\varepsilon}.
$$

It is a [convex combination](../../../../../../../convex-combination.md) of states. The equation $\varepsilon\Delta'_{AB}=(1+\varepsilon)\omega_{AB}-\rho_{AB}$ gives

$$
\Delta'_{AB}=X_-/\varepsilon,
$$

which is likewise positive and has trace one.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [C](../../c.md)
3. [4](../../../4.md)
4. [Paper 323](../../../../paper-323-split.md)
5. [Iii](../../../../split.md)
6. [2026](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
