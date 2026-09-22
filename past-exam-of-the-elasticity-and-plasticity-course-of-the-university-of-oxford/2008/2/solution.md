<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Use the [torsion stress function for a simply connected bar](../../../torsion-stress-function-for-a-simply-connected-bar.md). The only nonzero [strain](../../../strain.md) components are $e_{xz}=(w_x-\Omega y)/2$ and $e_{yz}=(w_y+\Omega x)/2$. Thus

$$
\tau_{xz}=\mu(w_x-\Omega y),\qquad\tau_{yz}=\mu(w_y+\Omega x).
$$

The axial [equilibrium](../../../equilibrium-point-of-a-dynamical-system.md) equation is $\partial_x\tau_{xz}+\partial_y\tau_{yz}=0$. Since the section is [simply connected](../../../simply-connected-space.md), the planar [divergence-free](../../../solenoidal-vector-field.md) [stress](../../../stress.md) field has a [stream function](../../../stream-function.md):

$$
\boxed{\tau_{xz}=\phi_y,\quad\tau_{yz}=-\phi_x,\quad w_x=\Omega y+\phi_y/\mu,\quad w_y=-\Omega x-\phi_x/\mu.}
$$

Equality of the mixed [warping](../../../torsional-warping.md) derivatives gives $\boxed{\Delta\phi=-2\mu\Omega}$. On the lateral boundary the axial [traction](../../../traction.md) is $\phi_y n_x-\phi_xn_y$, the tangential derivative of $\phi$. [Traction](../../../traction.md)-free walls therefore make $\phi$ constant on the connected boundary, and its arbitrary additive constant can be chosen so $\boxed{\phi=0\text{ on }\partial D}$.

The axial [torque](../../../torque.md) is

$$
M=\int_D(x\tau_{yz}-y\tau_{xz})\,dA=-\int_D(x\phi_x+y\phi_y)\,dA=\boxed{2\int_D\phi\,dA}.
$$

The [divergence theorem](../../../divergence-theorem.md) removes the boundary term because $\phi=0$.

Tresca's yield criterion requires the maximum [shear stress](../../../shear-stress.md), half the largest principal-[stress](../../../stress.md) difference, not to exceed the material's shear [yield stress](../../../yield-stress.md) $\tau_Y$. The [stress](../../../stress.md) [eigenvalues](../../../eigenvalue.md) here are $0,\pm\sqrt{\tau_{xz}^2+\tau_{yz}^2}$, so the maximum shear is $|\nabla\phi|$ and

$$
\boxed{|\nabla\phi|\leq\tau_Y.}
$$

If yield is instead quoted as a uniaxial tensile [stress](../../../stress.md), that parameter is $2\tau_Y$; the present convention is the source's shear parameter.

For the [ellipse](../../../ellipse.md), the proposed quadratic vanishes on its boundary. Its Laplacian fixes

$$
\boxed{C=\frac{\mu\Omega a^2b^2}{a^2+b^2},\qquad\phi=C(1-x^2/a^2-y^2/b^2).}
$$

The corresponding [warping](../../../torsional-warping.md) is $w=\Omega(b^2-a^2)xy/(a^2+b^2)+\text{constant}$. Elliptic polar coordinates $x=ar\cos\vartheta$, $y=br\sin\vartheta$ give $\int_D\phi=C\pi ab/2$, hence

$$
\boxed{M=\frac{\pi\mu\Omega a^3b^3}{a^2+b^2},\qquad R=M/\Omega=\frac{\pi\mu a^3b^3}{a^2+b^2}.}
$$

To locate first yield, maximize $|\nabla\phi|=2|C|\sqrt{x^2/a^4+y^2/b^4}$. It increases radially to the boundary. For $a>b$, the maximum there occurs at $(0,\pm b)$ and equals $2|C|/b$. Therefore

$$
\boxed{|\Omega|_Y=\frac{(a^2+b^2)\tau_Y}{2a^2b\mu}.}
$$

The positive-twist value is the requested expression. The ends of the minor axis yield first, not the ends of the longer axis. This is [elliptical-bar torsion and first yield](../../../elliptical-bar-torsion-and-first-yield.md).

## ↑ Ancestors (11)

1. [2](../2.md)
2. [2008](../../2008-split.md)
3. [Past exam of the elasticity and plasticity course of the University of Oxford](../../split.md)
4. [Elasticity and plasticity course of the University of Oxford](../../../elasticity-and-plasticity-course-of-the-university-of-oxford.md)
5. [Year 4 of the mathematics course of the University of Oxford](../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
6. [Mathematics course of the University of Oxford](../../../mathematics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
