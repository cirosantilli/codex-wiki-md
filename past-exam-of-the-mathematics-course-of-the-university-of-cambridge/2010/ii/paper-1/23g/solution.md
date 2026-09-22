<h1 id="23g/solution">Solution</h1>

↑ **Parent:** [23G](../23g.md)

Put $A=\wp(w)$ and $B=\wp'(w)$. At $z=0$, the first column has $\wp(z)=z^{-2}+O(z^2)$ and $\wp'(z)=-2z^{-3}+O(z)$, whereas the third has $\wp(-z-w)=A+Bz+O(z^2)$. Expanding the [determinant](../../../../../determinant.md), the coefficient multiplying $\wp'(z)$ is $\wp(-z-w)-A=O(z)$, so the apparent cubic pole reduces to order at most two. The only other possible pole is at $z=-w$, and $f(-z-w)=-f(z)$ gives the same bound there. Thus, **if $f$ is nonconstant, its total pole order and valency are at most four**. A constant case is handled by finding a zero below.

Column coincidences give zeros at $z=w$, at $z=-2w$, and at the four solutions of $2z=-w$ on $\mathbb C/\Lambda$. The latter are distinct because $\Lambda/2\Lambda$ has four elements. If $3w\notin\Lambda$, the first two points are distinct from each other and from these four solutions.

One exceptional pole issue needs care: when $2w\in\Lambda$, the first two prospective zeros are $w$ and $0$, the possible pole locations. They are actually removable zeros. Here $B=0$, and, with $C=\wp''(w)$, evenness about this half-period gives

$$
\wp(-z-w)=A+\frac C2z^2+O(z^4),\qquad
\wp'(-z-w)=-Cz+O(z^3).
$$

The [determinant](../../../../../determinant.md) becomes $(A-\wp(z))\wp'(-z-w)+\wp'(z)(\wp(-z-w)-A)$. Its two $C/z$ contributions cancel and it is $O(z)$; reflection transfers this conclusion to $z=w$. Thus there really are **six distinct zeros** also in this case.

If $3w\in\Lambda$ but $w\notin\Lambda$, then $z=w=-2w$ is one of the four solutions of $2z=-w$. All three columns coincide there, with no pole. Both the [determinant](../../../../../determinant.md) and its first derivative vanish, since each term in the derivative still has two identical columns. Hence there are **four distinct zeros, at least one multiple**, giving at least five zeros counted with multiplicity.

For a nonconstant [elliptic function](../../../../../elliptic-function.md), zeros and poles in a period parallelogram have equal total multiplicity, by the [argument principle](../../../../../argument-principle.md). Either count contradicts total pole order at most four. A constant with a zero is zero, so

$$
\boxed{f\equiv0.}
$$

This is the [elliptic collinearity determinant](../../../../../elliptic-collinearity-determinant.md). Consequently, when $z_1+z_2+z_3\in\Lambda$, the three vectors $(1,\wp(z_i),\wp'(z_i))$ have zero [determinant](../../../../../determinant.md). The three points on the [Weierstrass equation of an elliptic curve](../../../../../weierstrass-equation-of-an-elliptic-curve.md) are therefore **collinear in $\mathbb C^2$**.

## ↑ Ancestors (10)

1. [23G](../23g.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
