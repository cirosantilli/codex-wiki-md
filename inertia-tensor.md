# Inertia tensor

↑ **Parent:** [Moment of inertia](moment-of-inertia.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Inertia_tensor)

The [inertia tensor](inertia-tensor.md) packages the [moments of inertia](moment-of-inertia.md) about every axis through a specified point $O$ into one [symmetric matrix](symmetric-matrix.md). An axis still needs a direction: if $\mathbf n$ is a [unit vector](unit-vector.md), its scalar [moment of inertia](moment-of-inertia.md) is $I_{O,\mathbf n}=\mathbf n^T\mathbf I_O\mathbf n$. The same [mass](mass.md) layout can therefore be easy to spin about one direction and harder about another. The [inertia tensor](inertia-tensor.md) also determines [rotational kinetic energy](rotational-kinetic-energy.md) and relates [angular velocity](angular-velocity.md) to [angular momentum](angular-momentum.md) in the appropriate [rigid body](rigid-body-dynamics-split.md) model.

Take [position](position.md) vectors $\mathbf r=(x,y,z)$ relative to $O$, expressed in an [orthonormal basis](orthonormal-basis.md). For [point masses](point-mass.md) $m_a$, or a continuous distribution with [mass density](density.md) $\rho$ and $dm=\rho\,dV$,

$$
(\mathbf I_O)_{ij}=\sum_a m_a\bigl(|\mathbf r_a|^2\delta_{ij}-r_{ai}r_{aj}\bigr),
\qquad
(\mathbf I_O)_{ij}=\int\bigl(|\mathbf r|^2\delta_{ij}-r_ir_j\bigr)\,dm.
$$

Here $\delta_{ij}$ is the [Kronecker delta](kronecker-delta.md). Equivalently, using the [identity matrix](identity-matrix.md) $\mathbf1$ and an [outer product](outer-product.md),

$$
\mathbf I_O=\int\bigl(|\mathbf r|^2\mathbf1-\mathbf r\mathbf r^T\bigr)\,dm
=\int\begin{pmatrix}
y^2+z^2&-xy&-xz\\
-xy&x^2+z^2&-yz\\
-xz&-yz&x^2+y^2
\end{pmatrix}\,dm.
$$

Every entry has [SI](international-system-of-units.md) units $\mathrm{kg\,m^2}$. The diagonal entries are axial [moments of inertia](moment-of-inertia.md); the off-diagonal entries carry a minus sign in this convention. Some texts instead define the integrals without the prefixed minus sign $\int xy\,dm$, $\int xz\,dm$, $\int yz\,dm$ as their named off-diagonal quantities and put the minus signs into the displayed [matrix](matrix.md). Check that convention before combining formulas. [Moment of Inertia Tensor](newtonian-dynamics-by-richard-fitzpatrick/moment-of-inertia-tensor.md) [Lecture L26 - 3D Rigid Body Dynamics: The Inertia Tensor](16-07-dynamics/lecture-l26-3d-rigid-body-dynamics-the-inertia-tensor.md)

The [symmetric matrix](symmetric-matrix.md) is [positive semidefinite](positive-semidefinite-matrix.md), because its [quadratic form](quadratic-form-split.md) is

$$
\mathbf u^T\mathbf I_O\mathbf u
=\int\bigl(|\mathbf u|^2|\mathbf r|^2-(\mathbf u\cdot\mathbf r)^2\bigr)\,dm
=\int|\mathbf u\times\mathbf r|^2\,dm\geq0.
$$

The [dot product](dot-product.md) and [cross product](cross-product.md) identify this as a sum of squared distances when $\mathbf u$ is a [unit vector](unit-vector.md). A zero [moment of inertia](moment-of-inertia.md) occurs precisely when all the [mass](mass.md) lies on that axis, up to sets of zero [mass](mass.md). A genuine three-dimensional body with positive [mass density](density.md) in a volume has strictly positive axial [moments of inertia](moment-of-inertia.md). Do not confuse this [inertia tensor](inertia-tensor.md) with the [mass second-moment tensor](mass-second-moment-tensor.md) $\mathbf S=\int\mathbf r\mathbf r^T\,dm$: they obey $\mathbf I_O=\operatorname{tr}(\mathbf S)\mathbf1-\mathbf S$, where $\operatorname{tr}$ denotes the [matrix trace](matrix-trace.md).

If $O$ is fixed in an [inertial frame](inertial-frame.md) and each [velocity](velocity.md) is $\mathbf v=\boldsymbol\omega\times\mathbf r$, summing the individual [kinetic energies](kinetic-energy.md) and [angular momenta](angular-momentum.md) gives

$$
\mathbf L_O=\mathbf I_O\boldsymbol\omega,
\qquad
K=\frac12\boldsymbol\omega^T\mathbf I_O\boldsymbol\omega
=\frac12\boldsymbol\omega\cdot\mathbf L_O.
$$

