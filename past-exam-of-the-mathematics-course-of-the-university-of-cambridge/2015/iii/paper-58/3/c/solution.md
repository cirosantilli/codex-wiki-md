<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $g=Gm/r^2>0$, $H_P=-dr/d\log P>0$, $\nabla=d\log T/d\log P$, and $\nabla_\mu=d\log\mu/d\log P$. Consider a small radial [fluid displacement](../../../../../../lagrangian-displacement-fluid-mechanics.md) $\xi$ whose sound-crossing time is short enough to keep its [pressure](../../../../../../pressure.md) equal to its surroundings. Its composition is frozen and its heat exchange negligible. This is the local [stellar convective stability](../../../../../../stellar-convective-stability.md) test.

For gas-pressure-dominated [ideal gas](../../../../../../ideal-gas.md) matter, $\rho\propto\mu P/T$. The ambient gradient is therefore

$$
\frac{d\log\rho}{dr}=-\frac{1-\nabla+\nabla_\mu}{H_P}.
$$

The displaced element conserves [specific entropy](../../../../../../specific-entropy.md) and [mean molecular weight](../../../../../../mean-molecular-weight.md), giving $(d\log\rho/dr)_{\rm parcel}=-(1-\nabla_{\rm ad})/H_P$, where $\nabla_{\rm ad}=(\Gamma_2-1)/\Gamma_2$. The parcel-minus-environment [mass density](../../../../../../density.md) difference is

$$
\frac{\rho_{\rm parcel}-\rho_{\rm ambient}}\rho=\frac{\nabla_{\rm ad}-\nabla+\nabla_\mu}{H_P}\,\xi.
$$

Its [buoyancy](../../../../../../buoyancy.md) acceleration is minus $g$ times this difference. Thus

$$
\boxed{\ddot\xi+N^2\xi=0,\qquad N^2=\frac g{H_P}(\nabla_{\rm ad}-\nabla+\nabla_\mu).}
$$

Positive [stellar buoyancy frequency](../../../../../../stellar-buoyancy-frequency.md) squared gives a restoring force. The gas-pressure-dominated [Ledoux criterion](../../../../../../ledoux-criterion.md) is therefore

$$
\boxed{\text{stable: }\nabla<\nabla_{\rm ad}+\nabla_\mu,\qquad\text{unstable: }\nabla>\nabla_{\rm ad}+\nabla_\mu.}
$$

Equality is marginal in this ideal adiabatic test. For monatomic gas $\nabla_{\rm ad}=2/5$. An inward increase of [mean molecular weight](../../../../../../mean-molecular-weight.md) has $\nabla_\mu>0$ and stabilizes the layer; uniform composition recovers the [Schwarzschild criterion](../../../../../../schwarzschild-criterion.md). For a radiative layer one substitutes the [stellar radiative temperature gradient](../../../../../../stellar-radiative-temperature-gradient.md), $\nabla_{\rm rad}=3\kappa LP/(16\pi acGmT^4)$.

More generally define $\delta=-(\partial\log\rho/\partial\log T)_{P,\mu}$ and $\varphi=(\partial\log\rho/\partial\log\mu)_{P,T}$. The same displacement argument gives $N^2=(g/H_P)[\delta(\nabla_{\rm ad}-\nabla)+\varphi\nabla_\mu]$ and stability for $\nabla<\nabla_{\rm ad}+(\varphi/\delta)\nabla_\mu$. Both coefficients equal one in the gas-dominated ideal-gas limit used above. This is local dynamical stability against convection; it is distinct from global radial collapse and from instabilities requiring heat or composition diffusion.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 58](../../../paper-58-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
