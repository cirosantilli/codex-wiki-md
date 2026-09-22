<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Set $C=\cos u$, $S=\sin u$, and $D=1+S^2=2-C^2$. At $v=0$, the first [partial derivatives](../../../../partial-derivative.md) are

$$
\mathbf r_u=(-S,C,0),\qquad\mathbf r_v=(-S,1+C,1).
$$

Their [dot products](../../../../dot-product.md) give $E=1$, $F=1+C$, $G=3+2C$. Hence

$$
\boxed{I=du^2+2(1+\cos u)\,du\,dv+(3+2\cos u)\,dv^2.}
$$

Since $EG-F^2=3+2C-(1+C)^2=D>0$, the [parametric surface](../../../../parametric-surface.md) is regular everywhere. Its [cross product](../../../../cross-product.md) and [unit normal](../../../../unit-normal.md) at $v=0$ are

$$
\mathbf r_u\times\mathbf r_v=(C,S,-S),\qquad N=\frac{(C,S,-S)}{\sqrt D}.
$$

The second [partial derivatives](../../../../partial-derivative.md) at $v=0$ are

$$
\mathbf r_{uu}=(-C,-S,0),\qquad
\mathbf r_{uv}=(-C,-S,0),\qquad
\mathbf r_{vv}=(-1-C,-S,0).
$$

Their [dot products](../../../../dot-product.md) with $N$ give $e=f=-1/\sqrt D$ and $g_2=-(1+C)/\sqrt D$. Thus

$$
\boxed{II=-\frac{du^2+2\,du\,dv+(1+\cos u)\,dv^2}{\sqrt{1+\sin^2u}}.}
$$

Part (b) transports these [first fundamental form](../../../../first-fundamental-form.md) and [second fundamental form](../../../../second-fundamental-form-split.md) coefficients to every $v$. Finally,

$$
\boxed{\kappa(u,v)=\frac{(1+C)/D-1/D}{D}=\frac{\cos u}{(1+\sin^2u)^2},\qquad dA=\sqrt{1+\sin^2u}\,du\,dv.}
$$

The last expression is the [surface area](../../../../surface-area.md) element from $\sqrt{EG-F^2}$. In particular the [Gaussian curvature](../../../../gaussian-curvature.md) changes sign where $\cos u$ does; it vanishes at $u=\pi/2$ modulo $\pi$.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the geometry of surfaces course of the University of Oxford](../../../split.md)
5. [Geometry of surfaces course of the University of Oxford](../../../../geometry-of-surfaces-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
