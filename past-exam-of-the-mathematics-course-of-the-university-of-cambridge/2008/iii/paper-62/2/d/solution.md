<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For a homogeneous [scalar field](../../../../../../scalar-field.md), every spatial derivative vanishes. The [stress-energy tensor](../../../../../../stress-energy-tensor.md) consequently has no [momentum density](../../../../../../momentum-density.md) or directional stress:

$$
T^{0i}=0,\qquad T^{ij}=Pa^{-2}\delta^{ij},\qquad
\rho=\frac12\dot\phi^2+V,\quad P=\frac12\dot\phi^2-V.
$$

The only spatial tensor left is $\delta^{ij}$, so the stress is isotropic. This is the [perfect fluid](../../../../../../perfect-fluid.md) form in its comoving frame. Now expand the time component of [stress-energy conservation](../../../../../../stress-energy-conservation.md) using the [covariant derivative](../../../../../../covariant-derivative.md):

$$
0=\nabla_\mu T^{\mu0}
=\partial_\mu T^{\mu0}+\Gamma^\mu{}_{\mu\lambda}T^{\lambda0}
+\Gamma^0{}_{\mu\lambda}T^{\mu\lambda}.
$$

The first term is $\dot\rho$. In the second, only $\lambda=0$ contributes, and $\sum_i\Gamma^i{}_{i0}=3H$, giving $3H\rho$. The third is

$$
\sum_{i,j}(a\dot a\delta_{ij})(Pa^{-2}\delta^{ij})=3HP.
$$

Here the quoted [Christoffel symbols](../../../../../../christoffel-symbol.md) include their lower-index symmetry $\Gamma^i{}_{j0}=\Gamma^i{}_{0j}$. Therefore the [cosmological continuity equation](../../../../../../cosmological-continuity-equation.md) is

$$
\boxed{\dot\rho=-3\frac{\dot a}{a}(\rho+P).}
$$

As a check using the [scalar field](../../../../../../scalar-field.md) equation, $\dot\rho=\dot\phi(\ddot\phi+V_{,\phi})=-3H\dot\phi^2=-3H(\rho+P)$, with exactly the same sign.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 62](../../../paper-62-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
