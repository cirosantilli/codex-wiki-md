<h1 id="s1/1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Parametrize the positively oriented unit [circle](../../../../../circle.md) by $z=e^{i\theta}$. Then $e^{-1/z}=e^{-\cos\theta+i\sin\theta}$ and $dz=ie^{i\theta}d\theta$, so

$$
\oint_Ce^{-1/z}dz
=i\int_0^{2\pi}e^{-\cos\theta}\cos(\theta+\sin\theta)d\theta
-\int_0^{2\pi}e^{-\cos\theta}\sin(\theta+\sin\theta)d\theta.
$$

Equating the [real part](../../../../../real-part.md) and [imaginary part](../../../../../imaginary-part.md) with $-2\pi i$ gives

$$
\boxed{\int_0^{2\pi}e^{-\cos\theta}\cos(\theta+\sin\theta)d\theta=-2\pi,\qquad
\int_0^{2\pi}e^{-\cos\theta}\sin(\theta+\sin\theta)d\theta=0.}
$$

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [S1](../../../s1.md)
4. [2012](../../../../2012-split.md)
5. [Past exam of the short options paper shared by Prelims and Parts A and B of the physics course of the University of Oxford](../../../../split.md)
6. [Short options paper shared by Prelims and Parts A and B of the physics course of the University of Oxford](../../../../../short-options-paper-shared-by-prelims-and-parts-a-and-b-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
