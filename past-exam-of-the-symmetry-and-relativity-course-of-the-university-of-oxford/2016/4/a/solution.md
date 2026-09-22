<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Take $A^\mu=(\varphi/c,\mathbf A)$, $\partial_\mu=(c^{-1}\partial_t,\nabla)$ and $J^\mu=(c\rho,\mathbf j)$. Then

$$
\mathbf E=-\nabla\varphi-\partial_t\mathbf A,\qquad
\mathbf B=\nabla\times\mathbf A,
\qquad F^{0i}=-E_i/c,\qquad F^{ij}=-\epsilon^{ijk}B_k.
$$

Expanding the cyclic derivative of $F^{ab}=\partial^aA^b-\partial^bA^a$ produces six second derivatives, which cancel in pairs because partial derivatives commute. Hence

$$
\boxed{\partial^cF^{ab}+\partial^aF^{bc}+\partial^bF^{ca}=0.}
$$

This [Bianchi identity](../../../../bianchi-identity.md) contains $\nabla\cdot\mathbf B=0$ and $\nabla\times\mathbf E=-\partial_t\mathbf B$. The inhomogeneous [Maxwell equations](../../../../maxwell-equations-split.md) are

$$
\boxed{\partial_\mu F^{\mu\nu}=\mu_0J^\nu,\qquad
\partial^\mu F_{\mu\nu}=\mu_0J_\nu.}
$$

The temporal component is $\nabla\cdot\mathbf E=\rho/\epsilon_0$, since $\epsilon_0\mu_0c^2=1$; the spatial components give $\nabla\times\mathbf B-c^{-2}\partial_t\mathbf E=\mu_0\mathbf j$. The source suppresses the coupling factor, as in units with $\mu_0=1$ or a rescaled current.

For the physical [Lorentz force density](../../../../lorentz-force-density.md) on matter, the consistent tensor formula is

$$
\boxed{f^\mu=F^{\mu\nu}J_\nu=
\left(\frac{\mathbf j\cdot\mathbf E}{c},\rho\mathbf E+\mathbf j\times\mathbf B\right),\qquad
f_\mu=F_{\mu\nu}J^\nu.}
$$

Its temporal component is power transferred to matter per unit volume divided by $c$. The printed expression $J^\nu F_{\nu\mu}$ has the **opposite sign** for the stated definition of $F$ in this convention. A stationary positive charge in a positive $x$ electric field is a concrete check: the physical upper spatial force is $+\rho E_x$, whereas the printed expression, raised to an upper index, gives $-\rho E_x$. It can represent the opposite momentum transfer to the electromagnetic field, but must not be identified with the force on the charge without changing a convention.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [4](../../4.md)
3. [2016](../../../2016-split.md)
4. [Past exam of the symmetry and relativity course of the University of Oxford](../../../split.md)
5. [Symmetry and relativity course of the University of Oxford](../../../../symmetry-and-relativity-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
