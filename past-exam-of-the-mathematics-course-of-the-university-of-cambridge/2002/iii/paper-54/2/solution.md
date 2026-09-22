<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

An [elastic deformation](../../../../../elastic-deformation.md) is reversible: after removal of the deforming loads the material returns to its reference state, and its instantaneous [stress](../../../../../stress.md) is determined by its current deformation rather than a plastic or viscous history. In the infinitesimal approximation the [displacement field](../../../../../displacement-field-mechanics.md) $u_i$ gives the [infinitesimal strain tensor](../../../../../infinitesimal-strain-tensor.md) $e_{ij}=(u_{i,j}+u_{j,i})/2$. The [Cauchy stress tensor](../../../../../cauchy-stress-tensor.md) is defined by [traction](../../../../../traction.md) $t_i=\sigma_{ij}n_j$ on a plane of unit normal $\mathbf n$; absence of body couples makes $\sigma_{ij}=\sigma_{ji}$.

Let $\mathcal E(e)$ be the recoverable [elastic energy](../../../../../elastic-energy.md) per unit mass. The local mechanical power per unit volume is

$$
\sigma_{ij}\partial_j\dot u_i=\sigma_{ij}\dot e_{ij},
$$

because the symmetric [Cauchy stress tensor](../../../../../cauchy-stress-tensor.md) annihilates the antisymmetric part of the velocity gradient. Conservation of [energy](../../../../../energy.md) during the deformation gives $\rho\dot{\mathcal E}=\sigma_{ij}\dot e_{ij}$. Since $\dot{\mathcal E}=(\partial\mathcal E/\partial e_{ij})\dot e_{ij}$ for arbitrary symmetric [strain](../../../../../strain.md) rates,

$$
\boxed{\sigma_{ij}=\rho\frac{\partial\mathcal E}{\partial e_{ij}}.}
$$

Here the derivative is the gradient on the space of symmetric tensors, with the double-contraction inner product. This convention accounts for the two occurrences of each off-diagonal entry; treating six independent coordinates without their corresponding factors would give an erroneous factor of two in shear components.

Take a stress-free reference state of [mass density](../../../../../density.md) $\rho_0$. The [Taylor series](../../../../../taylor-series.md) of the [elastic energy](../../../../../elastic-energy.md) starts quadratically:

$$
\mathcal E(e)=\mathcal E(0)+\frac1{2\rho_0}c_{ijkl}e_{ij}e_{kl}+O(|e|^3).
$$

Using $\rho=\rho_0+O(|e|)$ gives $\sigma_{ij}=c_{ijkl}e_{kl}+O(|e|^2)$, the relation of [linear elasticity](../../../../../linear-elasticity.md). If the reference state has initial [stress](../../../../../stress.md), the first-order expansion also retains that constant [stress](../../../../../stress.md). Symmetry of [stress](../../../../../stress.md) and [strain](../../../../../strain.md) gives the minor symmetries $c_{ijkl}=c_{jikl}=c_{ijlk}$, while equality of the mixed second derivatives of [elastic energy](../../../../../elastic-energy.md) gives the major symmetry $c_{ijkl}=c_{klij}$. Thus the [elastic stiffness tensor](../../../../../elastic-stiffness-tensor.md) is a symmetric map on a six-dimensional [strain](../../../../../strain.md) space: **there are $6\cdot7/2=21$ independent coefficients**.

For [twofold elastic symmetry](../../../../../twofold-elastic-symmetry.md), choose the symmetry axis as $x_3$. Rotation through $\pi$ is $Q=\operatorname{diag}(-1,-1,1)$, and transforms the [infinitesimal strain tensor](../../../../../infinitesimal-strain-tensor.md) into $QeQ^T$. Components $e_{11},e_{22},e_{33},e_{12}$ are even and $e_{23},e_{13}$ are odd. Invariance of [elastic energy](../../../../../elastic-energy.md) excludes every coupling between these parity classes. In the engineering [strain](../../../../../strain.md) ordering $(e_{11},e_{22},e_{33},2e_{23},2e_{13},2e_{12})$, with corresponding [stress](../../../../../stress.md) ordering $(\sigma_{11},\sigma_{22},\sigma_{33},\sigma_{23},\sigma_{13},\sigma_{12})$, the symmetric stiffness matrix has the form

$$
C=\begin{pmatrix}
C_{11}&C_{12}&C_{13}&0&0&C_{16}\\
C_{12}&C_{22}&C_{23}&0&0&C_{26}\\
C_{13}&C_{23}&C_{33}&0&0&C_{36}\\
0&0&0&C_{44}&C_{45}&0\\
0&0&0&C_{45}&C_{55}&0\\
C_{16}&C_{26}&C_{36}&0&0&C_{66}
\end{pmatrix}.
$$

Its symmetric even block has ten independent entries and its symmetric odd block has three. Hence **a twofold axis leaves $13$ independent coefficients**. No invariance under other rotation angles has been assumed.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 54](../../paper-54-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
