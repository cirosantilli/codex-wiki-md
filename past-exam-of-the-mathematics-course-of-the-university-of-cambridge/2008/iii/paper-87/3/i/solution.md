<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

In this question $\Delta v$ is the [velocity](../../../../../../velocity.md) increment in the direction of the separation, so $S_2(r)=\langle(\Delta v)^2\rangle$ is a [longitudinal velocity structure function](../../../../../../longitudinal-velocity-structure-function.md). This interpretation is necessary for the kernel in part (iii); the full vector increment has a different kernel.

A [velocity](../../../../../../velocity.md) component that varies very little over distance $r$ is almost the same at the two sample points, so its common part cancels from their difference. A Fourier component acquires the difference factor $e^{i\boldsymbol k\cdot\boldsymbol r}-1$. Its squared magnitude is $2[1-\cos(\boldsymbol k\cdot\boldsymbol r)]$, of order $(kr)^2$ when $kr\ll1$ and of order one after averaging rapid phases when $kr\gg1$. Thus a [longitudinal structure function](../../../../../../longitudinal-velocity-structure-function.md) attenuates large eddies and retains smaller eddies, but is a smooth filter rather than an exact scale cutoff.

The heuristic cutoff $k_c=\pi/r$ marks wavelengths of order $2r$. If motions below that cutoff are treated as perfectly coherent and those above it as uncorrelated at the two points, isotropy allocates one third of their [velocity](../../../../../../velocity.md) [variance](../../../../../../variance-split.md) to the longitudinal component. Since the [turbulent energy spectrum](../../../../../../turbulent-energy-spectrum.md) integrates to one half of total [velocity](../../../../../../velocity.md) [variance](../../../../../../variance-split.md), the uncorrelated high-wavenumber component contributes

$$
S_2(r)\simeq2\left(\frac13\,2\int_{\pi/r}^\infty E(k)dk\right),
$$

or

$$
\boxed{\frac34S_2(r)\sim\int_{\pi/r}^\infty E(k)dk.}
$$

The factor $3/4$ follows from the component and energy normalizations. The approximation discards the finite [gradient](../../../../../../gradient.md) of eddies larger than $r$; part (iii) quantifies that missing contribution.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 87](../../../paper-87-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
