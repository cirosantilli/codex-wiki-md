<h1 id="16h/solution">Solution</h1>

↑ **Parent:** [16H](../16h.md)

Fix the [electric potential](../../../../../electric-potential.md) to vanish at infinity and assume a localized, nonsingular [charge density](../../../../../charge-density.md) of finite [electrostatic energy](../../../../../electrostatic-energy.md). Assemble the charge by scaling $\rho_s=s\rho$ from $s=0$ to $1$. Linearity gives $\phi_s=s\phi$, so the work is

$$
U=\int_0^1ds\int\phi_s\rho\,d^3x
=\frac12\int\rho\phi\,d^3x.
$$

The factor $1/2$ prevents double counting of pair interactions. Using [Gauss law](../../../../../gauss-s-law.md), $\rho=-\epsilon_0\Delta\phi$, and [integration by parts](../../../../../integration-by-parts.md),

$$
U=-\frac{\epsilon_0}2\int\phi\Delta\phi\,d^3x
=\boxed{\frac{\epsilon_0}2\int|\nabla\phi|^2\,d^3x
=\frac{\epsilon_0}2\int|\mathbf E|^2\,d^3x}.
$$

The boundary integral at infinity vanishes for a localized distribution since $\phi=O(r^{-1})$ and $\partial_r\phi=O(r^{-2})$. Singular point-charge self-energies require a separate regularization and are not finite instances of this identity.

For the uniform solid sphere, spherical symmetry and [Gauss law](../../../../../gauss-s-law.md) give

$$
\boxed{\mathbf E(r)=
\begin{cases}
\dfrac{\rho r}{3\epsilon_0}\,\widehat{\mathbf r},&0\le r\le R,\\[2pt]
\dfrac{\rho R^3}{3\epsilon_0r^2}\,\widehat{\mathbf r},&r\ge R.
\end{cases}}
$$

Integrating inward from infinity and matching the continuous [electric potential](../../../../../electric-potential.md) at $R$ gives

$$
\boxed{\phi(r)=
\begin{cases}
\dfrac{\rho}{6\epsilon_0}(3R^2-r^2),&r\le R,\\[2pt]
\dfrac{\rho R^3}{3\epsilon_0r},&r\ge R.
\end{cases}}
$$

The value of the [electric field](../../../../../electric-field.md) at the centre is the zero vector.

Writing $Q=4\pi\rho R^3/3$, the [electrostatic energy of a uniformly charged solid sphere](../../../../../electrostatic-energy-of-a-uniformly-charged-solid-sphere.md) follows either from the charge-potential integral or from the field integral including the exterior:

$$
U=\frac12\,4\pi\rho\int_0^R\phi(r)r^2\,dr
=\boxed{\frac{4\pi\rho^2R^5}{15\epsilon_0}
=\frac{3Q^2}{20\pi\epsilon_0R}}.
$$

For the nuclear scaling, $Q=Ze$ while constant volume per proton gives $R\propto Z^{1/3}$. Therefore **the electric contribution scales as $Q^2/R\propto Z^{5/3}$** in this uniform-density model.

## ↑ Ancestors (10)

1. [16H](../16h.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
