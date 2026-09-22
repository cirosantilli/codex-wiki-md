<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

For an isolated smooth mass distribution with [spherical symmetry](../../../../../spherical-symmetry.md), assemble each shell $dM$ at radius $r$ against the [Newtonian gravitational potential](../../../../../newtonian-gravitational-potential.md) of its interior mass. The [spherical shell theorem](../../../../../spherical-shell-theorem.md) gives

$$
W=-G\int_0^\infty\frac{M(r)}r\,dM(r)=-\frac G2\int_0^\infty\frac1r\,d[M(r)^2].
$$

Assume finite total mass, finite binding energy and no central point-mass self-energy, so $M(r)^2/r$ vanishes at both endpoints. [Integration by parts](../../../../../integration-by-parts.md) then gives

$$
\boxed{W=-\frac G2\int_0^\infty\frac{M(r)^2}{r^2}\,dr.}
$$

For example, $M(r)\propto r^3$ near a regular center guarantees the central boundary condition, while finite total mass guarantees the one at infinity. A divergent central binding energy would fall outside this formula's finite-energy hypotheses.

For the discrete system use the [centre of mass](../../../../../center-of-mass.md) frame, let $N$ be the particle number, and write $M_{\rm tot}=Nm$. The printed $M$ in the particle-count factor and the subsequent $n$ must be understood consistently as $N$. Define

$$
K=\frac12\sum_i m|\dot{\mathbf r}_i|^2,\qquad
W=-Gm^2\sum_{i<j}\frac1{r_{ij}},\qquad
I=\sum_i m|\mathbf r_i|^2.
$$

By [Newton's second law](../../../../../newton-s-second-law.md), differentiation gives

$$
\frac12\ddot I=2K+\sum_i\mathbf r_i\cdot\mathbf F_i.
$$

Each pair contributes

$$
\mathbf r_i\cdot\mathbf F_{ij}+\mathbf r_j\cdot\mathbf F_{ji}
=(\mathbf r_i-\mathbf r_j)\cdot\left[-Gm^2\frac{\mathbf r_i-\mathbf r_j}{r_{ij}^3}\right]
=-\frac{Gm^2}{r_{ij}}.
$$

Therefore the exact dynamical [virial theorem](../../../../../virial-theorem.md) is $\ddot I/2=2K+W$. In a stationary statistical state, or on a bounded-motion time average for which the mean $\ddot I$ vanishes, it becomes

$$
\boxed{2\langle K\rangle+\langle W\rangle=0.}
$$

There is no external pressure, tidal field or boundary work in this isolated point-particle derivation. For a time-averaged system, the following $W$ and [gravitational radius](../../../../../gravitational-radius.md) refer to that same averaged binding energy.

Using $W=-G(Nm)^2/R_g$ and $2K=Nm\langle v_{\rm eq}^2\rangle$, [virial equilibrium](../../../../../virial-equilibrium.md) gives

$$
\boxed{\langle v_{\rm eq}^2\rangle=\frac{GNm}{R_g},\qquad v_{{\rm eq},{\rm rms}}=\sqrt{\frac{GNm}{R_g}}.}
$$

This is the three-dimensional mean squared speed about the [centre of mass](../../../../../center-of-mass.md). For an isotropic system each one-dimensional [velocity dispersion](../../../../../velocity-dispersion.md) squared is one third of it.

Set the [Newtonian gravitational potential](../../../../../newtonian-gravitational-potential.md) to zero at infinity and exclude each particle's own field. The local [escape velocity](../../../../../escape-velocity.md) in the instantaneous frozen potential obeys $v_{{\rm esc},i}^2=-2\Phi_i$, where $\Phi_i=-Gm\sum_{j\ne i}r_{ij}^{-1}$. Since every pair occurs twice, $\sum_i m\Phi_i=2W$. Averaging over the identical particles proves the [gravitational rms escape and collapse speeds](../../../../../gravitational-rms-escape-and-collapse-speeds.md) relation

$$
\boxed{\langle v_{\rm esc}^2\rangle=-\frac{4W}{Nm}=\frac{4GNm}{R_g}=4\langle v_{\rm eq}^2\rangle,\qquad v_{{\rm esc},{\rm rms}}=2v_{{\rm eq},{\rm rms}}.}
$$

An actual encounter in a changing potential can exchange energy, so this is the usual local escape-speed definition, not a claim about every many-body trajectory.

Finally, dissipation-free collapse from rest at infinite separation has total energy zero. [Conservation of energy](../../../../../conservation-of-energy.md) at the specified binding energy therefore gives $K_{\rm coll}=-W$, twice the equilibrium kinetic energy at the same $W$. Hence

$$
\boxed{\langle v_{\rm coll}^2\rangle=\frac{2GNm}{R_g}=2\langle v_{\rm eq}^2\rangle,\qquad v_{{\rm coll},{\rm rms}}=\sqrt2\,v_{{\rm eq},{\rm rms}}.}
$$

This mean squared speed includes coherent infall; a local random [velocity dispersion](../../../../../velocity-dispersion.md) after subtracting the infall velocity need not obey that ratio.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 62](../../paper-62-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
