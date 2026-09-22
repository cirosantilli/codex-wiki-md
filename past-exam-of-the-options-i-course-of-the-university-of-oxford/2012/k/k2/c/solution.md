<h1 id="k/k2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For a [point vortex in stagnation flow beside a wall](../../../../../point-vortex-in-stagnation-flow-beside-a-wall.md), a freely moving [point vortex](../../../../../line-vortex.md) is transported by the regular [velocity](../../../../../velocity.md) due to the background and its image, excluding its own singular [velocity](../../../../../velocity.md). Differentiate the potential and evaluate that regular part at $z_0=x+iy$:

$$
\dot x-i\dot y=z_0+\frac{i\Gamma}{2\pi(z_0-\overline z_0)}
=x+iy+\frac{\Gamma}{4\pi y}.
$$

Thus the equations of motion are

$$
\boxed{\dot x=x+\frac{\Gamma}{4\pi y},\qquad\dot y=-y.}
$$

Writing $c=\Gamma/(4\pi)$, differentiate the proposed path function:

$$
\frac d{dt}(xy+c\log y)=\left(x+\frac cy\right)y+x(-y)+c\frac{-y}{y}=0.
$$

Hence

$$
\boxed{xy+\frac{\Gamma}{4\pi}\log y=\text{constant}.}
$$

For initial position $(x_0,y_0)$, an explicit check is $y(t)=y_0e^{-t}$ and $x(t)=e^t(x_0+ct/y_0)$. Their substitution makes the linear terms in $t$ cancel in the path function and also shows that the vortex stays above the wall at every finite time.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [K2](../../k2.md)
3. [K](../../../k.md)
4. [2012](../../../../2012-split.md)
5. [Past exam of the options I course of the University of Oxford](../../../../split.md)
6. [Options I course of the University of Oxford](../../../../../options-i-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
