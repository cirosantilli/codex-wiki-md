<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use the coefficients in the authoritative PDF, including their factor $i$. Write $a=2\sqrt3\,i$ and

$$
R(z)=\frac{z^4+az^2+1}{z^4-az^2+1},\qquad\omega=e^{2\pi i/3}.
$$

The numerator and denominator are coprime: a common zero would, by subtraction, require $z=0$, where both equal one. Therefore the [degree of a rational map of the Riemann sphere](../../../../../../degree-of-a-rational-map-of-the-riemann-sphere.md) is four. Direct algebra gives

$$
\boxed{R(iz)=\frac1{R(z)},\qquad
R\!\left(\frac{iz+1}{1-iz}\right)=\omega R(z),\qquad R(1/z)=R(z).}
$$

The domain transformations $z\mapsto iz$ and $z\mapsto(iz+1)/(1-iz)$ are [sphere rotations as special-unitary Möbius transformations](../../../../../../sphere-rotations-as-special-unitary-mobius-transformations.md): respectively a quarter-turn about the third axis and a one-third turn cycling the three coordinate axes. In particular the latter sends $0\mapsto1\mapsto i\mapsto0$, the north, first-axis and second-axis directions. They generate the order-24 [rotational symmetry group of a cube](../../../../../../rotational-symmetry-group-of-a-cube.md), isomorphic to the [symmetric group](../../../../../../symmetric-group.md) $S_4$. Their target transformations are rotations: $w\mapsto1/w$ is a half-turn about the first target axis and $w\mapsto\omega w$ is a one-third turn about the third target axis. This proves whole-map combined equivariance, not just symmetry of selected roots.

The target rotation image is the order-six [dihedral group](../../../../../../dihedral-group.md) $D_3$. The spatial half-turns about all three coordinate axes act trivially on the map: $R(-z)=R(z)$ and $R(1/z)=R(z)$ generate a [Klein four-group](../../../../../../klein-four-group.md) kernel. Thus the full [Skyrmion](../../../../../../skyrmion.md) symmetry combines the spatial cubic rotations with compensating [isospin rotations](../../../../../../isorotation.md), while its angular energy and [Skyrme baryon density](../../../../../../skyrme-baryon-density.md) have pure spatial cubic symmetry.

The critical directions make the geometry explicit. Its [Wronskian of a rational map](../../../../../../wronskian-of-a-rational-map.md) is

$$
p'q-pq'=4az(1-z^4)=8\sqrt3\,i\,z(1-z^4).
$$

The five finite [ramification points](../../../../../../ramification-point-of-a-holomorphic-map.md) are $0,\pm1,\pm i$; infinity supplies the sixth, since in the local coordinate $w=1/z$ the map starts with $R=1+2aw^2+O(w^4)$. These are the six coordinate-axis directions, or face centres of a [cube](../../../../../../cube.md). The [angular Jacobian of a rational map](../../../../../../angular-jacobian-of-a-rational-map.md) vanishes there, consistent with a cube-shaped shell whose density is concentrated away from its face centres. Any further rotational equivariance would have to preserve this set, so the spatial proper rotation group is exactly the cubic group already generated above.

There is also a reflection relation $R(\overline z)=1/\overline{R(z)}$. Together with the proper rotations, it makes the angular density invariant under the full order-48 [symmetry group of a cube](../../../../../../symmetry-group-of-a-cube.md), usually denoted $O_h$. The target operation in this reflection relation is orientation reversing; it should not be mistaken for a proper [isospin rotation](../../../../../../isorotation.md). In the full [Skyrme model](../../../../../../skyrme-model.md), reflections are expressed using the field parity operation $U(\mathbf x)\mapsto U^\dagger(-\mathbf x)$ together with a compensating [isospin rotation](../../../../../../isorotation.md).

**This is the cubic charge-four rational-map ansatz**:

$$
\boxed{\deg R=B=4,\qquad\text{proper spatial symmetry }O\cong S_4,\qquad\text{density symmetry }O_h.}
$$

The [cubic rational-map ansatz for four Skyrmions](../../../../../../cubic-rational-map-ansatz-for-four-skyrmions.md) is a useful approximation and starting point for the [cubic four-Skyrmion](../../../../../../cubic-four-skyrmion.md), whose lowest spin-zero, isospin-zero quantized state models an [alpha particle](../../../../../../alpha-particle.md). A radial minimization and, for precision, unrestricted field relaxation are still required. The TeX's missing $i$ changes this map; the six critical directions alone would not detect the error, because the same Wronskian zero set persists when $a$ is real. The actual rotational equivariance identities are the stronger check.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 308](../../../paper-308-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
