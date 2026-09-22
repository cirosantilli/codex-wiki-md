<h1 id="2d/solution">Solution</h1>

↑ **Parent:** [2D](../2d.md)

This is a [separable differential equation](../../../../../separable-differential-equation.md). On the solution with $y<1$, integration from the [initial condition](../../../../../initial-condition.md) gives

$$
\int_0^y\frac{dv}{\sqrt{1-v^2}}=\int_0^x\frac{u\,du}{\sqrt{1-u^2}},\qquad \arcsin y=1-\sqrt{1-x^2}.
$$

The right side lies in $[0,1)$, so taking its sine stays on the required branch. **The solution is**

$$
\boxed{y(x)=\sin\left(1-\sqrt{1-x^2}\right),\quad 0\le x<1.}
$$

Near the origin, $1-\sqrt{1-x^2}=x^2/2+O(x^4)$, so $y=x^2/2+O(x^4)$ and the [tangent line](../../../../../tangent-line.md) is horizontal. At the other end, $y\to\sin1$, while

$$
y'=\frac{x\cos(1-\sqrt{1-x^2})}{\sqrt{1-x^2}}\longrightarrow+\infty.
$$

Thus the curve has a vertical limiting [tangent line](../../../../../tangent-line.md) as $x\uparrow1$, even though $x=1$ is excluded from the domain.

For the [direction field](../../../../../direction-field.md), the slope is nonnegative everywhere in the square. The segments are horizontal on $x=0$ and on $y=1$, become steeper as $x$ increases at fixed $y<1$, and become flatter as $y$ increases at fixed $x$. Near $x=1$ they are almost vertical unless $y$ is correspondingly close to one. The excluded corner $(1,1)$ has no single limiting slope: the ratio $(1-y^2)/(1-x^2)$ depends on the path of approach.

<a id="2d/image-positive-slope-field-and-the-solution-from-the-origin-with-its-horizontal-and-vertical-limiting-tangents"></a>
![](../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ia/paper-2-direction-field.png)

**[Figure 1](#2d/image-positive-slope-field-and-the-solution-from-the-origin-with-its-horizontal-and-vertical-limiting-tangents). Positive slope field and the solution from the origin, with its horizontal and vertical limiting tangents**.

## ↑ Ancestors (10)

1. [2D](../2d.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
