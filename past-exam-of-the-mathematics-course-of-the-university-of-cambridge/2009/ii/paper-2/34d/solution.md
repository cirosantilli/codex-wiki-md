<h1 id="34d/solution">Solution</h1>

↑ **Parent:** [34D](../34d.md)

Assume the physical potential is real, as required for the stated conjugation identity, and use the regular radial solution and its analytic continuation. The [differential equation](../../../../../differential-equation-split.md) depends on $k^2$, so exchanging $k$ and $-k$ exchanges the outgoing and incoming coefficients of the same regular solution. Their ratio consequently gives $S(-k)=S(k)^{-1}$. Complex conjugation gives a solution at $k^*$ and exchanges those coefficients, so $S(k)^*S(k^*)=1$.

For real $k$, $|S(k)|=1$, hence $S=e^{2i\delta_0(k)}$ with real phase. The first identity makes the phase odd modulo $\pi$; one can choose odd branches on paired nonzero intervals. A continuous odd branch through zero additionally requires $S(0)=1$, excluding a threshold-resonance exception. For the given rational expression, which has $S(0)=1$, choose

$$
\delta_0(k)=-\arctan(k/\lambda)-\arctan(k/(3\lambda)).
$$

Its small-$k$ behavior is $\delta_0(k)=-4k/(3\lambda)+O(k^3)$. Thus

$$
\boxed{a=\frac4{3\lambda},\qquad4\pi a^2=\frac{64\pi}{9\lambda^2}.}
$$

A zero of the continued $S$ means that the outgoing coefficient vanishes, leaving an incoming-only asymptotic solution. It is paired by $S(k)S(-k)=1$ with a pole at the opposite wave number. The displayed zeros are $-i\lambda$ and $-3i\lambda$. Genuine bound-state poles on the positive imaginary axis correspond to negative energies and decaying regular solutions; their opposite zeros encode the same spectral information. A bare continued pole outside the physical analyticity region need not be a [bound state](../../../../../bound-state.md), so no additional classification of the two poles follows merely from the rational expression without further potential assumptions.

## ↑ Ancestors (10)

1. [34D](../34d.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
