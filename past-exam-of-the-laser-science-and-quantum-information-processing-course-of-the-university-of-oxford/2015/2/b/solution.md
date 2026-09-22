<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Orthogonality of the [number states](../../../../number-state.md) makes the [coherent state](../../../../coherent-state.md) norm an exponential series:

$$
\langle\alpha|\alpha\rangle=e^{-|\alpha|^2}\sum_{n=0}^\infty\frac{|\alpha|^{2n}}{n!}=1.
$$

Using $\hat a|n\rangle=\sqrt n|n-1\rangle$ and reindexing $m=n-1$,

$$
\hat a|\alpha\rangle=e^{-|\alpha|^2/2}\sum_{n=1}^\infty\frac{\alpha^n}{\sqrt{(n-1)!}}|n-1\rangle
=\boxed{\alpha|\alpha\rangle}.
$$

It is not an [eigenstate](../../../../eigenstate.md) of the [creation operator](../../../../creation-operator.md). Indeed its supposed eigenvalue would have to be $\alpha^*$, from its expectation, whereas

$$
\left\|(\hat a^\dagger-\alpha^*)|\alpha\rangle\right\|^2
=\langle\hat a\hat a^\dagger\rangle-|\alpha|^2=1.
$$

This nonzero residual holds even at $\alpha=0$.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [2015](../../../2015-split.md)
4. [Past exam of the laser science and quantum information processing course of the University of Oxford](../../../split.md)
5. [Laser science and quantum information processing course of the University of Oxford](../../../../laser-science-and-quantum-information-processing-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