These formulas also describe [angular momentum](angular-momentum.md) and [rotational kinetic energy](rotational-kinetic-energy.md) relative to the [centre of mass](center-of-mass.md) $G$ of a translating [rigid body](rigid-body-dynamics-split.md). In that case the total [kinetic energy](kinetic-energy.md) in the [inertial frame](inertial-frame.md) is $K_{\mathrm{total}}=\tfrac12M|\mathbf V_G|^2+\tfrac12\boldsymbol\omega^T\mathbf I_G\boldsymbol\omega$. For a general moving point $O$, the body's actual [velocities](velocity.md) include $\mathbf V_O$, so $\mathbf I_O\boldsymbol\omega$ alone need not be its [angular momentum](angular-momentum.md) about $O$. [Rotational Kinetic Energy](newtonian-dynamics-by-richard-fitzpatrick/rotational-kinetic-energy.md) [Lecture L26 - 3D Rigid Body Dynamics: The Inertia Tensor](16-07-dynamics/lecture-l26-3d-rigid-body-dynamics-the-inertia-tensor.md)

Changing the [orthonormal basis](orthonormal-basis.md) changes components, rather than the physical distribution: if the columns of an [orthogonal matrix](orthogonal-matrix.md) $Q$ are the new basis vectors expressed in the old basis, then $\mathbf I'_O=Q^T\mathbf I_OQ$. Changing the reference point is a different operation, governed by the [tensor parallel-axis theorem](tensor-parallel-axis-theorem.md). Both [principal axes](principal-axis.md) and [principal moments of inertia](principal-moment-of-inertia.md) must therefore be quoted with their reference point.

**Table of contents**

- [Inertia tensor of a uniform cube](inertia-tensor-of-a-uniform-cube.md)
- [Inertia tensor of a displaced uniform ball](inertia-tensor-of-a-displaced-uniform-ball.md)
- [Positive second-moment matrix test for an inertia tensor](positive-second-moment-matrix-test-for-an-inertia-tensor.md)
- [Inertia tensor of a sheared rectangular lamina](inertia-tensor-of-a-sheared-rectangular-lamina.md)
- [Inertia tensor of paired point masses](inertia-tensor-of-paired-point-masses.md)
- [Rotational inertia measurement with a falling mass](rotational-inertia-measurement-with-a-falling-mass.md)
  - [Rotary encoder](rotary-encoder.md)
- [Tensor parallel-axis theorem](tensor-parallel-axis-theorem.md)
- [Principal moment of inertia](principal-moment-of-inertia.md)
  - [Rotational energy ellipsoid](rotational-energy-ellipsoid.md)
  - [Degeneracy of principal moments of inertia](degeneracy-of-principal-moments-of-inertia.md)
- [Poinsot's ellipsoid](poinsot-s-ellipsoid.md)
  - [Herpolhode](herpolhode.md)
  - [Polhode](polhode.md)

## ↑ Ancestors (6)

1. [Moment of inertia](moment-of-inertia.md)
2. [Rigid body dynamics](rigid-body-dynamics-split.md)
3. [Classical mechanics](classical-mechanics-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (46)

- [Collective-rotation constraints for a Skyrmion](collective-rotation-constraints-for-a-skyrmion.md)
- [Degeneracy of principal moments of inertia](degeneracy-of-principal-moments-of-inertia.md)
- [Inertia tensor](inertia-tensor.md)
- [Inertia tensor of a displaced uniform ball](inertia-tensor-of-a-displaced-uniform-ball.md)
- [Inertia tensor of a sheared rectangular lamina](inertia-tensor-of-a-sheared-rectangular-lamina.md)
- [Inertia tensor of a uniform cube](inertia-tensor-of-a-uniform-cube.md)
- [Inertia tensor of paired point masses](inertia-tensor-of-paired-point-masses.md)
- [Mass second-moment tensor](mass-second-moment-tensor.md)
- [Moment of inertia](moment-of-inertia.md)
- [Odd-integrand cancellation by reflection](odd-integrand-cancellation-by-reflection.md)
- [Off-axis angular momentum of a square lamina](off-axis-angular-momentum-of-a-square-lamina.md)
- [Parallel axis theorem](parallel-axis-theorem.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/ib/paper-2/17b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ib/paper-1/14a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ii/paper-4/9c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ii/paper-4/9b/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ii/paper-3/9e/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ia/paper-3/9c/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ii/paper-4/12c/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ii/paper-4/12c/c/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-2/13e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-308/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-346/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-4/8b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ia/paper-3/12a/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ii/paper-2/14b/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2009/paper-2/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2016/paper-2/6/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2021/paper-2/6/b/i/solution.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2011/paper-2/section-c/c10/solution.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2012/paper-1/section-a/a5/solution.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2012/paper-2/section-b/b8/c/solution.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2014/paper-2/section-b/b8/b/solution.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2015/paper-2/section-b/b8/c/solution.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2016/paper-1/section-c/c11/solution.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2018/paper-1/section-c/c10/solution.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2019/paper-2/section-b/b9/solution.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2021/paper-1/section-a/a2/solution.md)
- [Solution](past-exam-of-the-physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2021/section-b/6/solution.md)
- [Positive second-moment matrix test for an inertia tensor](positive-second-moment-matrix-test-for-an-inertia-tensor.md)
- [Principal axis](principal-axis.md)
- [Principal moment of inertia](principal-moment-of-inertia.md)
- [Rigid rotor](rigid-rotor.md)
- [Rotational inertia measurement with a falling mass](rotational-inertia-measurement-with-a-falling-mass.md)
- [Rotational kinetic energy](rotational-kinetic-energy.md)
- [Tensor parallel-axis theorem](tensor-parallel-axis-theorem.md)
