# Exact tidal acceleration between separated masses

↑ **Parent:** [Tidal force](tidal-force.md)

Stipulate a fixed source [point mass](point-mass.md) $M=10^{12}\,\mathrm{kg}$, two equal [test particles](test-particle.md) of [mass](mass.md) $m=1\,\mathrm{kg}$, and $G=6.67430\times10^{-11}\,\mathrm{m^3\,kg^{-1}\,s^{-2}}$. This is a chosen model, not a measurement of a particular object. Place the [test particles](test-particle.md) on the outward radial axis at $R-L/2$ and $R+L/2$, with midpoint distance $R=100\,\mathrm m$ and separation $L=2\,\mathrm m$. Neglect their mutual attraction, other sources and all supporting [forces](force.md).

Each signed radial [gravitational acceleration](gravitational-acceleration.md) is inward:

$$
a_-=-\frac{\mu}{(R-L/2)^2}\approx-0.0068098153\,\mathrm{m\,s^{-2}},\qquad a_+=-\frac{\mu}{(R+L/2)^2}\approx-0.0065427899\,\mathrm{m\,s^{-2}}.
$$

Their separation has outward relative [acceleration](acceleration.md)

$$
\ddot L=a_+-a_-=\mu\left[\frac{1}{(R-L/2)^2}-\frac{1}{(R+L/2)^2}\right]=\frac{2\mu L}{R^3}\left(1-\frac{L^2}{4R^2}\right)^{-2}.
$$

The exact value is $2.6702540\times10^{-4}\,\mathrm{m\,s^{-2}}$. The midpoint [tidal tensor](tidal-tensor.md) predicts $2\mu L/R^3=2.6697200\times10^{-4}\,\mathrm{m\,s^{-2}}$, an underestimate of $0.019999\%$ relative to the exact value. For these equal $1\,\mathrm{kg}$ [masses](mass.md), the difference of external [forces](force.md) has the same numerical value in the [SI](international-system-of-units.md) unit of [force](force.md), the [newton](newton-unit.md). It is not an additional mutual [force](force.md) between the [test particles](test-particle.md).

The exact formula requires $L<2R$ and describes the instantaneous relative [acceleration](acceleration.md). Because the two sample [positions](position.md) are symmetric about the midpoint, the [Taylor expansion](taylor-expansion.md) error relative to the linear result starts at order $(L/R)^2$; a one-sided comparison with a reference point generally has relative error of order $L/R$. If either [test particle](test-particle.md) enters an extended source, use that source's interior [Newtonian gravitational field](newtonian-gravitational-field.md) instead of extrapolating the singular [point mass](point-mass.md) model.

## ↑ Ancestors (8)

1. [Tidal force](tidal-force.md)
2. [Tidal tensor](tidal-tensor.md)
3. [Newtonian gravitational field](newtonian-gravitational-field.md)
4. [Newton's law of universal gravitation](newton-s-law-of-universal-gravitation.md)
5. [Classical mechanics](classical-mechanics-split.md)
6. [Branches of physics](branches-of-physics.md)
7. [Physics](physics-split.md)
8. [Codex Wiki](split.md)
