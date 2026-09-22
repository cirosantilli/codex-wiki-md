<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The issue is the [square-integrable](../../../../square-integrable-function.md) condition on the whole real line, not just decay at one end. Because the [quantum harmonic oscillator](../../../../quantum-harmonic-oscillator-split.md) potential is [even](../../../../even-function.md), the even and odd parts of a square-integrable [wavefunction](../../../../wave-function-split.md) are themselves square integrable and satisfy the same equation. It is therefore enough to examine each parity sequence separately.

For a nonterminating sequence, put $b_j=a_{2j+p}$, where $p=0$ or $1$. Its [recurrence relation](../../../../recurrence-relation.md) gives

$$
\frac{b_{j+1}}{b_j}=\frac{4j+2p+1-\epsilon}{(2j+p+2)(2j+p+1)}\sim\frac1j.
$$

Since $\epsilon$ is real for an [energy eigenvalue](../../../../energy-eigenvalue-split.md), the ratio is eventually positive. After multiplying by one constant phase, the tail coefficients are all positive. Choose $0<\delta<1/2$. For sufficiently large $j$, the ratio is at least $(1-\delta)/(j+1)$, so for some $K>0$ the tail coefficients obey $b_j\geq K(1-\delta)^j/j!$. Consequently, for $\xi>0$, the magnitude of $f$ eventually exceeds a positive multiple of $\xi^p e^{(1-\delta)\xi^2}$ after subtraction of a fixed [polynomial](../../../../polynomial-split.md). Multiplication by $e^{-\xi^2/2}$ leaves exponential growth like $e^{(1/2-\delta)\xi^2}$, incompatible with the [square-integrable](../../../../square-integrable-function.md) condition. Thus each nonzero parity series must terminate. The parity argument also excludes cancellation between the two nonterminating sequences at both infinities. This proves [Normalization forces Hermite-series termination](../../../../normalization-forces-hermite-series-termination.md).

If the terminating [polynomial](../../../../polynomial-split.md) has degree $n$, its top nonzero coefficient requires $2n+1-\epsilon=0$. Conversely, when $\epsilon=2n+1$, choosing the seed of parity $n$ nonzero makes the [recurrence relation](../../../../recurrence-relation.md) terminate exactly at degree $n$. The opposite seed must be zero, since that sequence does not terminate. Therefore

$$
\boxed{E_n=\left(n+\frac12\right)\hbar\omega,\qquad n=0,1,2,\ldots.}
$$

The resulting [polynomials](../../../../polynomial-split.md) are proportional to the physicists' [Hermite polynomials](../../../../hermite-polynomial.md), and $\psi_n\propto H_n(\xi)e^{-\xi^2/2}$ is normalizable because any [polynomial](../../../../polynomial-split.md) times this [Gaussian function](../../../../gaussian-function.md) is square integrable. The two parity seeds describe the full solution space of the second-order [differential equation](../../../../differential-equation-split.md); the preceding argument therefore exhausts the normalizable [stationary states](../../../../stationary-state.md). Each [eigenspace](../../../../eigenspace.md) has dimension one. General time-dependent [quantum states](../../../../quantum-state.md) can of course be [superpositions](../../../../superposition-principle.md) of these [energy eigenstates](../../../../energy-eigenstate.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [2014](../../../2014-split.md)
4. [Past exam of the quantum theory course of the University of Oxford](../../../split.md)
5. [Quantum theory course of the University of Oxford](../../../../quantum-theory-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
