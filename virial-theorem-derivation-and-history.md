# Virial theorem derivation and history

↑ **Parent:** [Virial theorem](virial-theorem.md)

The proof is a single [time derivative](time-derivative.md). Apply the [product rule](product-rule.md) to each [dot product](dot-product.md) and use [Newton's second law](newton-s-second-law.md):

$$
\dot G=\sum_i\dot{\mathbf p}_i\cdot\mathbf r_i+\sum_i\mathbf p_i\cdot\dot{\mathbf r}_i
=\sum_i\mathbf F_i\cdot\mathbf r_i+2K.
$$

Integrating from $0$ to $T$ gives the endpoint identity; the stated sublinear condition removes the endpoint term only in the infinite-[time](time-in-physics.md) limit. Equivalently, for the scalar inertia $I=\tfrac12\sum_i m_i|\mathbf r_i|^2$ used in the [pairwise moment-of-inertia identity](pairwise-moment-of-inertia-identity.md), $\dot I=G$ and $\ddot I=2K+\sum_i\mathbf r_i\cdot\mathbf F_i$. Specifying this factor of one half avoids confusion with another common inertia convention.

In [On a Mechanical Theorem applicable to Heat by R. Clausius](on-a-mechanical-theorem-applicable-to-heat-by-r-clausius.md) (1870, pp. 123-124), the author defines stationary motion through bounded [positions](position.md) and [velocities](velocity.md), includes planetary [orbits](orbit-dynamical-system.md) and elastic vibrations, and names the average negative half of the force-position sum the “virial”. That historical convention differs from the auxiliary $G(t)$ defined above. His proof on pp. 126-127 keeps an endpoint term, then explains why it vanishes over a complete period or becomes small in a long bounded irregular motion. The same paper separates internal and external [forces](force.md) and includes uniform boundary [pressure](pressure.md) on pp. 125-126: confinement was already part of the formulation, rather than a reason to omit external stresses.[On a Mechanical Theorem applicable to Heat by R. Clausius (1870), pp. 123-127; p. 122 footnote dates the lecture to 13 June 1870](on-a-mechanical-theorem-applicable-to-heat-by-r-clausius.md)

## ↑ Ancestors (5)

1. [Virial theorem](virial-theorem.md)
2. [Classical mechanics](classical-mechanics-split.md)
3. [Branches of physics](branches-of-physics.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)
