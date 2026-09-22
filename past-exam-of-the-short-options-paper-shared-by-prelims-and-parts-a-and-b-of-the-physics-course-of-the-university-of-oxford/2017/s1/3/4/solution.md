<h1 id="s1/3/4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Split the sine into exponentials. The $e^{iz}$ term closes in the [upper half-plane](../../../../../upper-half-plane-complex-analysis.md) and picks up the [pole](../../../../../pole.md) $ia$, giving $2\pi i e^{-a}$; the $e^{-iz}$ term closes clockwise below and encloses no [pole](../../../../../pole.md). [Jordan's lemma](../../../../../jordan-s-lemma.md) applies to these separate [contours](../../../../../complex-integration-contour.md). Hence

$$
\boxed{\int_{-\infty}^\infty\frac{\sin x}{x-ia}\,dx=\pi e^{-a},\quad a>0.}
$$

To pass to $a\downarrow0$ without an invalid dominated-convergence [argument](../../../../../argument-complex-analysis.md) on an infinite interval, pair positive and negative $x$ first: the [imaginary part](../../../../../imaginary-part.md) is odd and the [real part](../../../../../real-part.md) is $2\int_0^\infty x\sin x/(x^2+a^2)dx$. On a bounded interval the limit is harmless, while [integration by parts](../../../../../integration-by-parts.md) bounds the oscillatory tail uniformly for $0<a\leq1$. This gives the convergent improper [Dirichlet integral](../../../../../dirichlet-integral.md) $\boxed{\int_{-\infty}^\infty\sin x/x\,dx=\pi}$.

## ↑ Ancestors (12)

1. [4](../4.md)
2. [3](../../3.md)
3. [S1](../../../s1.md)
4. [2017](../../../../2017-split.md)
5. [Past exam of the short options paper shared by Prelims and Parts A and B of the physics course of the University of Oxford](../../../../split.md)
6. [Short options paper shared by Prelims and Parts A and B of the physics course of the University of Oxford](../../../../../short-options-paper-shared-by-prelims-and-parts-a-and-b-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
