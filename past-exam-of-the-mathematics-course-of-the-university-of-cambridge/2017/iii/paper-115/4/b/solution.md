<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $p_i:M_1\times M_2\to M_i$ be the projections. The derivative of the two projections identifies the [tangent bundle](../../../../../../tangent-bundle.md) with

$$
T(M_1\times M_2)\cong p_1^*TM_1\oplus p_2^*TM_2.
$$

Take the [direct sum](../../../../../../direct-sum.md) of the two [pullback connections](../../../../../../pullback-connection.md). This is the [product affine connection](../../../../../../product-affine-connection.md). In product coordinates $(x^a,y^\alpha)$, its only nonzero [Christoffel symbols](../../../../../../christoffel-symbol.md) are the two blocks inherited from the factors; all mixed coefficients are zero.

To make the connection on arbitrary fields explicit, write $V=V^a\partial_{x^a}+V^\alpha\partial_{y^\alpha}$ and $W=W^a\partial_{x^a}+W^\alpha\partial_{y^\alpha}$, allowing all coefficients to depend on both variables. Then

$$
\boxed{\begin{aligned}
(\nabla_VW)^a&=V(W^a)+(\Gamma^1)^a{}_{bc}(x)V^bW^c,\\
(\nabla_VW)^\alpha&=V(W^\alpha)+(\Gamma^2)^\alpha{}_{\beta\gamma}(y)V^\beta W^\gamma.
\end{aligned}}
$$

The terms $V(W^a)$ and $V(W^\alpha)$ include derivatives in both factors. Omitting these cross derivatives for fields with variable coefficients would not define a connection.

The formula is real-bilinear, linear over [smooth functions](../../../../../../smooth-function.md) in $V$, and obeys the [Leibniz rule](../../../../../../leibniz-rule.md) in $W$. Under a change of product coordinates each block has the factor's connection transformation law, so the local formulas agree; equivalently the [pullback connection](../../../../../../pullback-connection.md) construction already guarantees this gluing.

A field $X_i$ on one factor has a canonical lift to the product. Opposite-factor lifts commute, and their mixed covariant derivatives vanish. For such lifted fields the coefficient derivatives reduce to their factor derivatives, giving

$$
\boxed{\nabla_{Y_1+Y_2}(X_1+X_2)=\nabla^1_{Y_1}X_1+\nabla^2_{Y_2}X_2.}
$$

These values determine the connection uniquely: lifted coordinate frames span locally, and the connection's product rules determine its action on all their smooth linear combinations.

## ↑ Ancestors (11)

1. [B](../b.md)
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
