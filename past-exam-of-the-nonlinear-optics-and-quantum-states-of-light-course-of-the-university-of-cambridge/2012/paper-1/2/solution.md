<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

A coherent pump has a [Poisson distribution](../../../../poisson-distribution.md) of [photon](../../../../photon.md) numbers. Second-harmonic conversion couples a pump [number state](../../../../number-state.md) $|n\rangle$ to a state with two fewer pump [photons](../../../../photon.md) with a matrix element proportional to $\sqrt{n(n-1)}$. Different number components therefore evolve at different rates, and the pump becomes correlated with the harmonic mode. Its reduced state is generally neither pure nor exactly Poisson coherent. An undepleted classical-pump approximation suppresses precisely this backaction; it cannot prove that the exact finite-depletion [quantum state](../../../../quantum-state.md) stays coherent. Vacuum input or zero interaction are trivial exceptions.

Let $A=a^{\dagger2}$, $B=a^2$ and $N=a^\dagger a$. The oscillator algebra gives $[A,B]=-4N-2$, $[N,A]=2A$ and $[N,B]=-2B$. Substituting into the definitions proves closure:

$$
\boxed{[K_1,K_2]=-4iK_3,\qquad [K_2,K_3]=iK_1,\qquad [K_3,K_1]=iK_2.}
$$

The factors depend on the stated normalization: $K_3$ has an extra factor one-half relative to $N+1/2$. The [Robertson uncertainty relation](../../../../robertson-uncertainty-principle.md) consequently gives

$$
(\Delta K_1)^2(\Delta K_2)^2\geq\frac14|\langle[K_1,K_2]\rangle|^2
=4\langle K_3\rangle^2.
$$

For a [coherent state](../../../../coherent-state.md) with $n=|\alpha|^2$, [normal ordering](../../../../normal-ordering.md) gives

$$
\langle A B\rangle=n^2,\quad\langle B A\rangle=n^2+4n+2,\quad
\langle A^2\rangle=\alpha^{*4},\quad\langle B^2\rangle=\alpha^4.
$$

Thus $\langle K_1\rangle=\operatorname{Re}\alpha^2$ and $\langle K_2\rangle=-\operatorname{Im}\alpha^2$. In either [variance](../../../../variance-split.md), the fourth-power and $n^2$ terms cancel against the square of the mean, leaving

$$
\boxed{(\Delta K_1)^2=(\Delta K_2)^2=n+\tfrac12,\qquad
\langle K_3\rangle=\tfrac12(n+\tfrac12).}
$$

The [variance](../../../../variance-split.md) product is exactly $4\langle K_3\rangle^2$, so the [coherent state](../../../../coherent-state.md) saturates the stated bound.

[Amplitude-squared squeezing](../../../../amplitude-squared-squeezing.md) in either of these axes means

$$
\boxed{(\Delta K_j)^2<2|\langle K_3\rangle|=\langle N\rangle+\tfrac12\quad(j=1\text{ or }2).}
$$

The other [variance](../../../../variance-split.md) must then rise sufficiently to respect the product inequality. A rotated [field-squared quadrature](../../../../field-squared-quadrature.md) can reveal squeezing in another direction; the criterion concerns the declared quadrature and reference, not merely a reduction in mean optical intensity.

## ↑ Ancestors (13)

1. [2](../2.md)
2. [Paper 1](../../paper-1-split.md)
3. [2012](../../split.md)
4. [Past exam of the nonlinear Optics and Quantum States of Light course of the University of Cambridge](../../../split.md)
5. [Nonlinear Optics and Quantum States of Light course of the University of Cambridge](../../../../nonlinear-optics-and-quantum-states-of-light-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 4 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 4 of the natural sciences course of the University of Cambridge](../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)
