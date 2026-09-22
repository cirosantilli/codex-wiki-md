# Dot product

↑ **Parent:** [Inner product](inner-product.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Dot_product)

A [dot product](dot-product.md) measures how much two [Euclidean vectors](euclidean-vector.md) point along each other. This article uses real [Euclidean vectors](euclidean-vector.md) in $\mathbb R^n$, with the usual [Cartesian basis](cartesian-basis.md): multiply matching coordinates and add,

$$
\mathbf a\cdot\mathbf b=\sum_{i=1}^n a_i b_i,\qquad
\|\mathbf a\|=\sqrt{\mathbf a\cdot\mathbf a}.
$$

The result is a [scalar](scalar.md), while $\|\mathbf a\|$ is the [Euclidean norm](euclidean-norm.md). This real convention has no [complex conjugation](complex-conjugation.md); for [vectors](vector.md) over the [complex numbers](complex-number.md), use the convention specified in [inner product](inner-product.md).

For two nonzero [Euclidean vectors](euclidean-vector.md), the same [dot product](dot-product.md) records their [angle](angle.md) $0\leq\theta\leq\pi$ through the [cosine](cosine.md):

$$
\mathbf a\cdot\mathbf b=\|\mathbf a\|\|\mathbf b\|\cos\theta,\qquad
\theta=\arccos\frac{\mathbf a\cdot\mathbf b}{\|\mathbf a\|\|\mathbf b\|}.
$$

