<h1 id="9/solution">Solution</h1>

↑ **Parent:** [9](../9.md)

Introduce a characteristic parameter $s$ and label each point of the initial segment by $r\in[0,1]$. The [method of characteristics](../../../method-of-characteristics.md) gives

$$
\frac{dx}{ds}=x-2,\qquad\frac{dy}{ds}=y,\qquad\frac{dz}{ds}=y,
\qquad (x,y,z)|_{s=0}=(1,r,1).
$$

Integrating gives the parametric solution

$$
\boxed{x=2-e^s,\qquad y=re^s,\qquad z=1+r(e^s-1),\quad s\in\mathbb R,\quad0\leq r\leq1.}
$$

The projected [characteristic curves](../../../characteristic-curve.md) satisfy $y=r(2-x)$, so each lies on a straight line through $(2,0)$. Its branch from the data always has $x<2$; the common vertex is approached only as $s\to-\infty$.

Eliminating $s,r$ using $e^s=2-x$ and $r=y/(2-x)$ yields

$$
\boxed{z(x,y)=1+y-\frac{y}{2-x}=1+\frac{y(1-x)}{2-x}.}
$$

Its derivatives give $(x-2)z_x+yz_y=y$, and substitution of $x=1$ gives the prescribed value one.

The [Jacobian determinant](../../../jacobian-determinant.md) of $(s,r)\mapsto(x,y)$ is $-e^{2s}\ne0$, and the inverse just displayed is unique. Hence the data determine the solution exactly on

$$
\boxed{\{(x,y):x<2,\ 0\leq y\leq2-x\}.}
$$

This is the [domain determined by a finite segment under a radial characteristic flow](../../../domain-determined-by-a-finite-segment-under-a-radial-characteristic-flow.md). Its interior is $x<2$, $0<y<2-x$; the two boundary rays come from the endpoints of the initial segment. Every point there lies on exactly one characteristic from the data. Outside this sector, a characteristic either misses the initial segment or lies on the branch $x>2$, which cannot reach it. Thus the formula may be extended beyond this sector, but such an extension is not uniquely specified by the given data.

## ↑ Ancestors (11)

1. [9](../9.md)
2. [2011](../../2011-split.md)
3. [Past exam of the algebra, analysis and differential equations 1 course of the University of Oxford](../../split.md)
4. [Algebra, analysis and differential equations 1 course of the University of Oxford](../../../algebra-analysis-and-differential-equations-1-course-of-the-university-of-oxford.md)
5. [Year 2 of the mathematics course of the University of Oxford](../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
6. [Mathematics course of the University of Oxford](../../../mathematics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
