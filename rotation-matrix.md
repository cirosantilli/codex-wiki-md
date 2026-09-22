# Rotation matrix

↑ **Parent:** [Linear algebra](linear-algebra-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Rotation_matrix)

A rotation matrix is an orthogonal matrix with determinant $1$.

A [rotation matrix](rotation-matrix.md) turns [vectors](vector.md) while preserving their shape relationships. For column [coordinate vectors](coordinate-vector.md) in an [orthonormal basis](orthonormal-basis.md), its defining conditions are

$$
R^TR=I,\qquad \det R=1,
$$

where $R^T$ is the [transpose](transpose.md) and $I$ the [identity matrix](identity-matrix.md). In the usual [Cartesian basis](cartesian-basis.md) of the [plane](plane.md), an active counterclockwise [planar rotation](planar-rotation.md) through an [angle](angle.md) $\theta$ uses

$$
R_\theta=\begin{pmatrix}\cos\theta&-\sin\theta\\\sin\theta&\cos\theta\end{pmatrix},\qquad v'=R_\theta v.
$$

Here the [vector](vector.md) moves and the [basis](basis.md) stays fixed: $R_{\pi/2}(1,0)^T=(0,1)^T$. Positive [angles](angle.md) turn from the positive horizontal axis towards the positive vertical axis. The two columns are precisely the rotated [basis vectors](basis-vector.md); the [sine](sine.md) and [cosine](cosine.md) entries encode their new directions. Turning the [basis](basis.md) instead uses [passive rotation of coordinates](passive-rotation-of-coordinates.md), which has the opposite sign.

This distinction makes [rotation matrices](rotation-matrix.md) useful for keeping a geometric action separate from its coordinate description. For a [rigid body](rigid-body-dynamics-split.md), a [rotation matrix](rotation-matrix.md) can encode the directions of an attached [orthonormal basis](orthonormal-basis.md) or convert between that [basis](basis.md) and a fixed [orthonormal basis](orthonormal-basis.md), with different meanings for its input and output.[Modern Robotics, §3.2.1.2, preprint p. 69: three uses of a rotation matrix](modern-robotics-mechanics-planning-and-control-by-kevin-m-lynch-and-frank-c-park.md)

The [orthogonal matrix](orthogonal-matrix.md) condition preserves every [dot product](dot-product.md):

$$
(Ru)\cdot(Rv)=(Ru)^T(Rv)=u^TR^TRv=u\cdot v.
$$

Consequently [Euclidean norms](euclidean-norm.md) and [angles](angle.md) between nonzero [vectors](vector.md) are preserved, as is the [Euclidean norm](euclidean-norm.md) of the difference between any two endpoints. The additional [determinant](determinant.md) condition preserves [orientation of a vector space](orientation-of-a-vector-space.md) and [oriented volume](oriented-volume.md): for any square [matrix](matrix.md) $V$ whose columns are the input [vectors](vector.md), $\det(RV)=\det V$. An [orthogonal matrix](orthogonal-matrix.md) of [determinant](determinant.md) $-1$, such as a [reflection matrix](reflection-matrix.md), preserves [dot products](dot-product.md) but reverses [orientation of a vector space](orientation-of-a-vector-space.md). The [matrix inverse](matrix-inverse-split.md) is especially simple: $R^{-1}=R^T$.[Modern Robotics, §3.2.1, definition 3.1 and propositions 3.3–3.6, preprint pp. 67–69](modern-robotics-mechanics-planning-and-control-by-kevin-m-lynch-and-frank-c-park.md)

**Table of contents**

- [Euler-Rodrigues formula](euler-rodrigues-formula.md)
- [Real rotation matrices that are Hermitian](real-rotation-matrices-that-are-hermitian.md)
- [Passive rotation of coordinates](passive-rotation-of-coordinates.md)
- [Composition of rotation matrices](composition-of-rotation-matrices.md)
  - [Noncommuting rotations about fixed axes](noncommuting-rotations-about-fixed-axes.md)
- [Trace of a three-dimensional rotation](trace-of-a-three-dimensional-rotation.md)
- [Planar rotation](planar-rotation.md)
  - [Active planar rotation](active-planar-rotation.md)
  - [Finite groups of planar rotations are cyclic](finite-groups-of-planar-rotations-are-cyclic.md)
- [Centralizer of a planar quarter-turn](centralizer-of-a-planar-quarter-turn.md)
- [Rotational symmetry](rotational-symmetry.md)
  - [Rotational symmetry group of a regular icosahedron](rotational-symmetry-group-of-a-regular-icosahedron.md)
  - [Rotational symmetry group of a regular dodecahedron](rotational-symmetry-group-of-a-regular-dodecahedron.md)

## ↑ Ancestors (5)

