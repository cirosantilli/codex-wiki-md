<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [product Riemannian metric](../../../../../../product-riemannian-metric.md) is

$$
\boxed{g=p_1^*g_1+p_2^*g_2,\qquad
g_{(p,q)}((u_1,u_2),(v_1,v_2))=(g_1)_p(u_1,v_1)+(g_2)_q(u_2,v_2).}
$$

It is smooth and symmetric. If $(u_1,u_2)\ne0$, at least one component is nonzero and contributes a strictly positive squared norm; the other contributes a nonnegative term. Thus $g$ is positive definite.

Let the factor connections be [Levi-Civita connections](../../../../../../levi-civita-connection.md). The [torsion form](../../../../../../torsion-form.md) of the [product affine connection](../../../../../../product-affine-connection.md) vanishes on two lifted fields from one factor because it equals the factor torsion; on opposite-factor fields it vanishes because both covariant derivatives and the [Lie bracket of vector fields](../../../../../../lie-bracket-of-vector-fields.md) vanish. By [tensoriality](../../../../../../tensoriality.md), torsion vanishes for all fields.

Check [metric compatibility](../../../../../../metric-compatibility.md) on lifted fields as well. When the two paired fields are from one factor, their metric pairing depends only on that factor. Differentiation along that factor gives the usual factor compatibility identity, and differentiation along the other factor gives zero on both sides. When the paired fields are from different factors, their pairing is identically zero and their derivatives stay in their original summands, so both sides are again zero. Since $\nabla g$ has [tensoriality](../../../../../../tensoriality.md), these checks imply $\nabla g=0$ globally.

The [existence and uniqueness of the Levi-Civita connection](../../../../../../existence-and-uniqueness-of-the-levi-civita-connection.md) therefore gives

$$
\boxed{\nabla^{g}=p_1^*\nabla^{g_1}\oplus p_2^*\nabla^{g_2}.}
$$

Equivalently, applying the [Christoffel symbol](../../../../../../christoffel-symbol.md) formula to the block metric gives the factor coefficients and zero mixed coefficients, because each factor metric is independent of the other coordinates.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 115](../../../paper-115-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
