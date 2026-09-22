<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Set $A=\alpha a^\dagger$ and $B=-\alpha^*a$. Their [commutator](../../../../commutator.md) is

$$
[A,B]=- |\alpha|^2[a^\dagger,a]=|\alpha|^2I.
$$

It commutes with both operators, so the stated [Baker--Campbell--Hausdorff formula](../../../../baker-campbell-hausdorff-formula.md) terminates:

$$
\boxed{D(\alpha)=e^{-|\alpha|^2/2}e^{\alpha a^\dagger}e^{-\alpha^*a}.}
$$

In particular $e^{-\alpha^*a}|0\rangle=|0\rangle$. Expanding the remaining exponential and using $(a^\dagger)^n|0\rangle=\sqrt{n!}|n\rangle$ gives the [number state](../../../../number-state.md) expansion

$$
\boxed{|\alpha\rangle=e^{-|\alpha|^2/2}\sum_{n=0}^\infty\frac{\alpha^n}{\sqrt{n!}}|n\rangle.}
$$

The orthonormality of the [number states](../../../../number-state.md) gives

$$
\boxed{P_n=e^{-|\alpha|^2}\frac{|\alpha|^{2n}}{n!}.}
$$

This is a [Poisson distribution](../../../../poisson-distribution.md) with parameter $\mu=|\alpha|^2$. Its probabilities sum to $e^{-\mu}e^\mu=1$. The phase of $\alpha$ affects the [coherent state](../../../../coherent-state.md)'s relative [probability amplitudes](../../../../probability-amplitude.md) but not its [photon number](../../../../photon-number.md) probabilities. At $\alpha=0$ the distribution is concentrated at $n=0$.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [3](../../3.md)
3. [2022](../../../2022-split.md)
4. [Past exam of the laser science and quantum information processing course of the University of Oxford](../../../split.md)
5. [Laser science and quantum information processing course of the University of Oxford](../../../../laser-science-and-quantum-information-processing-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
