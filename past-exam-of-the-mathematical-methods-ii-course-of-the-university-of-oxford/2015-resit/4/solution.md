<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The proposed linear [change of variables](../../../change-of-variables-formula.md) makes the two pairs of boundary lines constant-coordinate lines: $v=1,4$ and $u=0,7$. Thus the image of the [parallelogram](../../../parallelogram.md) is the rectangle $0\le u\le7$, $1\le v\le4$.

The forward [Jacobian matrix](../../../jacobian-matrix.md) and its [determinant](../../../determinant.md) are

$$
\frac{\partial(u,v)}{\partial(x,y)}=\begin{pmatrix}1&-3\\2&1\end{pmatrix},\qquad\det=7.
$$

Inverting gives $x=(u+3v)/7$, $y=(v-2u)/7$, so the area element is $dx\,dy=\tfrac17du\,dv$. The absolute inverse [Jacobian determinant](../../../jacobian-determinant.md), rather than the forward determinant, belongs in the transformed area integral. Consequently

$$
\begin{aligned}
\iint_D\frac{x-3y}{2x+y}\,dx\,dy&=\frac17\int_0^7\int_1^4\frac uv\,dv\,du\\
&=\frac17\left[\frac{u^2}{2}\right]_0^7[\log v]_1^4,
\end{aligned}
$$

which yields $\boxed{\tfrac72\log4=7\log2}$. The transformed denominator is bounded below by one throughout the region, so no singular or improper integral is involved.

## ↑ Ancestors (11)

1. [4](../4.md)
2. [2015 resit](../../2015-resit-split.md)
3. [Past exam of the mathematical methods II course of the University of Oxford](../../split.md)
4. [Mathematical methods II course of the University of Oxford](../../../mathematical-methods-ii-course-of-the-university-of-oxford.md)
5. [Year 1 of the physics course of the University of Oxford](../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
