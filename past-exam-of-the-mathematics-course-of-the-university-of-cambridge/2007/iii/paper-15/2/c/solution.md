<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Fix any point $p$ and use a [normal orthonormal frame](../../../../../../normal-orthonormal-frame.md) there. Such frames exist: in [geodesic normal coordinates](../../../../../../geodesic-normal-coordinates.md), $g_{ij}(p)=\delta_{ij}$, $\partial_kg_{ij}(p)=0$ and the [Christoffel symbols](../../../../../../christoffel-symbol.md) vanish at $p$. Applying the [Gram-Schmidt process](../../../../../../gram-schmidt-process.md) smoothly to the coordinate fields gives identity coefficients at $p$ and zero first derivatives there, so it produces the required frame. Reverse one frame vector if necessary to match the [orientation](../../../../../../orientation-of-a-simplex.md).

Because the [Levi-Civita connection](../../../../../../levi-civita-connection.md) is torsion-free, $[E_j,E_k](p)=(\nabla_{E_j}E_k-\nabla_{E_k}E_j)(p)=0$. The supplied formula for the [exterior derivative](../../../../../../exterior-derivative.md) of a one-form gives

$$
d\omega_i(E_j,E_k)(p)
=E_j(\delta_{ik})(p)-E_k(\delta_{ij})(p)-\omega_i([E_j,E_k](p))=0.
$$

Thus $d\omega_i(p)=0$, and the graded [Leibniz rule](../../../../../../leibniz-rule.md) implies $d\theta_i(p)=0$. Differentiate the formula in part (b):

$$
d\nu(p)=\sum_i(-1)^{i+1}df_i(p)\wedge\theta_i(p).
$$

Since $df_i=\sum_jE_j(f_i)\omega_j$, every summand with $j\ne i$ vanishes because $\omega_j$ already occurs in $\theta_i$. The remaining term has $\omega_i\wedge\theta_i=(-1)^{i-1}\omega_g$, so both signs cancel. Hence

$$
d\nu(p)=\sum_i E_i(f_i)(p)\omega_g(p)
=(\operatorname{div}X)(p)\omega_g(p).
$$

The point was arbitrary, proving the global [exterior derivative of contracted volume form](../../../../../../exterior-derivative-of-contracted-volume-form.md) identity

$$
\boxed{d\nu=(\operatorname{div}X)\omega_g.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 15](../../../paper-15-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
