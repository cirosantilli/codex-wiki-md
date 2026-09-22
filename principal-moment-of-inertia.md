# Principal moment of inertia

↑ **Parent:** [Inertia tensor](inertia-tensor.md)

The [principal moments of inertia](principal-moment-of-inertia.md) about a specified point $O$ are the [eigenvalues](eigenvalue.md) $I_1,I_2,I_3$ of the [inertia tensor](inertia-tensor.md) $\mathbf I_O$. Their associated [unit vectors](unit-vector.md) that are [eigenvectors](eigenvector.md) specify [principal axes](principal-axis.md) through $O$. The [spectral theorem for real symmetric matrices](spectral-theorem-for-real-symmetric-matrices.md) guarantees an [orthonormal basis](orthonormal-basis.md) of these [eigenvectors](eigenvector.md), even for an irregular [rigid body](rigid-body-dynamics-split.md). Choose their signs to make a right-handed basis and collect them as the columns of an [orthogonal matrix](orthogonal-matrix.md) $Q$:

$$
\mathbf I_O\mathbf e_i=I_i\mathbf e_i,
\qquad Q^T\mathbf I_OQ=\operatorname{diag}(I_1,I_2,I_3).
$$

Thus [diagonalization](diagonalization-of-a-matrix.md) removes the off-diagonal coupling in the [rotational kinetic energy](rotational-kinetic-energy.md). The [eigenvalues](eigenvalue.md) belong to the [mass](mass.md) distribution and reference point, independently of which [orthonormal basis](orthonormal-basis.md) initially describes them. [Principal Axes of Rotation](newtonian-dynamics-by-richard-fitzpatrick/principal-axes-of-rotation.md)

In this [principal body frame](principal-body-frame.md), write [angular velocity](angular-velocity.md) as $\boldsymbol\omega=\sum_i\omega_i\mathbf e_i$. Then

$$
\mathbf L_O=\sum_i I_i\omega_i\mathbf e_i,
\qquad
K=\frac12\sum_i I_i\omega_i^2.
$$

Use these as total [angular momentum](angular-momentum.md) and [kinetic energy](kinetic-energy.md) only under the reference-point conditions stated under [inertia tensor](inertia-tensor.md). Along a single [principal axis](principal-axis.md) with $I_i>0$, [angular momentum](angular-momentum.md) is parallel to [angular velocity](angular-velocity.md). For a mixture of directions with different [principal moments of inertia](principal-moment-of-inertia.md), it generally is not. A [principal axis](principal-axis.md) need not be a geometric symmetry axis: it is selected by the complete [mass](mass.md) distribution. A [principal axis](principal-axis.md) also need not give stable free rotation; for three distinct [principal moments of inertia](principal-moment-of-inertia.md), the [intermediate axis theorem](intermediate-axis-theorem.md) supplies the stability distinction.

For any [unit vector](unit-vector.md) $\mathbf n=\sum_i n_i\mathbf e_i$,

$$
I_{O,\mathbf n}=\sum_i I_i n_i^2,
\qquad \sum_i n_i^2=1,
\qquad \min_i I_i\leq I_{O,\mathbf n}\leq\max_i I_i.
$$

The axial [moment of inertia](moment-of-inertia.md) is a weighted average of the [principal moments of inertia](principal-moment-of-inertia.md). At fixed [angular speed](angular-speed.md), the least and greatest [rotational kinetic energies](rotational-kinetic-energy.md) occur in the corresponding [eigenspaces](eigenspace.md). At fixed nonzero [angular momentum](angular-momentum.md) magnitude $L$, instead, $K=\tfrac12\sum_i L_i^2/I_i$, so the largest [principal moment of inertia](principal-moment-of-inertia.md) gives the smallest [rotational kinetic energy](rotational-kinetic-energy.md). These comparisons hold the reference point fixed.

There is an additional physical restriction beyond [positive semidefiniteness](positive-semidefinite-matrix.md). In [principal axes](principal-axis.md) coordinates,

$$
I_1+I_2-I_3=2\int z^2\,dm\geq0,
$$

with two analogous cyclic inequalities. Therefore three arbitrary positive numbers do not always represent a possible [inertia tensor](inertia-tensor.md). For a distribution in the $xy$ plane through $O$, $I_3=I_1+I_2$, as in the planar [inertia tensor of paired point masses](inertia-tensor-of-paired-point-masses.md). A uniform solid [ellipsoid](ellipsoid.md) of [mass](mass.md) $M$ and semiaxes $a,b,c$ supplies a continuous three-dimensional example: using its [mass second-moment tensor](mass-second-moment-tensor.md), its central [principal moments of inertia](principal-moment-of-inertia.md) are $M(b^2+c^2)/5$, $M(a^2+c^2)/5$, $M(a^2+b^2)/5$. Setting $a=b=c=R$ recovers the [moment of inertia of a uniform solid sphere](moment-of-inertia-of-a-uniform-solid-sphere.md).

**Table of contents**

- [Rotational energy ellipsoid](rotational-energy-ellipsoid.md)
- [Degeneracy of principal moments of inertia](degeneracy-of-principal-moments-of-inertia.md)

## ↑ Ancestors (7)

1. [Inertia tensor](inertia-tensor.md)
2. [Moment of inertia](moment-of-inertia.md)
3. [Rigid body dynamics](rigid-body-dynamics-split.md)
4. [Classical mechanics](classical-mechanics-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (8)

- [Gyroscope vector geometry](gyroscope-vector-geometry.md)
- [Inertia tensor of paired point masses](inertia-tensor-of-paired-point-masses.md)
- [Linear stability of principal-axis rotation](linear-stability-of-principal-axis-rotation.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ii/paper-3/9e/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-4/15e/a/solution.md)
- [Principal moment of inertia](principal-moment-of-inertia.md)
- [Rotational energy ellipsoid](rotational-energy-ellipsoid.md)
- [Rotational inertia measurement with a falling mass](rotational-inertia-measurement-with-a-falling-mass.md)
