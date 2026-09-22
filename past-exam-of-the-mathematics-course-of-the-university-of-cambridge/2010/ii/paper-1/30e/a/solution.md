<h1 id="30e/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [characteristic equations for a transport equation](../../../../../../characteristic-equations-for-a-transport-equation.md) are $\dot x_1=x_1$, $\dot x_2=2x_2$, $\dot u=5u$. Starting from $(\xi,1)$ at parameter zero gives $(x_1,x_2)=(\xi e^s,e^{2s})$, $u=e^{5s}g(\xi)$. Eliminating $s,\xi$ gives

$$
\boxed{u(x_1,x_2)=x_2^{5/2}g(x_1/\sqrt{x_2}),\qquad x_2>0.}
$$

Every point of this upper half-plane lies on exactly one characteristic from the initial line, so it is the maximal characteristic domain determined by the data. Neither the line $x_2=0$ nor the lower half-plane is reached in finite characteristic time; extra data would be needed there.

For $g\in C^1$ this is a classical solution, directly verified by differentiation. The printed assumption is only continuity, which in general does not give a classical $C^1$ solution. Under that assumption the same formula is the unique continuous characteristic solution and solves the transport equation distributionally; smoothing $g$ locally and passing to limits verifies the latter interpretation. A classical interpretation needs the additional regularity just stated.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [30E](../../30e.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
