<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Write $\phi_B=Z^{1/2}\phi$, $Z=1+\delta_Z$, and define the [mass counterterm](../../../../mass-counterterm.md) $\delta_m$ as a squared-mass coefficient:

$$
\mathcal L_{\rm ct}=\frac12\delta_Z(\partial\phi)^2-\frac12\delta_m\phi^2,
\qquad \delta_m=Zm_B^2-m^2.
$$

With the [self-energy](../../../../self-energy.md) convention in [b](../b.md), the inverse [scalar propagator](../../../../scalar-propagator.md) is $p^2-m^2+\delta_Zp^2-\delta_m-\Sigma(p^2)$. Requiring the [pole mass](../../../../pole-mass.md) to equal $m$ therefore gives the [on-shell renormalization scheme](../../../../on-shell-renormalization-scheme.md) condition

$$
\delta_m=m^2\delta_Z-\Sigma(m^2).
$$

At one [loop order](../../../../loop-order.md), $\Sigma_1'=0$; hence a unit [pole residue](../../../../pole-residue.md) also gives $\delta_Z^{(1)}=0$, and

$$
\boxed{\delta_m^{(1)}=-\frac{g_4}{8\pi}\log\left(1+\frac{\Lambda^2}{m^2}\right),\qquad
m_B^2=m^2+\delta_m^{(1)}+O(g_4^2).}
$$

The [mass counterterm](../../../../mass-counterterm.md) [Feynman rule](../../../../feynman-rule.md) is $-i\delta_m$, cancelling the [tadpole diagram](../../../../tadpole-diagram.md). A convention defining a positive mass subtraction by $m_B^2=m^2-\delta_m^{\rm sub}$ instead has $\delta_m^{\rm sub}=-\delta_m$; specifying this convention avoids a spurious sign disagreement.

There is no one-loop [wave-function renormalization](../../../../wave-function-renormalization.md) because the [tadpole diagram](../../../../tadpole-diagram.md) is independent of [momentum](../../../../momentum-split.md). Each one-loop four-point [bubble diagram](../../../../bubble-diagram.md) has two [scalar propagators](../../../../scalar-propagator.md), so its large Euclidean [loop momentum](../../../../loop-momentum.md) integral behaves as $\int d^2k_E/k_E^4$ and is [ultraviolet finite](../../../../ultraviolet-finiteness.md). Thus no divergent [quartic interaction](../../../../quartic-interaction.md) [counterterm](../../../../counterterm.md) is required. Finite coupling redefinitions remain possible. At higher [loop orders](../../../../loop-order.md), finite [wave-function renormalization](../../../../wave-function-renormalization.md) may be needed if unit [pole residue](../../../../pole-residue.md) is imposed; [power counting](../../../../power-counting-in-quantum-field-theory.md) only rules out its [ultraviolet divergence](../../../../ultraviolet-divergence.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the quantum field theory course of the University of Oxford](../../../split.md)
5. [Quantum field theory course of the University of Oxford](../../../../quantum-field-theory-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
