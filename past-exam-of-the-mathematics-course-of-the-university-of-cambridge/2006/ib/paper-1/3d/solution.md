<h1 id="3d/solution">Solution</h1>

↑ **Parent:** [3D](../3d.md)

Write the [holomorphic function](../../../../../holomorphic-function.md) as $f=u+iv$. Analyticity gives smooth real and imaginary parts satisfying the [Cauchy-Riemann equations](../../../../../cauchy-riemann-equations.md) $u_x=v_y$, $u_y=-v_x$. Differentiating these identities shows

$$
\Delta u=v_{yx}-v_{xy}=0,\qquad \Delta v=-u_{yx}+u_{xy}=0.
$$

Thus both parts are [harmonic functions](../../../../../harmonic-function.md). The [product rule](../../../../../product-rule.md) then gives

$$
\Delta|f|^2=\Delta(u^2+v^2)
=2(u_x^2+u_y^2+v_x^2+v_y^2)+2u\Delta u+2v\Delta v
=4(u_x^2+v_x^2).
$$

Since $f'=u_x+iv_x$, this proves the [Laplacian identity for the squared modulus of a holomorphic function](../../../../../laplacian-identity-for-the-squared-modulus-of-a-holomorphic-function.md),

$$
\boxed{\Delta|f(z)|^2=4|f'(z)|^2.}
$$

## ↑ Ancestors (10)

1. [3D](../3d.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