1. [Linear algebra](linear-algebra-split.md)
2. [Algebra](algebra-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (103)

- [Calculated transmission Laue pattern](calculated-transmission-laue-pattern.md)
- [Cartesian basis under rotation](cartesian-basis-under-rotation.md)
- [Centralizer of a planar quarter-turn](centralizer-of-a-planar-quarter-turn.md)
- [Composition of rotation matrices](composition-of-rotation-matrices.md)
- [Cross-product Lie algebra](cross-product-lie-algebra.md)
- [Equivariance of isotropic principal stresses](equivariance-of-isotropic-principal-stresses.md)
- [Faraday rotation on a round trip](faraday-rotation-on-a-round-trip.md)
- [Free particle in rotating coordinates](free-particle-in-rotating-coordinates.md)
- [Givens rotation](givens-rotation.md)
- [Helium-3 B phase](helium-3-b-phase.md)
- [Isotropic second-rank tensor](isotropic-second-rank-tensor.md)
- [Isotropic third-rank tensor](isotropic-third-rank-tensor.md)
- [Lie group](lie-group.md)
- [Noncommuting rotations about fixed axes](noncommuting-rotations-about-fixed-axes.md)
- [Orbital-frame rotation from inclination and node](orbital-frame-rotation-from-inclination-and-node.md)
- [Orientation of an orthonormal reciprocal basis](orientation-of-an-orthonormal-reciprocal-basis.md)
- [Orthogonal skew-symmetric matrix](orthogonal-skew-symmetric-matrix.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-47/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ia/paper-3/8b/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/ia/paper-1/5b/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/ia/paper-3/1a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/ia/paper-3/6e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/ib/paper-2/2c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/ib/paper-3/7g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/ia/paper-3/6d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-78/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ia/paper-1/6c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ia/paper-3/12a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ia/paper-3/10c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ib/paper-1/2g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-57/2/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-57/4/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ia/paper-3/1d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ia/paper-3/1d/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ia/paper-3/1d/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2011/ia/paper-1/6a/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2011/ia/paper-3/9c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/ia/paper-1/2a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/ia/paper-3/4c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/ia/paper-3/6e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/ia/paper-1/8b/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-6/4/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/ia/paper-3/12a/b/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ia/paper-1/2c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ia/paper-3/4c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ia/paper-3/4b/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ia/paper-3/7e/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-324/2/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-327/2/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-344/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ia/paper-1/6b/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ia/paper-4/3a/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ii/paper-2/9b/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ia/paper-1/8a/d/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-3/10d/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-324/2/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-3/32c/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ia/paper-1/8b/b/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ia/paper-1/6b/a/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ia/paper-3/12a/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-324/2/b/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2006/paper-1/2/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2016/paper-2/5/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2020/paper-1/18/a/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2021/paper-1/18/d/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2023/paper-1/14/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2025/paper-1/17/f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2025/paper-2/18/c/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2010/paper-2/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2016/paper-2/6/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2021/paper-1/5/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2021/paper-1/5/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2021/paper-1/5/d/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2021/paper-1/5/f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2022/paper-2/6/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2023/paper-2/10/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2023/paper-2/6/b/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2024/paper-2/6/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2024/paper-2/6/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2025/paper-2/6/a/solution.md)
- [Solution](past-exam-of-the-optics-and-electrodynamics-course-of-the-university-of-cambridge/2021/section-b/b4/f/solution.md)
- [Solution](past-exam-of-the-optics-and-electrodynamics-course-of-the-university-of-cambridge/2022/section-b/4/c/solution.md)
- [Planar rotation](planar-rotation.md)
- [Planar rotation as a one-parameter subgroup](planar-rotation-as-a-one-parameter-subgroup.md)
- [Pseudotensor](pseudotensor.md)
- [Pseudovector](pseudovector.md)
- [Pythagorean trigonometric identity](pythagorean-trigonometric-identity.md)
- [Quarter-turn action on diagonal quadratic forms](quarter-turn-action-on-diagonal-quadratic-forms.md)
- [Real rotation matrices that are Hermitian](real-rotation-matrices-that-are-hermitian.md)
- [Rotation invariance of the Levi-Civita symbol](rotation-invariance-of-the-levi-civita-symbol.md)
- [Rotation matrix](rotation-matrix.md)
- [Rotational invariance of the Laplacian](rotational-invariance-of-the-laplacian.md)
- [Rotational invariant of a symmetric traceless tensor](rotational-invariant-of-a-symmetric-traceless-tensor.md)
- [Rotational symmetry](rotational-symmetry.md)
- [Sine addition formula](sine-addition-formula.md)
- [Skew-symmetric exponential as an axial rotation](skew-symmetric-exponential-as-an-axial-rotation.md)
- [Small rotation commutator](small-rotation-commutator.md)
- [Static inhomogeneity refocusing](static-inhomogeneity-refocusing.md)
- [Symmetric and skew-symmetric Cayley transforms](symmetric-and-skew-symmetric-cayley-transforms.md)
- [Torque-free tumbling](torque-free-tumbling.md)
- [Trace of a three-dimensional rotation](trace-of-a-three-dimensional-rotation.md)
- [Triangular-rotation factorization of real determinant-one matrices](triangular-rotation-factorization-of-real-determinant-one-matrices.md)
- [Two-flavour vacuum survival model](two-flavour-vacuum-survival-model.md)
