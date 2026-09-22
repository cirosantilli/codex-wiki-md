<h1 id="11f/solution">Solution</h1>

↑ **Parent:** [11F](../11f.md)

The [tangent vectors](../../../../../tangent-vector.md) of

$$
\sigma(u,v)=(u,v,f(u,v))
$$

are

$$
\sigma_u=(1,0,f_u),
\qquad
\sigma_v=(0,1,f_v).
$$

Hence the [first fundamental form](../../../../../first-fundamental-form.md) has coefficients

$$
E=1+f_u^2,
\qquad
F=f_uf_v,
\qquad
G=1+f_v^2.
$$

Put

$$
W=\sqrt{1+f_u^2+f_v^2}.
$$

The upward [unit normal](../../../../../unit-normal.md) is $N=(-f_u,-f_v,1)/W$, so the [second fundamental form](../../../../../second-fundamental-form-split.md) has coefficients

$$
e=\frac{f_{uu}}W,
\qquad
f_{II}=\frac{f_{uv}}W,
\qquad
g=\frac{f_{vv}}W.
$$

Thus the two forms are

$$
I=E\,du^2+2F\,du\,dv+G\,dv^2,
\qquad
II=e\,du^2+2f_{II}\,du\,dv+g\,dv^2.
$$

The [Gaussian curvature](../../../../../gaussian-curvature.md) is

$$
K=\frac{eg-f_{II}^2}{EG-F^2}.
$$

Since $EG-F^2=W^2$, the graph formula is

$$
\boxed{
K=\frac{f_{uu}f_{vv}-f_{uv}^2}
{(1+f_u^2+f_v^2)^2}
},
$$

as in [Gaussian curvature of a graph surface](../../../../../gaussian-curvature-of-a-graph-surface.md).

For the final claim, fix a point of $\gamma$ and make a [rigid motion](../../../../../rigid-transformation.md) taking $P$ to the plane $z=0$. The common tangent plane is horizontal, so locally $\Sigma$ is the graph $z=f(u,v)$. Along the projected curve $c(s)$ of tangency,

$$
f(c(s))=0,
\qquad
\nabla f(c(s))=0.
$$

Differentiating the second identity gives

$$
\operatorname{Hess}f(c(s))\,c'(s)=0.
$$

Because $c$ is a [smooth curve](../../../../../smooth-curve.md), $c'(s)\ne0$, so the Hessian is singular. Its [determinant](../../../../../determinant.md) is zero, and the graph formula gives $K=0$ at every point of $\gamma$. This is [tangency to a plane along a curve forces zero Gaussian curvature](../../../../../tangency-to-a-plane-along-a-curve-forces-zero-gaussian-curvature.md).

## ↑ Ancestors (10)

1. [11F](../11f.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
