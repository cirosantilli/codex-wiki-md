<h1 id="12g/solution">Solution</h1>

↑ **Parent:** [12G](../12g.md)

Parametrize the graph by $X(u,v)=(u,v,f(u,v))$. The [first fundamental form](../../../../../first-fundamental-form.md) has coefficients $E=1+f_u^2$, $F=f_uf_v$, $G=1+f_v^2$. With unit normal $(-f_u,-f_v,1)/\sqrt{1+|\nabla f|^2}$, the [second fundamental form](../../../../../second-fundamental-form-split.md) has coefficients $e=f_{uu}/\sqrt{1+|\nabla f|^2}$, $f_{\rm II}=f_{uv}/\sqrt{1+|\nabla f|^2}$, and $g=f_{vv}/\sqrt{1+|\nabla f|^2}$. Consequently the [Gaussian curvature of a graph surface](../../../../../gaussian-curvature-of-a-graph-surface.md) is

$$
\boxed{K=\frac{eg-f_{\rm II}^2}{EG-F^2}
=\frac{f_{uu}f_{vv}-f_{uv}^2}{(1+f_u^2+f_v^2)^2}.}
$$

A compact embedded surface has a highest point in the vertical direction. At that point its tangent plane is horizontal, so it is locally a graph with a local maximum of $f$. Its [Hessian matrix](../../../../../hessian-matrix.md) is negative semidefinite, giving $\det D^2f\geq0$ and hence $K\geq0$. Thus the [Gaussian curvature](../../../../../gaussian-curvature.md) cannot be everywhere negative.

An embedded ring [torus](../../../../../torus.md), with major radius $R$ larger than minor radius $r>0$, is a compact surface without boundary. Its standard parametrization is $((R+r\cos\theta)\cos\phi,(R+r\cos\theta)\sin\phi,r\sin\theta)$, and the [Gaussian curvature of a ring torus](../../../../../gaussian-curvature-of-a-ring-torus.md) is

$$
\boxed{K=\frac{\cos\theta}{r(R+r\cos\theta)}.}
$$

Since the denominator is positive, curvature is positive on the outer side and negative on the inner side, so this example changes sign.

## ↑ Ancestors (10)

1. [12G](../12g.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
