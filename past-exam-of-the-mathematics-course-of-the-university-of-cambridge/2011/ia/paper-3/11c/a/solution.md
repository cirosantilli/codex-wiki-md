<h1 id="11c/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Integrating the local electric-field [divergence](../../../../../../divergence.md) equation and applying the [divergence theorem](../../../../../../divergence-theorem.md) gives [Gauss's law](../../../../../../gauss-s-law.md):

$$
\boxed{Q=\int_V\rho\,dV=\varepsilon_0\int_V\nabla\cdot\mathbf E\,dV
=\varepsilon_0\int_{\partial V}\mathbf E\cdot d\mathbf S.}
$$

For a [point charge](../../../../../../point-charge.md) at the origin, [spherical symmetry](../../../../../../spherical-symmetry.md) requires $\mathbf E=E_r(r)\mathbf e_r$. A sphere of radius $r>0$ encloses charge $q$, so its electric flux is $4\pi r^2E_r(r)$. Thus

$$
\boxed{\mathbf E(\mathbf x)=\frac{q}{4\pi\varepsilon_0r^2}\mathbf e_r
=\frac{q\mathbf x}{4\pi\varepsilon_0r^3}.}
$$

The [electrostatic potential](../../../../../../electric-potential.md) satisfies $E_r=-d\phi/dr$. Integrating and choosing the reference value $\phi(\infty)=0$ yields

$$
\boxed{\phi(\mathbf x)=\frac{q}{4\pi\varepsilon_0r}\quad(r>0).}
$$

An arbitrary additive constant gives any other choice of potential reference. The singularity at the origin is represented by the [Dirac delta distribution](../../../../../../dirac-delta-function.md); it is not a point where the ordinary derivatives of this field are finite.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [11C](../../11c.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ia](../../../split.md)
5. [2011](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
