<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [multivariable chain rule](../../../../../../multivariable-chain-rule.md) first gives

$$
g_u=uf_x+vf_y,\qquad g_v=-vf_x+uf_y.
$$

Taking a second [partial derivative](../../../../../../partial-derivative.md) in each variable, with the [partial derivatives](../../../../../../partial-derivative.md) of $f$ evaluated at $(x(u,v),y(u,v))$, gives

$$
\begin{aligned}
g_{uu}&=f_x+u^2f_{xx}+uv(f_{xy}+f_{yx})+v^2f_{yy},\\
g_{vv}&=-f_x+v^2f_{xx}-uv(f_{xy}+f_{yx})+u^2f_{yy}.
\end{aligned}
$$

The [mixed partial derivatives](../../../../../../mixed-partial-derivative.md) cancel even without using their equality. Hence the [Laplacians](../../../../../../laplacian.md) satisfy

$$
\boxed{g_{uu}+g_{vv}=(u^2+v^2)(f_{xx}+f_{yy}).}
$$

Away from the origin the factor $u^2+v^2$ is positive, so **$g$ is a [harmonic function](../../../../../../harmonic-function.md) if and only if $f$ is a [harmonic function](../../../../../../harmonic-function.md)** on the corresponding local coordinate patch. This is the [Laplacian in planar parabolic coordinates](../../../../../../laplacian-in-planar-parabolic-coordinates.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [Mathematics III](../../../mathematics-iii-split.md)
4. [Prelims](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
