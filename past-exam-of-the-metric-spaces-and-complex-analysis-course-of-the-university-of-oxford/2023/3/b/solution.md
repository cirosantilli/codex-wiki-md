<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [b](../b.md)

A sufficient condition is that $U$ is a [connected space](../../../../connected-space.md). Suppose, towards a contradiction, that $|f|$ is the same constant $R$ throughout $U$. If $R=0$, then $f=0$, contradicting $f(a)\ne f(b)$.

If $R>0$, differentiate $u^2+v^2=R^2$ in $x$ and $y$, and use the [Cauchy-Riemann equations](../../../../cauchy-riemann-equations.md) from part (a). They give

$$
uu_x+vv_x=0,\qquad vu_x-uv_x=0.
$$

The coefficient [matrix](../../../../matrix.md) for $(u_x,v_x)$ has [determinant](../../../../determinant.md) $-(u^2+v^2)=-R^2\ne0$. Hence $u_x=v_x=0$, so $f'=0$ everywhere. A [holomorphic function](../../../../holomorphic-function-split.md) with zero [complex derivative](../../../../complex-derivative.md) is locally constant: within a small disc, differentiate along a straight segment. Local constancy and [connectedness](../../../../connected-space.md) imply constancy on $U$, again a contradiction.

Consequently,

$$
\boxed{U\text{ connected and }f(a)\ne f(b)\ \Longrightarrow\ \exists c,d\in U:\ |f(c)|\ne|f(d)|}.
$$

This is the [constant-modulus holomorphic function](../../../../constant-modulus-holomorphic-function.md) principle. The extra hypothesis matters: on two disjoint [open discs](../../../../open-disc.md), define $f=1$ on one and $f=-1$ on the other. It is [holomorphic](../../../../holomorphic-function-split.md) and nonconstant, yet $|f|=1$ everywhere.

## ↑ Ancestors (12)

1. [b](../b.md)
2. [3](../../3.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the metric spaces and complex analysis course of the University of Oxford](../../../split.md)
5. [Metric spaces and complex analysis course of the University of Oxford](../../../../metric-spaces-and-complex-analysis-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
