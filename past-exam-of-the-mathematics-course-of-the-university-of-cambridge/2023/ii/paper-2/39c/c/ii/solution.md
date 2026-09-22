<h1 id="39c/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For the outer flow from part (i), the [rate-of-strain tensor](../../../../../../../strain-rate-tensor.md) in polar coordinates has components

$$
e_{rr}=-\frac{2Ua^2}{r^3}\cos\theta,
\qquad
e_{\theta\theta}=\frac{2Ua^2}{r^3}\cos\theta,
\qquad
e_{r\theta}=-\frac{2Ua^2}{r^3}\sin\theta.
$$

Therefore

$$
\mathbf e:\mathbf e
=e_{rr}^2+e_{\theta\theta}^2+2e_{r\theta}^2
=\frac{8U^2a^4}{r^6}.
$$

The leading dissipation per unit axial length is

$$
\begin{aligned}
\mathcal D
&=2\mu\int_a^\infty\int_0^{2\pi}
\mathbf e:\mathbf e\,r\,d\theta\,dr\\
&=16\mu U^2a^4(2\pi)
\int_a^\infty r^{-5}\,dr\\
&=8\pi\mu U^2.
\end{aligned}
$$

Balancing this with drag power $DU$ gives the [drag on a two-dimensional circular bubble from outer-flow dissipation](../../../../../../../drag-on-a-two-dimensional-circular-bubble-from-outer-flow-dissipation.md)

$$
\boxed{D=8\pi\mu U}
$$

per unit axial length, directed opposite to the bubble velocity.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [39C](../../../39c.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [Ii](../../../../split.md)
6. [2023](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
