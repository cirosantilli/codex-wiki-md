<h1 id="5/b/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

After the first update, the [sequence](../../../../../../sequence.md) lies in $[\sqrt a,x_1]$ and is nonincreasing. The [monotone convergence theorem for sequences](../../../../../../bounded-monotone-sequence-theorem.md) gives a [limit](../../../../../../limit-of-a-function.md) $L\geq\sqrt a$. The update is [continuous](../../../../../../continuous-function.md) on this interval, so passing to the [limit](../../../../../../limit-of-a-function.md) gives

$$
L=\frac12\left(L+\frac aL\right),\qquad L^2=a.
$$

Positivity forces $\boxed{x_n\to\sqrt a\text{ for every }x_0>0}$. If an iterate reaches the root exactly, the constant tail gives the same conclusion. The [Exact Newton error identity for a quadratic](../../../../../../exact-newton-error-identity-for-a-quadratic.md) here is $x_n-\sqrt a=(x_{n-1}-\sqrt a)^2/(2x_{n-1})$, also showing [quadratic convergence](../../../../../../quadratic-convergence.md) once the error is small.

## ↑ Ancestors (13)

1. [Iv](../iv.md)
2. [B](../../b.md)
3. [5](../../../5.md)
4. [Discrete mathematics, continuous mathematics and probability](../../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
5. [2014](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
