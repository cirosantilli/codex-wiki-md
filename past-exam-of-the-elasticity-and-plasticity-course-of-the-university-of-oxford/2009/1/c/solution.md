<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The perturbation preserves the prescribed [displacement](../../../../displacement.md) because $\mathbf w=0$ on the boundary. [Strain](../../../../strain.md) varies as $e_{ij}(\mathbf u+\alpha\mathbf w)=e_{ij}(\mathbf u)+\alpha(w_{i,j}+w_{j,i})/2$. Taylor expansion of the [strain energy density](../../../../strain-energy-density.md) gives

$$
U[\mathbf u+\alpha\mathbf w]-U[\mathbf u]
=\alpha\int_B\left[\tau_{ij}\frac{w_{i,j}+w_{j,i}}2-\rho g_iw_i\right]dV+O(\alpha^2).
$$

Symmetry of the [stress](../../../../stress.md) makes its contraction with the two symmetric terms equal, hence

$$
\boxed{U[\mathbf u+\alpha\mathbf w]-U[\mathbf u]=\alpha\int_B(\tau_{ij}w_{i,j}-\rho g_iw_i)\,dV+O(\alpha^2).}
$$

A [minimizer](../../../../global-minimizer.md) must have zero [first variation](../../../../first-variation.md) for both signs of $\alpha$. Integrating by parts and using the zero boundary variation yields $\int_B(-\partial_j\tau_{ij}-\rho g_i)w_i\,dV=0$. The [fundamental lemma of the calculus of variations](../../../../fundamental-lemma-of-the-calculus-of-variations.md), applied to arbitrary compactly supported variations, gives

$$
\boxed{\partial_j\tau_{ij}+\rho g_i=0,\quad\text{or }\nabla\cdot\tau+\rho\mathbf g=0.}
$$

This is the static momentum equation. Fixed-[displacement](../../../../displacement.md) data remove the surface variation; prescribed [tractions](../../../../traction.md) would instead appear through boundary work in the potential energy.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [2009](../../../2009-split.md)
4. [Past exam of the elasticity and plasticity course of the University of Oxford](../../../split.md)
5. [Elasticity and plasticity course of the University of Oxford](../../../../elasticity-and-plasticity-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
