<h1 id="24f/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The formula $[X:Y:Z]\mapsto[X:Z]$ is initially undefined at the unique point $P_\infty=[0:1:0]$ of $X$ at infinity. Since $X$ is a [smooth projective curve](../../../../../../smooth-projective-curve.md), the [extension of a rational map from a smooth projective curve](../../../../../../extension-of-a-rational-map-from-a-smooth-projective-curve.md) extends it uniquely to a morphism

$$
\varphi:X\longrightarrow\mathbb P^1.
$$

On the affine chart it is the rational function $x$, and the equation $y^3=x^4+1$ shows that $\varphi$ has degree three.

For each of the four roots $\alpha$ of $x^4+1$, let $P_\alpha=(\alpha,0)$. Since the root is simple, $t=y$ is a [uniformizer](../../../../../../uniformizer.md) at $P_\alpha$, and the equation gives

$$
x-\alpha=c_\alpha t^3+O(t^6),
\qquad c_\alpha\ne0.
$$

Thus the [ramification index of a holomorphic map](../../../../../../ramification-index-of-a-holomorphic-map.md) at every $P_\alpha$ is three.

At $P_\infty$, use the chart $Y=1$ and put $u=X/Y$, $v=Z/Y$. The equation becomes

$$
v=u^4+v^4.
$$

The [implicit function theorem](../../../../../../implicit-function-theorem.md) makes $u$ a uniformizer and gives $v=u^4$ times a local unit. Hence

$$
x=\frac XZ=\frac uv=u^{-3}\mathbin{\cdot}(\text{local unit}),
$$

so $P_\infty$ also has ramification index three. These are all the [ramification points of a holomorphic map](../../../../../../ramification-point-of-a-holomorphic-map.md) because the resulting ramification degree is $5(3-1)=10$. Indeed, the [Riemann-Hurwitz formula](../../../../../../riemann-hurwitz-formula.md) gives

$$
2g_X-2=3(2g_{\mathbb P^1}-2)+10=-6+10=4.
$$

Therefore $g_X=3$, in agreement with the [genus of a smooth plane curve](../../../../../../genus-of-a-smooth-plane-curve.md), and the [Euler characteristic](../../../../../../euler-characteristic.md) of the underlying compact orientable surface is

$$
\boxed{g_X=3,\qquad \chi(X)=2-2g_X=-4.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [24F](../../24f.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
