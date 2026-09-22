<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Consider an element displaced upward by $\xi$ in [hydrostatic equilibrium](../../../../../../hydrostatic-equilibrium.md). Assume it quickly reaches the ambient [pressure](../../../../../../pressure.md), but moves adiabatically and retains its composition. Put $\nabla=d\log T/d\log P$, $\nabla_\mu=d\log\mu/d\log P$, and let $\nabla_{\rm ad}$ be the [adiabatic temperature gradient](../../../../../../adiabatic-temperature-gradient.md). The [equation of state](../../../../../../equation-of-state.md) has differential

$$
d\log\rho=\alpha_P\,d\log P-\delta\,d\log T+\phi\,d\log\mu,
$$

where $\delta=-(\partial\log\rho/\partial\log T)_{P,\mu}$ and $\phi=(\partial\log\rho/\partial\log\mu)_{P,T}$.

At the new [pressure](../../../../../../pressure.md), the parcel-to-environment density difference is

$$
\frac{\rho_{\rm parcel}-\rho_{\rm env}}\rho
=[\delta(\nabla-\nabla_{\rm ad})-\phi\nabla_\mu]\,\Delta\log P.
$$

With positive pressure scale height $H_P=-(d\log P/dr)^{-1}$, $\Delta\log P=-\xi/H_P$. The [buoyancy](../../../../../../buoyancy.md) acceleration is therefore $\ddot\xi=-N^2\xi$, with [stellar buoyancy frequency](../../../../../../stellar-buoyancy-frequency.md)

$$
N^2=\frac g{H_P}[\delta(\nabla_{\rm ad}-\nabla)+\phi\nabla_\mu].
$$

A negative $N^2$ amplifies the displacement. For a radiative background, $\nabla=\nabla_{\rm rad}$, so the [Ledoux criterion](../../../../../../ledoux-criterion.md) for instability is

$$
\boxed{\nabla_{\rm rad}>\nabla_{\rm ad}+\frac\phi\delta\nabla_\mu.}
$$

For uniform composition, $\nabla_\mu=0$, giving the [Schwarzschild criterion](../../../../../../schwarzschild-criterion.md)

$$
\boxed{\nabla_{\rm rad}>\nabla_{\rm ad}.}
$$

Equality is marginal stability. A [mean molecular weight](../../../../../../mean-molecular-weight.md) increasing inward has $\nabla_\mu>0$ and supplies a stabilizing composition term when $\phi,\delta>0$.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 317](../../../paper-317-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
