<h1 id="question-1/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

In [cylindrical coordinates](../../../../../../../cylindrical-coordinate-system.md), $(-y,x,0)=r\mathbf e_\theta$ and $x+r=r(1+\cos\theta)$. Hence the [vector field](../../../../../../../vector-field.md) simplifies to

$$
\mathbf F=\frac{\sqrt{1+\cos\theta}}{r}\mathbf e_\theta.
$$

Take the [orientation](../../../../../../../orientation-of-a-simplex.md) of $C$ to be increasing $\theta$, as in its given [parametrization](../../../../../../../parametric-equation.md). On the [circle](../../../../../../../circle.md), $d\mathbf r=a\mathbf e_\theta\,d\theta$, so its [line integral](../../../../../../../line-integral.md) is

$$
\int_C\mathbf F\cdot d\mathbf r
=\int_{-\pi}^{\pi}\sqrt{1+\cos\theta}\,d\theta
=\sqrt2\int_{-\pi}^{\pi}\cos(\theta/2)\,d\theta
=\boxed{4\sqrt2}.
$$

We used $\sqrt{1+\cos\theta}=\sqrt2|\cos(\theta/2)|$; the [cosine](../../../../../../../cosine.md) is nonnegative on this interval. In particular, the answer does not depend on $a$.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [Question 1](../../../question-1.md)
4. [Mathematics V resit](../../../../mathematics-v-resit-split.md)
5. [Prelims](../../../../split.md)
6. [2015](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