Here $\arccos$ is an [inverse trigonometric function](inverse-trigonometric-functions.md). The [Cauchy-Schwarz inequality](cauchy-schwarz-inequality.md) guarantees that the normalized ratio lies in $[-1,1]$. The [zero vector](zero-vector.md) has [dot product](dot-product.md) zero with every [vector](vector.md), but its [angle](angle.md) is undefined: the ratio would divide by zero. To outline the geometric identity, expand $\|\mathbf a-\mathbf b\|^2=\|\mathbf a\|^2+\|\mathbf b\|^2-2\mathbf a\cdot\mathbf b$ and compare with the [law of cosines](law-of-cosines.md).[OpenStax, Calculus Volume 3, §2.3: the dot product and angles](https://openstax.org/books/calculus-volume-3/pages/2-3-the-dot-product)

Take $\mathbf a=(3,4)$ and $\mathbf c=(2,0)$. Their [Euclidean norms](euclidean-norm.md) are $5$ and $2$, and

$$
\mathbf a\cdot\mathbf c=3(2)+4(0)=6,\qquad
\cos\theta=\frac{6}{5\cdot2}=\frac35,\qquad
\theta=\arccos(3/5)\approx53.1301^\circ.
$$

The [unit vector](unit-vector.md) $\mathbf u=\mathbf c/\|\mathbf c\|=(1,0)$ selects the horizontal direction. The [scalar projection](scalar-projection.md) $\mathbf a\cdot\mathbf u=3$ says how far $\mathbf a$ reaches along that direction; its [vector projection](vector-projection.md) is $3\mathbf u=(3,0)$. Thus $\mathbf a=(3,0)+(0,4)$ splits into an aligned part and an [orthogonal projection residual](orthogonal-projection-residual.md).

<a id="image-the-vector-projection-of-3-4-onto-the-horizontal-line-is-3-0-the-orthogonal-projection-residual-is-0-4-and-the-angle-is-53-1301-circ"></a>
![](dot-product-projection-and-angle.png)

**[Figure 43](#image-the-vector-projection-of-3-4-onto-the-horizontal-line-is-3-0-the-orthogonal-projection-residual-is-0-4-and-the-angle-is-53-1301-circ). The vector projection of $(3,4)$ onto the horizontal line is $(3,0)$; the orthogonal projection residual is $(0,4)$ and the angle is $53.1301^\circ$**.

For $\mathbf b=(4,-3)$, the [dot product](dot-product.md) $\mathbf a\cdot\mathbf b=12-12=0$ proves [orthogonality](orthogonal-vectors.md); both [Euclidean norms](euclidean-norm.md) are $5$. For $\mathbf d=(-2,0)$, $\mathbf a\cdot\mathbf d=-6$: the [scalar projection](scalar-projection.md) onto $\mathbf d/\|\mathbf d\|=(-1,0)$ is $-3$, because $\mathbf a$ reaches against that chosen direction. Its [angle](angle.md) with $\mathbf d$ is $126.8699^\circ$.

Keeping $\mathbf a=(3,4)$ fixed and choosing $\mathbf b$ of [Euclidean norm](euclidean-norm.md) $2$ gives $\mathbf a\cdot\mathbf b=10\cos\theta$. At [angles](angle.md) $0^\circ,60^\circ,90^\circ,120^\circ,180^\circ$, the [dot products](dot-product.md) are $10,5,0,-5,-10$. Positive values mean partial alignment, zero means [orthogonality](orthogonal-vectors.md), and negative values mean a component against the other direction.

<a id="image-with-euclidean-norms-5-and-2-the-dot-product-follows-10-cos-theta-equal-length-arrows-show-positive-zero-and-negative-alignment-with-3-4"></a>
![](dot-product-angle-sign.png)

**[Figure 44](#image-with-euclidean-norms-5-and-2-the-dot-product-follows-10-cos-theta-equal-length-arrows-show-positive-zero-and-negative-alignment-with-3-4). With Euclidean norms $5$ and $2$, the dot product follows $10\cos\theta$; equal-length arrows show positive, zero, and negative alignment with $(3,4)$**.

This interpretation explains [work](work.md): for a constant [force](force.md) $\mathbf F$ and a straight [displacement](displacement.md) $\mathbf s$, $W=\mathbf F\cdot\mathbf s$ counts the [force](force.md) component along the motion. A sideways [force](force.md) contributes zero [work](work.md), and an opposing [force](force.md) contributes negative [work](work.md).[OpenStax, §2.3: work](https://openstax.org/books/calculus-volume-3/pages/2-3-the-dot-product)

**Table of contents**

- [Scalar projection](scalar-projection.md)
- [Vector projection](vector-projection.md)

## ↑ Ancestors (6)

1. [Inner product](inner-product.md)
2. [Linear algebra](linear-algebra-split.md)
3. [Algebra](algebra-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (151)

- [Acceleration](acceleration.md)
- [Active planar rotation](active-planar-rotation.md)
- [Altitude](altitude.md)
- [Areal velocity](areal-velocity.md)
- [Bilinear form](bilinear-form.md)
- [Bond angle](bond-angle.md)
- [Central angle between independent uniform sphere points](central-angle-between-independent-uniform-sphere-points.md)
- [Conic dual problem](conic-dual-problem.md)
- [Conic primal-dual gap](conic-primal-dual-gap.md)
- [Convex conjugate](convex-conjugate.md)
- [Coordinate (linear algebra)](coordinate-linear-algebra.md)
- [Cross-product Lie algebra](cross-product-lie-algebra.md)
- [Current density](current-density.md)
- [Curvature](curvature.md)
- [Declination](declination.md)
- [Derivative along a curve](derivative-along-a-curve.md)
- [Dot product](dot-product.md)
- [Dot-product gradient identity](dot-product-gradient-identity.md)
- [Dual basis](dual-basis.md)
- [Duality of primitive cyclic Reed-Solomon codes](duality-of-primitive-cyclic-reed-solomon-codes.md)
- [Electric dipole](electric-dipole.md)
- [Electric flux](electric-flux.md)
- [Elsässer energy invariant](elsasser-energy-invariant.md)
- [Euclidean geometry](euclidean-geometry.md)
- [Eventown theorem](eventown-theorem.md)
- [Farkas' lemma](farkas-lemma.md)
- [Fenchel–Young inequality](fenchel-young-inequality.md)
- [Finite-dimensional spectral theorem](finite-dimensional-spectral-theorem.md)
- [Gabor filter](gabor-filter.md)
- [Gram-Schmidt process](gram-schmidt-process.md)
- [Gyroscope vector geometry](gyroscope-vector-geometry.md)
- [Hadamard transform](hadamard-transform.md)
- [Heath-Jarrow-Morton model](heath-jarrow-morton-model.md)
- [Hermitian inner product](hermitian-inner-product.md)
- [Horizontal coordinate system](horizontal-coordinate-system.md)
- [Inertia tensor](inertia-tensor.md)
- [Interference (wave propagation)](interference-wave-propagation.md)
- [Investment portfolio](investment-portfolio.md)
- [Kinetic energy](kinetic-energy.md)
- [Local Joule heating rate](local-joule-heating-rate.md)
- [Local wavelength](local-wavelength.md)
- [Lorentz force](lorentz-force.md)
- [Lunar phase](lunar-phase.md)
- [Magnetic dipole torque](magnetic-dipole-torque.md)
- [Magnetic flux](magnetic-flux.md)
- [Magnetic helicity](magnetic-helicity.md)
- [Malus's law](malus-s-law.md)
- [Matrix determinant lemma](matrix-determinant-lemma.md)
- [Mutual inclination of nearly edge-on orbits](mutual-inclination-of-nearly-edge-on-orbits.md)
- [Nanson's formula](nanson-s-formula.md)
- [Normal vector](normal-vector.md)
- [Oddtown theorem](oddtown-theorem.md)
- [Orbital-frame rotation from inclination and node](orbital-frame-rotation-from-inclination-and-node.md)
- [Orthogonal opposite edges of a tetrahedron](orthogonal-opposite-edges-of-a-tetrahedron.md)
- [Orthogonal projection onto a finite-dimensional subspace](orthogonal-projection-onto-a-finite-dimensional-subspace.md)
- [Orthogonal projection residual](orthogonal-projection-residual.md)
- [Orthogonal vectors](orthogonal-vectors.md)
- [Orthogonality of hypercube body diagonals](orthogonality-of-hypercube-body-diagonals.md)
- [Paired coordinates of a symplectic basis](paired-coordinates-of-a-symplectic-basis.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/ia/paper-1/1c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ia/paper-1/8d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ia/paper-3/11a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ia/paper-3/12a/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ia/paper-3/5e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ia/paper-3/6e/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ia/paper-3/6e/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-30/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-49/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/ia/paper-1/5b/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/ia/paper-1/5b/b/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/ia/paper-1/8d/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/ia/paper-1/8d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/ia/paper-3/11a/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/ia/paper-3/5e/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/ia/paper-3/6e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/ia/paper-3/9a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/ia/paper-4/4e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-36/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-70/1/c/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/ia/paper-1/2c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/ia/paper-1/8c/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-2/6/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-70/1/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ia/paper-1/7a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ia/paper-3/3a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-87/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-66/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ia/paper-1/1a/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ia/paper-1/5b/i/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ia/paper-1/7c/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ia/paper-2/12f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-53/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ia/paper-1/5b/a/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ia/paper-1/5b/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ia/paper-1/5b/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ia/paper-1/7c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-77/1/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ia/paper-1/5c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ib/paper-2/12g/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-14/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-2/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ia/paper-1/6c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-61/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2011/ia/paper-1/5c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2011/ia/paper-3/3c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/ia/paper-1/6a/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-38/6/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ia/paper-1/2c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ia/paper-1/5b/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-63/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-63/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ia/paper-1/5a/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ia/paper-1/6b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-109/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-314/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-314/1/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-338/1/a/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ia/paper-1/5c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-3/8b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-316/1/i/solution.md)
- [Positive-weight expectation cone](positive-weight-expectation-cone.md)
- [Power method](power-method.md)
- [Poynting theorem](poynting-theorem.md)
- [Projected area](projected-area.md)
- [Radiant flux through an oriented surface](radiant-flux-through-an-oriented-surface.md)
- [Rank-nullity theorem](rank-nullity-theorem.md)
- [Rank-one matrix update](rank-one-matrix-update.md)
- [Right circular conical surface](right-circular-conical-surface.md)
- [Right-triangle geometry of internal-wave velocities](right-triangle-geometry-of-internal-wave-velocities.md)
- [Rotation matrix](rotation-matrix.md)
- [Second-order-cone optimality certificate](second-order-cone-optimality-certificate.md)
- [Self-dual code](self-dual-code.md)
- [Signed spatial filter model of a simple cell](signed-spatial-filter-model-of-a-simple-cell.md)
- [Simple cell](simple-cell.md)
- [Specular reflection](specular-reflection.md)
- [Spherical geometry](spherical-geometry.md)
- [Spherical law of cosines](spherical-law-of-cosines.md)
- [Spherical trigonometry](spherical-trigonometry.md)
- [Tangent plane](tangent-plane.md)
- [Tetrahedral molecular geometry](tetrahedral-molecular-geometry.md)
- [Torque](torque.md)
- [Two-particle relative coordinate](two-particle-relative-coordinate.md)
- [Unit normal](unit-normal.md)
- [Valence shell electron pair repulsion theory](valence-shell-electron-pair-repulsion-theory.md)
- [Vector projection](vector-projection.md)
- [Virial theorem](virial-theorem.md)
- [Virial theorem derivation and history](virial-theorem-derivation-and-history.md)
- [Wavenumber](wavenumber.md)
- [Work](work.md)
- [Work done by a constant force](work-done-by-a-constant-force.md)
- [Work-energy theorem](work-energy-theorem.md)
