<h1 id="4a/solution">Solution</h1>

↑ **Parent:** [4A](../4a.md)

Parametrize the positively oriented circle by $z=re^{i\theta}$. The [Cauchy derivative formula](../../../../../cauchy-derivative-formula.md) at the origin becomes

$$
f'(0)=\frac1{2\pi r}\int_0^{2\pi}f(re^{i\theta})e^{-i\theta}\,d\theta.
$$

Taking the complex conjugate of the [Cauchy integral theorem](../../../../../cauchy-s-integral-theorem.md) and using $d\bar z=-ir e^{-i\theta}\,d\theta$ gives

$$
0=-ir\int_0^{2\pi}\overline{f(re^{i\theta})}e^{-i\theta}\,d\theta.
$$

Add this zero integral to the derivative integral. Since $f+\bar f=2\operatorname{Re}f=2u$, [recovering an analytic derivative from the boundary real part](../../../../../recovering-an-analytic-derivative-from-the-boundary-real-part.md) yields

$$
\boxed{f'(0)=\frac1{\pi r}\int_0^{2\pi}u(\theta)e^{-i\theta}\,d\theta.}
$$

The [complex conjugation](../../../../../complex-conjugation.md) on the integrand and the reversed sign in $d\bar z$ are both required; the circle's orientation itself has not been reversed.

## ↑ Ancestors (10)

1. [4A](../4a.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
