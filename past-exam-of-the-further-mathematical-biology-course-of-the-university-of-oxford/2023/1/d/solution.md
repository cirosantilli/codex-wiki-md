<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Because the [hazard functions](../../../../hazard-function.md) are constant, normalization gives $\Lambda_1=2\alpha$ and $\Lambda_2=3\alpha$. The population [characteristic polynomial](../../../../characteristic-polynomial.md) factors as

$$
s^2+5\alpha s-6\alpha^2=(s-\alpha)(s+6\alpha).
$$

Thus

$$
\boxed{\mu=\alpha,\qquad f_1(\tau)=3\alpha e^{-3\alpha\tau},\qquad f_2(\tau)=4\alpha e^{-4\alpha\tau}.}
$$

These [exponential distributions](../../../../exponential-distribution.md) describe ages among currently present [biological cells](../../../../biological-cell-split.md). Their rates differ from the phase-exit rates because [exponential growth](../../../../exponential-growth.md) overrepresents younger entrants. The stable phase ratio is $N_2/N_1=1/2$, so the [G1 phase](../../../../g1-phase.md) and [G2 phase](../../../../g2-phase.md) fractions approach $2/3$ and $1/3$.

Increasing $\alpha$ rescales all times by $1/\alpha$: the population undergoes faster [exponential growth](../../../../exponential-growth.md), its [doubling time](../../../../doubling-time.md) is $\boxed{(\log2)/\alpha}$, and the profile [means](../../../../expected-value-split.md) $1/(3\alpha)$ and $1/(4\alpha)$ decrease. The phase fractions do not depend on $\alpha$. The population [matrix](../../../../matrix.md) has exact solution

$$
\begin{pmatrix}N_1\\N_2\end{pmatrix}
=C e^{\alpha t}\begin{pmatrix}2\\1\end{pmatrix}
+E e^{-6\alpha t}\begin{pmatrix}-3\\2\end{pmatrix},
$$

so population-ratio transients decay relative to the growing term at rate $7\alpha$. This exact population formula does not require initially stationary [cell-cycle age densities](../../../../cell-cycle-age-density.md).

## ↑ Ancestors (12)

1. [D](../d.md)
2. [1](../../1.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the further mathematical biology course of the University of Oxford](../../../split.md)
5. [Further mathematical biology course of the University of Oxford](../../../../further-mathematical-biology-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
