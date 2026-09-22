<h1 id="5d/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

An [integrating factor for a differential one-form](../../../../../../integrating-factor-for-a-differential-one-form.md) makes the multiplied form exact. If $dF=\mu g\,dx+\mu f\,dy$, then $F_x=\mu g$ and $F_y=\mu f$. Equality of the mixed [partial derivatives](../../../../../../partial-derivative.md) yields

$$
\boxed{\partial_x(\mu f)=\partial_y(\mu g).}
$$

This is a local compatibility condition under the usual smoothness assumptions.

For the trigonometric equation, where its coefficients are defined and division is legitimate, the slope is $y'=\tan x\tan y$. In the first quadrant it is positive, small near either axis and large near the upper-right corner. The [direction field](../../../../../../direction-field.md) below uses normalized line segments, so steep directions remain visible.

Multiplication by $\sin x\cos y$ gives

$$
\cos x\cos y\,dy-\sin x\sin y\,dx=d(\cos x\sin y)=0.
$$

Thus the multiplying function is an [integrating factor](../../../../../../integrating-factor.md), and the implicit [general solution](../../../../../../general-solution.md) is

$$
\boxed{\cos x\sin y=C.}
$$

In the larger square, $\cos x\ge0$. The positive-$C$ curves have positive $y$ and are symmetric about the $y$-axis; the negative-$C$ curves are their reflections. For $0<|C|<1$, a graph representation is

$$
y=\arcsin(C\sec x),\qquad |x|<\arccos|C|,
$$

with endpoints tending to $y=\operatorname{sgn}(C)\pi/2$. The $C=0$ interior curve is $y=0$. The domain boundaries include singular coefficients or zeros of the [integrating factor](../../../../../../integrating-factor.md), so these endpoint limits and smooth continuations through $x=0$ describe the regularized relation; they must not be mistaken for additional solutions of the literal original equation at undefined points.

<a id="5d/a/image-trigonometric-direction-field-regularized-implicit-solution-family-and-the-positive-higher-order-particular-solution"></a>
![](../../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/ia/paper-2-integrating-factor.png)

**[Figure 2](#5d/a/image-trigonometric-direction-field-regularized-implicit-solution-family-and-the-positive-higher-order-particular-solution). Trigonometric direction field, regularized implicit solution family, and the positive higher-order particular solution**.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5D](../../5d.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
