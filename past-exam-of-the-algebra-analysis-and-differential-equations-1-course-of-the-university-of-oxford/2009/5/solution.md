<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

For $f=u+iv$, the [Cauchy-Riemann equations](../../../cauchy-riemann-equations.md) are $u_x=v_y$ and $u_y=-v_x$. Holomorphy implies these relations. Conversely, if the first partial derivatives exist and are continuous near a point, satisfying the equations there gives complex differentiability; satisfying them on an [open set](../../../open-set.md) gives a [holomorphic function](../../../holomorphic-function-split.md) on that set.

Let $r=\sqrt{x^2+y^2}$. On the cut plane, $r+x>0$: equality could occur only at a nonpositive real point, which is excluded. Thus $u=\sqrt{(r+x)/2}$ is strictly positive and $v=y/(2u)$ is well defined and smooth. Since $y^2=(r-x)(r+x)$,

$$
u^2=\frac{r+x}2,\qquad v^2=\frac{r-x}2,\qquad2uv=y.
$$

Consequently

$$
\boxed{(u+iv)^2=x+iy=z.}
$$

One can verify [holomorphy](../../../holomorphic-function-split.md) directly:

$$
u_x=\frac u{2r}=v_y,\qquad u_y=\frac v{2r}=-v_x.
$$

Here $r>0$ throughout the domain, so all partial derivatives are continuous. Therefore **$f$ is holomorphic**, specifically the [principal square root](../../../principal-square-root-of-a-complex-number.md) on the cut plane, with [derivative](../../../derivative.md) $f'(z)=1/[2f(z)]$.

## ↑ Ancestors (11)

1. [5](../5.md)
2. [2009](../../2009-split.md)
3. [Past exam of the algebra, analysis and differential equations 1 course of the University of Oxford](../../split.md)
4. [Algebra, analysis and differential equations 1 course of the University of Oxford](../../../algebra-analysis-and-differential-equations-1-course-of-the-university-of-oxford.md)
5. [Year 2 of the mathematics course of the University of Oxford](../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
6. [Mathematics course of the University of Oxford](../../../mathematics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
