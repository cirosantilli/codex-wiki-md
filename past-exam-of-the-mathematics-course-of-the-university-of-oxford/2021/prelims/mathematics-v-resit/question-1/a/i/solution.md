<h1 id="question-1/a/i/solution">Solution</h1>

↑ **Parent:** [i](../i.md)

Use [polar coordinates](../../../../../../../polar-coordinates.md) with $0\leq r\leq\sin^2\theta$ and $0\leq\theta\leq\pi$. The [Jacobian determinant](../../../../../../../jacobian-determinant.md) gives $dA=r\,dr\,d\theta$, so the [area](../../../../../../../surface-area.md) is

$$
A=\iint_R1\,dA
=\int_0^\pi\int_0^{\sin^2\theta}r\,dr\,d\theta
=\frac12\int_0^\pi\sin^4\theta\,d\theta.
$$

The [trigonometric identity](../../../../../../../trigonometric-identity.md)

$$
\sin^4\theta=\frac{3-4\cos(2\theta)+\cos(4\theta)}8
$$

reduces the [integral](../../../../../../../integral-split.md) to its constant term: both [cosine](../../../../../../../cosine.md) terms have zero [integral](../../../../../../../integral-split.md) over this interval. Therefore

$$
\boxed{\operatorname{Area}(R)=\frac{3\pi}{16}}.
$$

## ↑ Ancestors (13)

1. [i](../i.md)
2. [a](../../a.md)
3. [Question 1](../../../question-1.md)
4. [Mathematics V resit](../../../../mathematics-v-resit-split.md)
5. [Prelims](../../../../split.md)
6. [2021](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
