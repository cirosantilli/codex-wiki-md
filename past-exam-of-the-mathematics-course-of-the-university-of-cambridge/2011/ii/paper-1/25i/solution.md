<h1 id="25i/solution">Solution</h1>

↑ **Parent:** [25I](../25i.md)

A point $x$ is critical for a smooth map $f:X\to Y$ when $Df_x:T_xX\to T_{f(x)}Y$ is not surjective. A critical value is the image of a critical point; a [regular value](../../../../../regular-value.md) has no critical point in its fiber, including the case of an empty fiber.

To prove the [regular level set theorem](../../../../../regular-level-set-theorem.md), take $x_0\in f^{-1}(y)$ and write $n=\dim X$, $m=\dim Y$. In local coordinates, surjectivity supplies an invertible $m\times m$ derivative minor; relabel source coordinates so it uses the first $m$ columns. The map

$$
\Phi(x)=(f_1(x),\ldots,f_m(x),x_{m+1},\ldots,x_n)
$$

has an invertible derivative. The [inverse function theorem](../../../../../inverse-function-theorem.md) makes it a local diffeomorphism. In these coordinates the fiber is obtained by fixing its first $m$ coordinates, so it is locally an open subset of $\mathbb R^{n-m}$. These smooth charts prove that **a nonempty regular fiber is a smooth embedded manifold of dimension $n-m$**, with tangent space $\ker Df_x$.

For the [special orthogonal group](../../../../../special-orthogonal-group.md), use $F:M_n(\mathbb R)\to\operatorname{Sym}_n(\mathbb R)$ defined by $F(A)=AA^T$. Its derivative is $DF_A(H)=HA^T+AH^T$. At an orthogonal $A$, any symmetric matrix $B$ is obtained by taking $H=BA/2$, so $I$ is a regular value. Therefore $O(n)=F^{-1}(I)$ has dimension $n^2-n(n+1)/2=n(n-1)/2$. The determinant takes only the values $\pm1$ there, so $SO(n)$ is an open and closed part of $O(n)$ and has the same manifold dimension:

$$
\boxed{\dim SO(n)=\frac{n(n-1)}2.}
$$

It is closed in matrix space and bounded because every orthogonal matrix column has norm one. The [Heine-Borel theorem](../../../../../heine-borel-theorem.md) proves compactness. Finally the tangent space is the derivative kernel,

$$
\boxed{T_ASO(n)=\{H:AH^T+HA^T=0\}
=\{AK:K^T=-K\}.}
$$

Thus its translated tangent space is the vector space of skew-symmetric matrices.

## ↑ Ancestors (11)

1. [25I](../25i.md)
2. [Section II](../section-ii.md)
3. [Paper 1](../../paper-1-split.md)
4. [Ii](../../split.md)
5. [2011](../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
