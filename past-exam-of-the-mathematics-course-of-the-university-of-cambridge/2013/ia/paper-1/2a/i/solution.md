<h1 id="2a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Left multiplication by the given [Givens rotation](../../../../../../givens-rotation.md) mixes rows two and three, so $b_{31}=a_{21}\sin\theta_1+a_{31}\cos\theta_1$. If $r_1=\sqrt{a_{21}^2+a_{31}^2}>0$, choose

$$
\boxed{\cos\theta_1=\frac{a_{21}}{r_1},\qquad\sin\theta_1=-\frac{a_{31}}{r_1}.}
$$

Equivalently $\theta_1=\operatorname{atan2}(-a_{31},a_{21})$ modulo $2\pi$. Substitution gives $b_{31}=0$ and $b_{21}=r_1$. If $a_{21}=a_{31}=0$, take $\theta_1=0$; the desired zero is already present. This also covers singular matrices without division by zero.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2A](../../2a.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
