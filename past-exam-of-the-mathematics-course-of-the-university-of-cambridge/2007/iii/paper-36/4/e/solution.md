<h1 id="4/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

For any initial point, rotate its vector through the Brownian angle:

$$
\boxed{X_t=x_0\cos B_t-y_0\sin B_t,\qquad Y_t=x_0\sin B_t+y_0\cos B_t.}
$$

This is a nonanticipating function of the prescribed Brownian path and has the required initial value. Equivalently, $Z_t=X_t+iY_t=(x_0+iy_0)e^{iB_t}$. The [Itô formula](../../../../../../ito-s-lemma.md) gives $dZ_t=iZ_t\,dB_t-Z_t\,dt/2$, whose real and imaginary parts are exactly the equations in part c. Therefore the displayed formula is the [strong solution of a stochastic differential equation](../../../../../../strong-solution-of-a-stochastic-differential-equation.md), and uniqueness from part d makes it the only one.

The [Brownian rotation in the plane](../../../../../../brownian-rotation-in-the-plane.md) preserves radius: $X_t^2+Y_t^2=x_0^2+y_0^2$. Nonzero starting points move around their initial circle, and the origin remains fixed.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [4](../../4.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
