<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the [parametric curve](../../../../../../parametric-curve.md)

$$
X=2\sqrt2\cos t,\quad Y=\sqrt2\sin t,\qquad x(t)=2\cos t+\sin t,\quad y(t)=-2\cos t+\sin t,\quad 0\leq t\leq2\pi.
$$

Here $|y(t)|\leq\sqrt5<3$, so the [ellipse](../../../../../../ellipse.md) stays strictly above the [axis of rotation](../../../../../../axis-of-rotation.md) $y=-3$. Rotating in three dimensions gives a [surface of revolution](../../../../../../surface-of-revolution.md) with [parametrization](../../../../../../parametric-equation.md)

$$
\mathbf s(t,\varphi)=\bigl(x(t),-3+(y(t)+3)\cos\varphi,(y(t)+3)\sin\varphi\bigr),\qquad 0\leq\varphi\leq2\pi.
$$

The two parameter [tangent vectors](../../../../../../tangent-vector-split.md) are [orthogonal](../../../../../../orthogonal-vectors.md), with [Euclidean norms](../../../../../../euclidean-norm.md) $\sqrt{x'(t)^2+y'(t)^2}$ and $y(t)+3$. Hence the [area element of a surface](../../../../../../area-element-of-a-surface.md) is

$$
|\mathbf s_t\times\mathbf s_\varphi|=(y(t)+3)\sqrt{x'(t)^2+y'(t)^2}.
$$

The generating [ellipse](../../../../../../ellipse.md) is simple and has positive distance from the [axis of rotation](../../../../../../axis-of-rotation.md); its [rotation](../../../../../../rotation-mathematics.md) sweeps the [surface](../../../../../../topological-surface-split.md) once, apart from the identified parameter endpoints. Also

$$
x'(t)^2+y'(t)^2=(-2\sin t+\cos t)^2+(2\sin t+\cos t)^2=8\sin^2t+2\cos^2t.
$$

Writing $w(t)=\sqrt{8\sin^2t+2\cos^2t}$, the [surface area](../../../../../../surface-area.md) is therefore $2\pi\int_0^{2\pi}(3+y(t))w(t)\,dt$. Since $y(t+\pi)=-y(t)$ and $w(t+\pi)=w(t)$,

$$
\int_0^{2\pi}y(t)w(t)\,dt=\int_0^\pi\bigl(y(t)w(t)+y(t+\pi)w(t+\pi)\bigr)\,dt=0.
$$

Consequently

$$
\boxed{\operatorname{Area}(S)=6\pi\int_0^{2\pi}\sqrt{8\sin^2t+2\cos^2t}\,dt.}
$$

The cancellation is an instance of the [surface area of revolution of a centrally symmetric curve](../../../../../../surface-area-of-revolution-of-a-centrally-symmetric-curve.md): the [surface area](../../../../../../surface-area.md) is the generating curve’s [arc length](../../../../../../arc-length.md) times the distance $6\pi$ traveled by its center.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
3. [Mathematics IV resit](../../../mathematics-iv-resit-split.md)
4. [Prelims](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
