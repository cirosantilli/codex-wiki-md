<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the high-temperature state consistently to first order in $\epsilon$. Applying the lower-target [controlled-transfer gate](../../../../controlled-transfer-gate.md) with $\cos\theta_1=1/3$ gives

$$
\rho_1=\frac14\operatorname{diag}\left(1+\epsilon,1,1-\frac\epsilon3,1-\frac{2\epsilon}3\right).
$$

The upper-target gate with $\cos\theta_2=0$ then equalizes the second and fourth populations. The result is

$$
\boxed{\rho_{\mathrm{pp}}=\frac14\operatorname{diag}\left(1+\epsilon,1-\frac\epsilon3,1-\frac\epsilon3,1-\frac\epsilon3\right)
=(1-p)\frac I4+p|00\rangle\langle00|,\qquad p=\frac\epsilon3.}
$$

This is a [pseudo-pure state](../../../../pseudo-pure-state.md); the identity part is unchanged by unitary gates and does not contribute to traceless [NMR](../../../../nuclear-magnetic-resonance-split.md) signals.

For $n$ equal, weakly polarized [spins](../../../../spin.md), the high-temperature expansion is $\rho\simeq2^{-n}[I+(\epsilon/2)\sum_j Z_j]$. The all-zero population is $a_0=2^{-n}(1+n\epsilon/2)$. Preserving this largest population and averaging the other $2^n-1$ populations gives

$$
\boxed{p_n=\frac{2^na_0-1}{2^n-1}\simeq\frac{n\epsilon}{2(2^n-1)}.}
$$

Thus the signal-bearing effective purity falls approximately as $n/2^n$ at fixed small per-spin [polarization](../../../../polarization-waves.md). The linear expansion requires $n|\epsilon|\ll1$. More generally, if the exact single-spin [polarization](../../../../polarization-waves.md) is $r=\tanh(\epsilon/2)$, the same population-preserving averaging gives $p_n=[(1+r)^n-1]/(2^n-1)$, which still decreases exponentially for fixed $0<r<1$. This scaling concerns high-temperature ensemble preparation, not an impossibility theorem for every initialization method.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [5](../../5.md)
3. [2018](../../../2018-split.md)
4. [Past exam of the laser science and quantum information processing course of the University of Oxford](../../../split.md)
5. [Laser science and quantum information processing course of the University of Oxford](../../../../laser-science-and-quantum-information-processing-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
