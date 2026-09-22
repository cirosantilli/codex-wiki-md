<h1 id="12a/solution">Solution</h1>

↑ **Parent:** [12A](../12a.md)

For a regular [parametrized surface](../../../../../parametrized-surface.md) $\sigma(u,v)$, the [first fundamental form](../../../../../first-fundamental-form.md) is the induced metric

$$
I=E\,du^2+2F\,du\,dv+G\,dv^2,\qquad E=\sigma_u\cdot\sigma_u,\quad F=\sigma_u\cdot\sigma_v,\quad G=\sigma_v\cdot\sigma_v.
$$

Choose the [unit normal](../../../../../unit-normal.md) $N=(\sigma_u\times\sigma_v)/|\sigma_u\times\sigma_v|$. With the convention $II_{ij}=N\cdot\sigma_{ij}$, the [second fundamental form](../../../../../second-fundamental-form-split.md) is

$$
II=e\,du^2+2f\,du\,dv+g\,dv^2,\qquad e=N\cdot\sigma_{uu},\quad f=N\cdot\sigma_{uv},\quad g=N\cdot\sigma_{vv}.
$$

The [Gaussian curvature](../../../../../gaussian-curvature.md), the product of the [principal curvatures](../../../../../principal-curvature.md), is

$$
\boxed{K=\frac{eg-f^2}{EG-F^2}.}
$$

For a compact [smooth embedded surface](../../../../../smooth-embedded-surface.md) without boundary, the [Gauss-Bonnet theorem](../../../../../gauss-bonnet-theorem.md) gives

$$
\boxed{\int_S K\,dA=2\pi e(S),}
$$

where $e(S)$ is the [Euler characteristic](../../../../../euler-characteristic.md). The no-boundary condition is needed for this form; a [smooth embedded surface](../../../../../smooth-embedded-surface.md) with boundary has the additional boundary [geodesic curvature](../../../../../geodesic-curvature.md) integral.

For the [surface of revolution](../../../../../surface-of-revolution.md), use

$$
\sigma(u,v)=\bigl((r+a\sin u)\cos v,(r+a\sin u)\sin v,b\cos u\bigr).
$$

The parameters are periodic, with local open parameter rectangles providing the [coordinate charts](../../../../../manifold-chart.md). Put $R=r+a\sin u$ and $D=\sqrt{a^2\cos^2u+b^2\sin^2u}$. Since $r>a>0$ and $b>0$, both $R$ and $D$ are positive. The tangent vectors are

$$
\sigma_u=(a\cos u\cos v,a\cos u\sin v,-b\sin u),\qquad\sigma_v=(-R\sin v,R\cos v,0).
$$

Their [inner products](../../../../../inner-product.md) are $E=D^2$, $F=0$, and $G=R^2$. Thus

$$
\boxed{I=(a^2\cos^2u+b^2\sin^2u)\,du^2+(r+a\sin u)^2\,dv^2.}
$$

Their [cross product](../../../../../cross-product.md) is $R(b\sin u\cos v,b\sin u\sin v,a\cos u)$, so its normalization gives the outward [unit normal](../../../../../unit-normal.md)

$$
N=\frac1D(b\sin u\cos v,b\sin u\sin v,a\cos u).
$$

Next,

$$
\begin{aligned}
\sigma_{uu}&=(-a\sin u\cos v,-a\sin u\sin v,-b\cos u),\\
\sigma_{uv}&=(-a\cos u\sin v,a\cos u\cos v,0),\\
\sigma_{vv}&=(-R\cos v,-R\sin v,0).
\end{aligned}
$$

Taking their [inner products](../../../../../inner-product.md) with $N$ yields $e=-ab/D$, $f=0$, and $g=-bR\sin u/D$. Hence the [fundamental forms of an elliptic ring torus](../../../../../fundamental-forms-of-an-elliptic-ring-torus.md) give

$$
\boxed{II=-\frac{ab}{\sqrt{a^2\cos^2u+b^2\sin^2u}}\,du^2-\frac{b(r+a\sin u)\sin u}{\sqrt{a^2\cos^2u+b^2\sin^2u}}\,dv^2.}
$$

Choosing the inward [unit normal](../../../../../unit-normal.md) changes both displayed coefficients of $II$ to their negatives and leaves $I$ and $K$ unchanged. As a consistency check, $K=ab^2\sin u/(RD^4)$; its integral over the [torus](../../../../../torus.md) is zero, since $K\,dA=ab^2\sin u\,du\,dv/D^3$ cancels under $u\mapsto u+\pi$. This agrees with $e(S)=0$ in the [Gauss-Bonnet theorem](../../../../../gauss-bonnet-theorem.md).

## ↑ Ancestors (10)

1. [12A](../12a.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
