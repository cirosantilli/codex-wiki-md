<h1 id="25i/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a local parametrization $\phi(u,v)$, write the [first fundamental form](../../../../../../first-fundamental-form.md) and [second fundamental form](../../../../../../second-fundamental-form-split.md) as

$$
I=E\,du^2+2F\,du\,dv+G\,dv^2,
\qquad
II=e\,du^2+2f\,du\,dv+g\,dv^2.
$$

The [Gaussian curvature](../../../../../../gaussian-curvature.md) is

$$
\boxed{K=\frac{eg-f^2}{EG-F^2}.}
$$

To prove the [Theorema Egregium](../../../../../../theorema-egregium.md), set $g_{ij}=\langle\phi_i,\phi_j\rangle$ and decompose

$$
\phi_{ij}=\Gamma^k_{ij}\phi_k+h_{ij}N.
$$

Differentiating $g_{ij}$ and solving for the tangential coefficients gives

$$
\Gamma_{ijk}
=\frac12\left(\partial_i g_{jk}+\partial_jg_{ik}-\partial_kg_{ij}\right),
$$

so every [Christoffel symbol](../../../../../../christoffel-symbol.md) depends only on $E,F,G$ and their first derivatives. Equality of mixed third derivatives yields the [Gauss equation](../../../../../../gauss-equation.md)

$$
R_{1212}=h_{11}h_{22}-h_{12}^2=eg-f^2.
$$

The [Riemann curvature tensor](../../../../../../riemann-curvature-tensor.md) is formed from first derivatives and quadratic products of the Christoffel symbols, and hence from the first and second derivatives of $E,F,G$. Consequently

$$
\boxed{K=\frac{R_{1212}}{\det(g_{ij})}
=\frac{R_{1212}}{EG-F^2}}
$$

depends only on the first fundamental form.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [25I](../../25i.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
