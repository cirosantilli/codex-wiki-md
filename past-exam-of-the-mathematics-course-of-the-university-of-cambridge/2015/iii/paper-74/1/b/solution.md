<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For a two-dimensional [internal gravity wave](../../../../../../internal-wave.md) with fixed horizontal [wave number](../../../../../../wavenumber.md) $k\ne0$, the vertical [velocity](../../../../../../velocity.md) amplitude satisfies

$$
\widehat w_{zz}+m(z)^2\widehat w=0,\qquad m(z)^2=k^2\left(\frac{N(z)^2}{\omega^2}-1\right).
$$

This follows from the [Linearized Boussinesq equations](../../../../../../linearized-boussinesq-equations.md) just as in part (a), allowing the background [buoyancy frequency](../../../../../../buoyancy-frequency.md) to vary. The [WKB approximation](../../../../../../wkb-approximation.md) gives locally

$$
\widehat w\simeq\frac{A_\pm}{\sqrt{|m(z)|}}\exp\!\left(\pm i\int^z m(s)\,ds\right).
$$

It requires slowly varying stratification compared with the local vertical [wavelength](../../../../../../wavelength.md), in particular $|m_z|\ll m^2$, and a small-amplitude wave in the inviscid, nonrotating regime. Propagation requires $N>|\omega|$; where $N<|\omega|$, the local vertical [wave number](../../../../../../wavenumber.md) is imaginary and the solution is evanescent. Turning levels and abrupt changes need a separate connection calculation. Finite [viscosity](../../../../../../dynamic-viscosity.md), background flow, rotation or nonlinear effects require modifications of this model.

The [ray tracing](../../../../../../ray-tracing.md) equations use the local [dispersion relation](../../../../../../dispersion-relation.md) as a [Hamiltonian](../../../../../../hamiltonian.md):

$$
\dot x=\partial_k\omega,\qquad \dot z=\partial_m\omega,\qquad \dot k=0,\qquad \dot m=-\partial_z\omega.
$$

The stationary, horizontally uniform background conserves the [frequency](../../../../../../frequency.md) and horizontal [wave number](../../../../../../wavenumber.md). In two dimensions the [group velocity](../../../../../../group-velocity.md) gives $dx/dz=-m/k$. For the specified [buoyancy frequency](../../../../../../buoyancy-frequency.md) and $\omega=1$, $m^2=256k^2z^2$. Hence for $z>0$ the two geometric [internal-wave rays](../../../../../../internal-wave-ray-tracing.md) through the specified point are

$$
\boxed{x=8(z^2-1)\quad\hbox{or}\quad x=-8(z^2-1).}
$$

Each curve has both directed propagation senses, giving four local directed rays. Their formal intersections with $z=0$ are $x=-8$ and $x=8$.

At $z=0$, $N=\omega$ and $m=0$: this is a [double-zero internal-wave turning level](../../../../../../double-zero-internal-wave-turning-level.md), since $m^2$ touches zero without changing sign. The ray becomes vertical geometrically, but its [group velocity](../../../../../../group-velocity.md) tends to zero. Taking $k>0$ without loss of generality, the downward branch has

$$
|c_{g,z}|=\frac{16z}{|k|(1+256z^2)},\qquad
\Delta t=\frac{|k|}{16}\log\frac{z_i}{z}+8|k|(z_i^2-z^2).
$$

The formal travel time diverges logarithmically as $z\to0$. Meanwhile $|m_z|/m^2=1/(16|k|z^2)$ grows, so the [WKB approximation](../../../../../../wkb-approximation.md) fails before that limit; its predicted $|m|^{-1/2}$ amplitude cannot be extrapolated to infinity. **The spatial ray reaches a finite limiting position, but finite-wavelength behaviour near the zero must be found beyond WKB.** There is no evanescent half-space supplied by this particular $N(z)$, so ordinary simple-turning-point reflection cannot be assumed solely from the local ray construction.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 74](../../../paper-74-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
