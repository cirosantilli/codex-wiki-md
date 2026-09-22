<h1 id="s1/3/3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

First remove the removable singularities introduced by tangent and secant: the integrand is $\cos\theta/(3+\cos\theta+2\sin\theta)$. The denominator stays positive since $3>\sqrt5$. With $z=e^{i\theta}$ the [contour](../../../../../complex-integration-contour.md) integrand is

$$
\frac{z^2+1}{iz\{(1-2i)z^2+6z+(1+2i)\}}.
$$

Its interior [poles](../../../../../pole.md) are zero and $r=-1/(1-2i)$; the other quadratic root is $-5/(1-2i)$ and lies outside. The [residues](../../../../../residue.md) are $1/[i(1+2i)]$ and $(r^2+1)/(4ir)$, whose sum is $i/10$. Consequently

$$
\boxed{\int_0^{2\pi}\frac{d\theta}{1+2\tan\theta+3\sec\theta}=-\frac\pi5.}
$$

Assigning arbitrary finite values at the isolated removable points does not change the [integral](../../../../../integral-split.md).

## ↑ Ancestors (12)

1. [3](../3.md)
2. [3](../../3.md)
3. [S1](../../../s1.md)
4. [2017](../../../../2017-split.md)
5. [Past exam of the short options paper shared by Prelims and Parts A and B of the physics course of the University of Oxford](../../../../split.md)
6. [Short options paper shared by Prelims and Parts A and B of the physics course of the University of Oxford](../../../../../short-options-paper-shared-by-prelims-and-parts-a-and-b-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
