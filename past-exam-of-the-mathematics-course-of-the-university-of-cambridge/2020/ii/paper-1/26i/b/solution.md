<h1 id="26i/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let

$$
F(x)=-x_0^2+x_1^2+x_2^2+x_3^2=x^TMx,
\qquad
M=\operatorname{diag}(-1,1,1,1).
$$

At $x\in F^{-1}(-1)$,

$$
dF_x(v)=2x^TMv.
$$

This differential is nonzero because $x\ne0$, so $-1$ is a [regular value](../../../../../../regular-value.md). The [regular level set theorem](../../../../../../regular-level-set-theorem.md) makes $F^{-1}(-1)$ a three-dimensional embedded submanifold; intersecting it with the open set $\{x_0>0\}$ preserves that property. Therefore $X$ is the [three-dimensional hyperboloid model](../../../../../../three-dimensional-hyperboloid-model.md), and

$$
\boxed{
T_xX=\ker dF_x
=\{v\in\mathbb R^4:-x_0v_0+x_1v_1+x_2v_2+x_3v_3=0\}
=\{v:x^TMv=0\}.
}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [26I](../../26i.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
