<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Join the [Laplace operator](../../../../../../laplace-operator.md) to the target operator by

$$
L_tu=((1-t)\delta_{ij}+ta_{ij})\partial_{ij}u,
\qquad0\leq t\leq1.
$$

The family has one ellipticity constant. The global [Schauder estimate](../../../../../../schauder-estimates.md) and the maximum principle give, uniformly in $t$,

$$
\lVert u\rVert_{C^{2,\alpha}(\overline\Omega)}
\leq C\lVert L_tu\rVert_{C^\alpha(\overline\Omega)}
$$

for zero boundary data. Let $I$ contain those $t$ for which $L_t:C_0^{2,\alpha}\to C^\alpha$ is onto. The assumed Laplace solvability gives $0\in I$; the [bounded inverse theorem](../../../../../../bounded-inverse-theorem.md) and small perturbations make $I$ open; and the uniform estimate plus compactness of lower Hölder embeddings makes $I$ closed. The [method of continuity](../../../../../../method-of-continuity.md) yields $I=[0,1]$. At $t=1$ this gives the required solution, and the maximum principle gives uniqueness.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 107](../../../paper-107-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
