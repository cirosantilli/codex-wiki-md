<h1 id="1/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [velocity](../../../../../velocity.md) of a [fluid element](../../../../../fluid-element.md) is the [time derivative](../../../../../time-derivative.md) of its position with its [Lagrangian coordinates](../../../../../lagrangian-coordinate.md) $X,Y$ held fixed. Direct [differentiation](../../../../../differentiation.md) gives

$$
\begin{aligned}
\dot x&=-e^{-t}(X\cos\Omega t+Y\sin\Omega t)
+\Omega e^{-t}(Y\cos\Omega t-X\sin\Omega t)
=-x+\Omega e^{-2t}y,\\
\dot y&=e^t(Y\cos\Omega t-X\sin\Omega t)
-\Omega e^t(X\cos\Omega t+Y\sin\Omega t)
=y-\Omega e^{2t}x.
\end{aligned}
$$

Replacing the [Lagrangian coordinates](../../../../../lagrangian-coordinate.md) by the current [Eulerian coordinates](../../../../../eulerian-coordinate.md) therefore gives the [velocity field](../../../../../velocity-field.md)

$$
\boxed{\mathbf u(x,y,t)=(-x+\Omega e^{-2t}y,\ y-\Omega e^{2t}x)}.
$$

The distinction between following a [fluid element](../../../../../fluid-element.md) and differentiating at fixed [Eulerian coordinates](../../../../../eulerian-coordinate.md) is what connects the given [deformation map](../../../../../deformation-map.md) to this [velocity field](../../../../../velocity-field.md).

## ↑ Ancestors (13)

1. [I](../i.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the fluids and waves course of the University of Oxford](../../../../split.md)
6. [Fluids and waves course of the University of Oxford](../../../../../fluids-and-waves-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
