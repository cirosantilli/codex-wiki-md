<h1 id="2/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Let $Z=\int_Xe^{-V}dx$ and $P_B=e^{-V}/Z$. Then

$$
F[P]=\int P\log\frac{P}{P_B}\,dx-\log Z
=D_{\rm KL}(P\|P_B)-\log Z.
$$

By nonnegativity of [Kullback-Leibler divergence](../../../../../../../kullback-leibler-divergence.md),

$$
\boxed{F[P]\geq-\log Z},
$$

with equality exactly when $P=P_B$ almost everywhere. Hence a normalizable $P_B$ is the unique minimizer and, because $\dot F<0$ elsewhere, the unique steady density compatible with the boundary condition.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [2](../../../2.md)
4. [Paper 353](../../../../paper-353-split.md)
5. [Iii](../../../../split.md)
6. [2026](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
