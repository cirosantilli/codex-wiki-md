<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $D_{abc}=\nabla_a\nabla_bK_c$. Differentiating the [Killing equation](../../../../../../killing-equation.md) gives $D_{abc}=-D_{acb}$. For a covector, the [Ricci identity](../../../../../../curvature-commutator-on-a-covariant-tensor.md) is

$$
D_{abc}-D_{bac}=-R^d{}_{cab}K_d=R_{cdab}K^d.
$$

Call this difference $C_{abc}$. The differentiated [Killing equation](../../../../../../killing-equation.md) then gives

$$
C_{abc}=D_{abc}+D_{bca},\quad
C_{bca}=D_{bca}+D_{cab},\quad
C_{cab}=D_{cab}+D_{abc}.
$$

Taking the first minus the second plus the third yields

$$
2D_{abc}=(R_{cdab}-R_{adbc}+R_{bdca})K^d.
$$

The pair symmetries of the [Riemann curvature tensor](../../../../../../riemann-curvature-tensor.md) and the [first Bianchi identity](../../../../../../first-bianchi-identity.md) reduce the coefficient to $2R_{cbad}$. Therefore the [second covariant derivative of a Killing vector](../../../../../../second-covariant-derivative-of-a-killing-vector.md) is

$$
\boxed{\nabla_a\nabla_bK_c=R_{cbad}K^d,\qquad
\nabla_a\nabla_bK^c=R^c{}_{bad}K^d.}
$$

For an [affine parameter](../../../../../../affine-parameter.md) $\lambda$ on a [geodesic](../../../../../../geodesic.md), its tangent obeys $V^b\nabla_bV^a=0$. Thus

$$
\frac{d}{d\lambda}(K_aV^a)
=V^bV^a\nabla_bK_a+K_aV^b\nabla_bV^a=0.
$$

The second term vanishes by the [geodesic equation](../../../../../../geodesic-equation.md); the first contracts a symmetric product $V^aV^b$ with the antisymmetric derivative from the [Killing equation](../../../../../../killing-equation.md). This establishes the [geodesic conserved quantity from a Killing vector](../../../../../../geodesic-conserved-quantity-from-a-killing-vector.md):

$$
\boxed{K_aV^a\text{ is constant along every affinely parametrized geodesic}.}
$$

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 309](../../../paper-309-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
