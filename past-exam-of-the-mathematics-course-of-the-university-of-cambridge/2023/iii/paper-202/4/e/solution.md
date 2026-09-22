<h1 id="4/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

For $Y=X^\alpha$, the [Itô formula](../../../../../../ito-s-lemma.md) and the Bessel equation give

$$
dY_t=\alpha X_t^{\alpha-1}dB_t
+\frac{\alpha(d+\alpha-2)}2X_t^{\alpha-2}dt.
$$

Use the clock

$$
C_t=\alpha^2\int_0^tX_s^{2\alpha-2}ds
$$

and its inverse. The [Dambis-Dubins-Schwarz theorem](../../../../../../dambis-dubins-schwarz-theorem.md) turns the first term into Brownian motion, while division of the drift by the clock rate gives

$$
d\widetilde Y_u=dW_u+
\frac{d+\alpha-2}{2\alpha}\frac{du}{\widetilde Y_u}.
$$

Hence $\widetilde Y$ is a Bessel process of dimension

$$
d'=1+\frac{d+\alpha-2}{\alpha}
=2+\frac{d-2}{\alpha}.
$$

This is the [Power time change of a Bessel process](../../../../../../power-time-change-of-a-bessel-process.md).

## ↑ Ancestors (11)

1. [E](../e.md)
2. [4](../../4.md)
3. [Paper 202](../../../paper-202-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
