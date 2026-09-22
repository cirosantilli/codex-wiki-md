# Killing equation

↑ **Parent:** [Killing vector field](killing-vector-field-split.md)

The [Killing equation](killing-equation.md) tests whether a candidate [vector field](vector-field.md) generates a local [isometry](isometry.md), without needing to solve for its [flow of a vector field](flow-of-a-vector-field.md). For the [Levi-Civita connection](levi-civita-connection.md) of a [metric tensor](metric-tensor.md) $g$, it is

$$
\nabla_{(\mu}K_{\nu)}=\tfrac12(\nabla_\mu K_\nu+\nabla_\nu K_\mu)=0,
\qquad K_\nu=g_{\nu\rho}K^\rho.
$$

Parentheses mean averaging over the two index orders. The equation says the symmetric part of the [covariant derivative](covariant-derivative.md) vanishes, not that the entire [covariant derivative](covariant-derivative.md) vanishes. The [Lie derivative](lie-derivative-of-a-differential-form.md) of the [metric tensor](metric-tensor.md) gives the coordinate form

$$
(\mathcal L_Kg)_{\mu\nu}
=K^\rho\partial_\rho g_{\mu\nu}
+g_{\rho\nu}\partial_\mu K^\rho+g_{\mu\rho}\partial_\nu K^\rho
=\nabla_\mu K_\nu+\nabla_\nu K_\mu.
$$

The last two terms account for how [tangent vectors](tangent-vector-split.md) move with the field; checking only $K^\rho\partial_\rho g_{\mu\nu}$ misses this. See [Carroll, section 5, equations (5.33) and (5.41)-(5.42)](https://arxiv.org/pdf/gr-qc/9712019#page=147).

For the [Euclidean Killing vector field](euclidean-killing-vector-field.md) $K=-y\partial_x+x\partial_y$, the [Euclidean metric](euclidean-metric.md) in [Cartesian coordinates](cartesian-coordinate-system.md) makes [covariant derivatives](covariant-derivative.md) ordinary [partial derivatives](partial-derivative.md). Its diagonal equations give $\partial_xK_x=\partial_yK_y=0$, and its mixed equation gives $\partial_xK_y+\partial_yK_x=1-1=0$. Thus a varying [vector field](vector-field.md) can preserve a constant [metric tensor](metric-tensor.md). In contrast, $K=x\partial_x+y\partial_y$ gives $(\mathcal L_Kg)_{xx}=2$ and fails the [Killing equation](killing-equation.md), despite the constant metric components.

If $K=\partial_z$ is a [coordinate basis](coordinate-basis.md) vector, its components are constant and the coordinate form reduces to $\partial_zg_{\mu\nu}=0$. Hence independence of the metric components from $z$ supplies a [Killing vector field](killing-vector-field-split.md). This shortcut applies to that coordinate generator, not to an arbitrary varying [vector field](vector-field.md).

**Table of contents**

- [Killing derivative contraction identity](killing-derivative-contraction-identity.md)
- [Second covariant derivative of a Killing vector](second-covariant-derivative-of-a-killing-vector.md)
  - [Curvature-sign convention in Killing derivative identities](curvature-sign-convention-in-killing-derivative-identities.md)
  - [Killing vector preserves scalar curvature](killing-vector-preserves-scalar-curvature.md)

## ↑ Ancestors (5)

1. [Killing vector field](killing-vector-field-split.md)
2. [General relativity](general-relativity-split.md)
3. [Branches of physics](branches-of-physics.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (49)

- [Angular momentum conservation in an axisymmetric vacuum region](angular-momentum-conservation-in-an-axisymmetric-vacuum-region.md)
- [Charged-particle conserved quantity from a Killing symmetry](charged-particle-conserved-quantity-from-a-killing-symmetry.md)
- [Curvature-sign convention in Killing derivative identities](curvature-sign-convention-in-killing-derivative-identities.md)
- [Dimension bound for Killing vector fields](dimension-bound-for-killing-vector-fields.md)
- [Euclidean Killing vector field](euclidean-killing-vector-field.md)
- [Geodesic conserved quantity from a Killing vector](geodesic-conserved-quantity-from-a-killing-vector.md)
- [Killing derivative contraction identity](killing-derivative-contraction-identity.md)
- [Killing equation](killing-equation.md)
- [Killing fields on incomplete manifolds need not generate global isometries](killing-fields-on-incomplete-manifolds-need-not-generate-global-isometries.md)
- [Killing-flow four-acceleration](killing-flow-four-acceleration.md)
- [Killing transport](killing-transport.md)
- [Killing vector field](killing-vector-field-split.md)
- [Komar angular momentum with inner boundaries](komar-angular-momentum-with-inner-boundaries.md)
- [Normalized Killing one-form](normalized-killing-one-form.md)
- [Optical scalars on a Killing horizon](optical-scalars-on-a-killing-horizon.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-28/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-54/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-56/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-60/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-15/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-63/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ii/paper-2/35a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-61/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-63/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-54/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-56/2/c/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ii/paper-2/36b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-54/1/a/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-54/1/a/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-54/3/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-56/4/a/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-58/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-58/section-i/vi/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-51/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-52/1/b/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-52/1/b/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-52/1/b/iv/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-309/3/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-311/1/a/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-309/2/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-309/2/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-311/2/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-1/37d/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-1/37d/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-311/2/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-311/2/e/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-309/2/b/iii/solution.md)
- [Reissner-Nordstrom horizon surface gravity](reissner-nordstrom-horizon-surface-gravity.md)
- [Second covariant derivative of a Killing vector](second-covariant-derivative-of-a-killing-vector.md)
