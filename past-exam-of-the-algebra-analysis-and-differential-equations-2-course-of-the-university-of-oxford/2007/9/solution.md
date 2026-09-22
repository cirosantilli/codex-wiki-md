<h1 id="9/solution">Solution</h1>

↑ **Parent:** [9](../9.md)

A sufficient condition for existence of the [Laplace transform](../../../laplace-transform.md) is that $y$ be piecewise continuous on each bounded interval and have [exponential order](../../../exponential-order.md): $|y(t)|\le Ce^{at}$ for sufficiently large $t$. The defining integral then converges absolutely for real $p>a$, and more generally defines a [holomorphic function](../../../holomorphic-function-split.md) for complex $p$ with $\operatorname{Re}p>a$. The boundary $p=a$ may or may not be included, depending on $y$.

Write $Y(p)=\mathcal L[y](p)$. To solve the [differential equation](../../../differential-equation-split.md) by [Laplace transform](../../../laplace-transform.md), initially seek a sufficiently regular solution with $y(0)=1$ and finite $y'(0)=b$. The [Laplace transform of a derivative](../../../laplace-transform-of-a-derivative.md) gives

$$
\mathcal L[y']=pY-1,\qquad \mathcal L[y'']=p^2Y-p-b.
$$

Using $\mathcal L[ty]=-Y'$ from part (i), the transformed [differential equation](../../../differential-equation-split.md) becomes

$$
-(2pY+p^2Y'-1)-Y-pY'-(pY-1)-Y=0,
$$

or

$$
p(p+1)Y'+(3p+2)Y=2.
$$

After division by $p(p+1)$, an [integrating factor](../../../integrating-factor.md) is $p^2(p+1)$, since $(3p+2)/(p(p+1))=2/p+1/(p+1)$. Consequently

$$
\frac d{dp}\bigl[p^2(p+1)Y\bigr]=2p,\qquad
Y=\frac1{p+1}+\frac{C}{p^2(p+1)}.
$$

For a bounded $y$, $|Y(p)|\le\|y\|_\infty/p$ for $p>0$. Letting $p\downarrow0$ forces $C=0$, an instance of how [boundedness selects a Laplace transform at a singular endpoint](../../../boundedness-selects-a-laplace-transform-at-a-singular-endpoint.md). By the exponential formula in part (iii), this yields

$$
\boxed{y(t)=e^{-t}.}
$$

Direct substitution checks the [differential equation](../../../differential-equation-split.md), boundedness and the required limit.

To complete the uniqueness argument, no unproved endpoint regularity is needed. The two functions $e^{-t}$ and $t-1$ solve the homogeneous [linear differential equation](../../../linear-differential-equation.md) on $(0,\infty)$, and their [Wronskian](../../../wronskian.md) is $te^{-t}\ne0$. They form a [fundamental system of solutions](../../../fundamental-system-of-solutions.md) on that interval, so every classical solution is $Ae^{-t}+B(t-1)$. Boundedness forces $B=0$ and the limit at zero forces $A=1$. Thus **the bounded solution with the specified limit is unique**. The limit alone would not suffice: $e^{-t}+C(t-1+e^{-t})$ has the same limit for every $C$, but is unbounded when $C\ne0$.

## ↑ Ancestors (11)

1. [9](../9.md)
2. [2007](../../2007-split.md)
3. [Past exam of the algebra, analysis and differential equations II course of the University of Oxford](../../split.md)
4. [Algebra, analysis and differential equations II course of the University of Oxford](../../../algebra-analysis-and-differential-equations-ii-course-of-the-university-of-oxford.md)
5. [Year 2 of the mathematics course of the University of Oxford](../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
6. [Mathematics course of the University of Oxford](../../../mathematics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
