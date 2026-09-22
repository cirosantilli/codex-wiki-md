<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Take the trace of the constitutive relation at zero [stress](../../../stress.md). It gives $0=(2\mu+3\lambda)e_{kk}-3c\alpha(T-T_0)$. With the observed [stress](../../../stress.md)-free volume [strain](../../../strain.md) this requires

$$
\boxed{c=K=\lambda+\frac{2\mu}3.}
$$

This is the [bulk modulus](../../../bulk-modulus.md). A stable solid resists uniform compression, so $\boxed{K>0}$; equivalently the [elastic energy](../../../elastic-energy.md) of a nonzero pure dilation is positive. The [thermal strain](../../../thermal-strain.md) is isotropic, $e^{\rm th}_{ij}=\alpha(T-T_0)\delta_{ij}/3$, because $\alpha$ here is the volumetric, not linear, [thermal expansion](../../../thermal-expansion.md) coefficient.

Let $\beta=K\alpha$. Using $e_{ij}=(u_{i,j}+u_{j,i})/2$, [stress](../../../stress.md) divergence is

$$
\partial_j\tau_{ij}=\mu\Delta u_i+(\lambda+\mu)\partial_i(\nabla\cdot u)-\beta\partial_iT.
$$

Zero [body force](../../../body-force.md) and [equilibrium](../../../equilibrium-point-of-a-dynamical-system.md) therefore give

$$
\boxed{\mu\Delta u+(\lambda+\mu)\nabla(\nabla\cdot u)=\beta\nabla T,\qquad
\beta=\alpha(\lambda+2\mu/3).}
$$

For an applied [body force](../../../body-force.md) per unit volume $b$, [equilibrium](../../../equilibrium-point-of-a-dynamical-system.md) is $\nabla\cdot\tau+b=0$, so its right-hand side becomes $\beta\nabla T-b$. Consequently

$$
\boxed{b=+\beta\nabla T}
$$

cancels the effective thermal forcing in the [displacement](../../../displacement.md) equation. Per unit mass the force is $\beta\nabla T/\rho$. This sign follows from the divergence of the [thermal stress](../../../thermal-stress.md) $-\beta(T-T_0)I$, which is $-\beta\nabla T$. Cancelling that divergence is distinct from removing the [stress tensor](../../../cauchy-stress-tensor.md) itself: boundary tractions and thermal compatibility still matter.

For spatially uniform heating with the entire boundary fixed, $u=0$ is the unique [equilibrium](../../../equilibrium-point-of-a-dynamical-system.md) [displacement](../../../displacement.md) in a stable elastic solid, and

$$
\boxed{\tau_{ij}=-K\alpha(T-T_0)\delta_{ij}.}
$$

The [stress](../../../stress.md) is compressive [hydrostatic stress](../../../hydrostatic-stress.md) for a temperature rise. The fixed boundary supplies the tractions that prevent [thermal expansion](../../../thermal-expansion.md). If $T$ varies spatially and no compensating [body force](../../../body-force.md) is imposed, fixing the boundary alone does not generally force the interior [displacement](../../../displacement.md) to vanish: one must solve the displayed forced [Navier-Cauchy equation](../../../navier-cauchy-equation.md) with $u=0$ on the boundary, then recover the [stress](../../../stress.md). The simple uniform hydrostatic expression should not be asserted for arbitrary temperature fields. This is [uniform thermal stress in a fully constrained solid](../../../uniform-thermal-stress-in-a-fully-constrained-solid.md).

## ↑ Ancestors (11)

1. [4](../4.md)
2. [2007](../../2007-split.md)
3. [Past exam of the elasticity and plasticity course of the University of Oxford](../../split.md)
4. [Elasticity and plasticity course of the University of Oxford](../../../elasticity-and-plasticity-course-of-the-university-of-oxford.md)
5. [Year 4 of the mathematics course of the University of Oxford](../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
6. [Mathematics course of the University of Oxford](../../../mathematics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
