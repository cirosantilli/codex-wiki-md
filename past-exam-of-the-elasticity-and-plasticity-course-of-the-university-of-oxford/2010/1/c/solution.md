<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [traction](../../../../traction.md) on the oriented solid element is

$$
\boxed{\boldsymbol\sigma=\tau\mathbf n,\qquad\sigma_i=\tau_{ij}n_j.}
$$

With constant Lamé coefficients and derivatives in the reference variables,

$$
\partial_j\tau_{ij}
=\lambda\partial_i(\partial_ku_k)
+\mu\partial_j(\partial_ju_i+\partial_iu_j)
=(\lambda+\mu)\partial_i(\nabla\cdot\mathbf u)+\mu\nabla^2u_i.
$$

Substitution into [balance of linear momentum](../../../../balance-of-linear-momentum.md) gives

$$
\boxed{\rho\mathbf u_{tt}=(\lambda+\mu)\nabla(\nabla\cdot\mathbf u)
+\mu\nabla^2\mathbf u+\rho\mathbf g.}
$$

To check the [vector](../../../../vector.md) identity componentwise, contract the two alternating [tensors](../../../../tensor.md):

$$
[\nabla\times(\nabla\times\mathbf u)]_i
=\epsilon_{ijk}\epsilon_{klm}\partial_j\partial_lu_m
=\partial_i\partial_ju_j-\partial_j\partial_ju_i.
$$

Rearranging proves $\nabla^2\mathbf u=\nabla(\nabla\cdot\mathbf u)-\nabla\times(\nabla\times\mathbf u)$. Therefore

$$
\boxed{\rho\mathbf u_{tt}=(\lambda+2\mu)\nabla(\nabla\cdot\mathbf u)
-\mu\nabla\times(\nabla\times\mathbf u)+\rho\mathbf g.}
$$

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [2010](../../../2010-split.md)
4. [Past exam of the elasticity and plasticity course of the University of Oxford](../../../split.md)
5. [Elasticity and plasticity course of the University of Oxford](../../../../elasticity-and-plasticity-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
