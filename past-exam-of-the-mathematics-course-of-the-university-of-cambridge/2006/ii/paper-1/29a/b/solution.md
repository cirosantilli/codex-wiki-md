<h1 id="29a/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Characteristics satisfy $dx/ds=1$, $dy/ds=x$, $du/ds=0$. From $(\xi,0)$ they are $x=\xi+s$, $y=\xi s+s^2/2$, $u=f(\xi)$, so $x^2-2y=\xi^2$. The initial parameter is recovered on the two initial half-axes by

$$
\boxed{u(x,y)=f\left(\operatorname{sgn}(x)\sqrt{x^2-2y}\right),\qquad x\ne0,\quad y<x^2/2.}
$$

This is $C^1$ on the displayed [open set](../../../../../../open-set.md), takes the prescribed data at $y=0,x\ne0$, and substitution verifies $u_x+xu_y=0$. Each branch may extend separately beyond this chosen domain, but arbitrary data on both half-axes need not allow one common extension.

The initial line has normal $(0,1)$; the transport field is $(1,x)$, whose normal component is $x$. Thus it is non-characteristic exactly away from the origin. At the origin the equation itself would require $u_x(0,0)=f'(0)=0$. For generic $f$ this fails, so a $C^1$ solution on a neighborhood of the entire initial line is not guaranteed. The parabola $y=x^2/2$ is the envelope where the recovery of $\xi$ degenerates. Characteristics can also meet both initial half-axes, imposing compatibility such as $f(\xi)=f(-\xi)$ on an attempted larger domain.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [29A](../../29a.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
