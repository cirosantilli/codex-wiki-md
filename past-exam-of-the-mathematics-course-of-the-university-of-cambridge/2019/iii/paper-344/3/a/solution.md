<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the stable parameters $b,\kappa>0$. The bulk stationary points satisfy $f'(\phi)=a\phi+b\phi^3=0$. For $a<0$, $\phi=0$ has negative curvature, while the two minima are

$$
\boxed{\phi=\pm\phi_B,\qquad\phi_B=\sqrt{-a/b}.}
$$

Both have $f(\pm\phi_B)=-a^2/(4b)$ and $f''(\pm\phi_B)=-2a>0$. To establish minimization at fixed total composition, write

$$
f(\phi)=-\frac{a^2}{4b}+\frac b4(\phi^2-\phi_B^2)^2,
\qquad F\geq-\frac{Va^2}{4b}.
$$

For mean composition $\bar\phi$ with $|\bar\phi|<\phi_B$, a mixture of the two minima with volume fraction $\lambda=(\bar\phi+\phi_B)/(2\phi_B)$ in the positive phase attains this lower bound in the bulk. Macroscopic slabs have only a subextensive interfacial excess [free energy](../../../../../../thermodynamic-free-energy.md), so the bound is attained per unit volume in the [thermodynamic limit](../../../../../../thermodynamic-limit.md). Thus constrained minimization gives [phase coexistence](../../../../../../phase-coexistence.md) in the [mean-field approximation](../../../../../../mean-field-approximation.md); at the endpoints only one phase is needed.

The two equilibrium conditions also follow directly by [constrained optimization](../../../../../../constrained-optimization.md). Introduce a [Lagrange multiplier](../../../../../../lagrange-multiplier.md) $\mu$ for $\lambda\phi_++(1-\lambda)\phi_-=\bar\phi$ in the mixture's bulk [free-energy density](../../../../../../free-energy-density.md). Varying $\phi_+$ and $\phi_-$ gives $f'(\phi_+)=f'(\phi_-)=\mu$; varying $\lambda$ gives $f(\phi_+)-\mu\phi_+=f(\phi_-)-\mu\phi_-$. These equate the [chemical potentials](../../../../../../chemical-potential.md) and [pressures](../../../../../../pressure.md), respectively.

Equivalently, their bulk [chemical potentials](../../../../../../chemical-potential.md) are both zero and their [pressures](../../../../../../pressure.md) are equal:

$$
\boxed{\mu=f'(\pm\phi_B)=0,\qquad\Pi=\mu\phi-f(\phi)=\frac{a^2}{4b}.}
$$

These are precisely the conditions of the [common-tangent construction for phase coexistence](../../../../../../common-tangent-construction-for-phase-coexistence.md): the horizontal supporting tangent touches both minima. Equal [chemical potentials](../../../../../../chemical-potential.md) prevent net composition exchange, and equal [pressure](../../../../../../pressure.md) gives mechanical equilibrium at a flat interface.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 344](../../../paper-344-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
