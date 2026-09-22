<h1 id="5a/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

At the first half-temperature time, the solution of [Newton's law of cooling](../../../../../../../newton-s-law-of-cooling.md) gives

$$
1+(\alpha-1)e^{-kt_1}=\frac\alpha2,\qquad \boxed{t_1=\frac1k\log\frac{2(\alpha-1)}{\alpha-2}.}
$$

Since $\alpha>2$, this time is positive and finite. The instantaneous temperature increase supplies the new [initial condition](../../../../../../../initial-condition.md) $T(t_1+)=\alpha T_0/2+\beta$. Restart the same [first-order linear differential equation](../../../../../../../first-order-linear-differential-equation.md) at $t_1$:

$$
\boxed{T(t)=T_0+\left[\left(\frac\alpha2-1\right)T_0+\beta\right]e^{-k(t-t_1)},\qquad t>t_1.}
$$

This is [Newton cooling with an instantaneous temperature jump](../../../../../../../newton-cooling-with-an-instantaneous-temperature-jump.md). The time translation in the [exponential decay](../../../../../../../exponential-decay.md) is essential: its prefactor is the excess immediately after the jump.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [5A](../../../5a.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [Ia](../../../../split.md)
6. [2016](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
