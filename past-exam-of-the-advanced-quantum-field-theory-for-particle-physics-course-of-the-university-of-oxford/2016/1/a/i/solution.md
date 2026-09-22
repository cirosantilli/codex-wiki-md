<h1 id="1/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Choose the [covariant derivative](../../../../../covariant-derivative.md) $D_\mu=\partial_\mu+i\mu^{\epsilon/2}eA_\mu$, so the [interaction term](../../../../../interaction-term.md) is $-\mu^{\epsilon/2}e\bar\psi\gamma^\mu A_\mu\psi$. The [gauge transformation](../../../../../gauge-transformation.md) is $A_\mu\mapsto A_\mu+\partial_\mu\alpha$ and $\psi\mapsto e^{-i\mu^{\epsilon/2}e\alpha}\psi$. The derivative of this local phase cancels the added vector-potential term in $D_\mu\psi$, making $i\bar\psi\gamma^\mu D_\mu\psi$ [gauge-invariant](../../../../../gauge-invariance.md).

For renormalized fields and parameters, a complete local [QED](../../../../../quantum-electrodynamics.md) [counterterm](../../../../../counterterm.md) parametrization is

$$
\boxed{\begin{aligned}
\mathcal L={}&i\bar\psi\not\partial\psi-m\bar\psi\psi-\frac14F_{\mu\nu}F^{\mu\nu}
-\mu^{\epsilon/2}e\bar\psi\gamma^\mu A_\mu\psi+\mathcal L_{\rm ct},\\
\mathcal L_{\rm ct}={}&i\delta Z_2\bar\psi\not\partial\psi-\delta m_L\bar\psi\psi
-\frac{\delta Z_3}{4}F_{\mu\nu}F^{\mu\nu}
-\mu^{\epsilon/2}e\delta Z_1\bar\psi\gamma^\mu A_\mu\psi.
\end{aligned}}
$$

With $\psi_0=\sqrt{Z_2}\psi$, $A_0=\sqrt{Z_3}A$, the definitions are $\delta Z_i=Z_i-1$, $\delta m_L=Z_2m_0-m$, and $e_0=\mu^{\epsilon/2}eZ_1/(Z_2\sqrt{Z_3})$. In particular $\delta m_L$ is the coefficient in the [Lagrangian density](../../../../../lagrangian-density.md), not just $m_0-m$.

The [Ward identity](../../../../../ward-identity.md) requires $Z_1=Z_2$ in a gauge-preserving [renormalization scheme](../../../../../renormalization-scheme.md). The kinetic and vertex [counterterms](../../../../../counterterm.md) then combine into $i\delta Z_2\bar\psi\not D\psi$, so [gauge invariance](../../../../../gauge-invariance.md) is explicit and $e_0=\mu^{\epsilon/2}e/\sqrt{Z_3}$. A [photon](../../../../../photon.md) [mass](../../../../../mass.md) term is not an allowed [counterterm](../../../../../counterterm.md) in unbroken [QED](../../../../../quantum-electrodynamics.md). For perturbative inversion one separately adds [gauge fixing](../../../../../gauge-fixing.md), $\mathcal L_{\rm gf}=-(\partial_\mu A^\mu)^2/(2\xi)$, taking $\xi=1$ in [Feynman gauge](../../../../../feynman-gauge.md). That quantization term is not itself part of the gauge-invariant density. The Abelian [Faddeev-Popov determinant](../../../../../faddeev-popov-determinant.md) is field independent for this linear gauge and introduces no interacting ghost contribution.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [2016](../../../../2016-split.md)
5. [Past exam of the advanced quantum field theory for particle physics course of the University of Oxford](../../../../split.md)
6. [Advanced quantum field theory for particle physics course of the University of Oxford](../../../../../advanced-quantum-field-theory-for-particle-physics-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Mathematical and theoretical physics course of the University of Oxford](../../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
