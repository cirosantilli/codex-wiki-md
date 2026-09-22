<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The stability convention matters. The [Cambridge numerical analysis notes](https://www.damtp.cam.ac.uk/user/na/PartIB/Lect10.pdf) define a [strict linear stability domain](../../../../../../strict-linear-stability-domain.md) through decay $y_n\to0$. For a multistep recurrence, robust decay requires every [amplification root](../../../../../../amplification-root.md) to lie strictly inside the [unit disk](../../../../../../unit-disk.md). With that convention we can prove the stronger result that **this method's strict linear stability domain is empty**, and therefore bounded. Mere boundedness of oscillatory sequences gives a different answer, described below.

On the [Dahlquist test equation](../../../../../../dahlquist-test-equation.md), $g(y)=\lambda^2y$. With $z=h\lambda$, the [amplification polynomial of a multistep method](../../../../../../amplification-polynomial-of-a-multistep-method.md) is

$$
D\xi^2-16z\xi-A=0,\qquad D=z^2-7z+15,\qquad A=z^2+7z+15.
$$

Exclude $D=0$, where the intended two-step update cannot be solved. If both [polynomial roots](../../../../../../root-of-a-polynomial.md) have [modulus](../../../../../../modulus.md) below one, their product requires $|A|<|D|$. But

$$
|A|^2-|D|^2=28\operatorname{Re}z\,(|z|^2+15),
$$

so necessarily $\operatorname{Re}z<0$. The [complex quadratic Schur criterion](../../../../../../complex-quadratic-schur-criterion.md) also requires

$$
|\overline D(-16z)-(-A)(-16\overline z)|<|D|^2-|A|^2.
$$

Its left-hand side equals $32|\operatorname{Re}z|(|z|^2+15)$, while for $\operatorname{Re}z<0$ its right-hand side is only $28|\operatorname{Re}z|(|z|^2+15)$. The inequality is impossible. Thus

$$
\boxed{\mathcal D_{\rm decay}=\varnothing}.
$$

For comparison, the [bounded-root stability set of the symmetric two-derivative formula](../../../../../../bounded-root-stability-set-of-the-symmetric-two-derivative-formula.md) is unbounded. On $z=iy$, rotate the [amplification polynomial](../../../../../../amplification-polynomial-of-a-multistep-method.md) into a real reciprocal quadratic. Its two roots are distinct and on the [unit circle](../../../../../../complex-unit-circle.md) precisely when

$$
(15-y^2)^2-15y^2>0,
$$

equivalently $y^2<(45-15\sqrt5)/2$ or $y^2>(45+15\sqrt5)/2$. In particular, arbitrarily large imaginary parameters give bounded, undamped numerical oscillations. At the two equality thresholds, repeated [unit-circle roots](../../../../../../unit-circle-root.md) produce unbounded solutions. Hence the question's bounded-domain claim holds for the strict decay convention; it does not hold if the phrase is interpreted using the non-growing [root condition for a multistep method](../../../../../../root-condition-for-a-multistep-method.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 69](../../../paper-69-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
