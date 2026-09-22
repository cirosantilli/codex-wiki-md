<h1 id="9/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

On $0<x<2$, $2x-x^2=x(2-x)>0$. A valid [probability density function](../../../../../../probability-density-function.md) must integrate to one, so

$$
1=\alpha\int_0^2(2x-x^2)\,dx=\alpha\left[x^2-\frac{x^3}{3}\right]_0^2=\frac43\alpha.
$$

Thus $\alpha=3/4$, which is positive and ensures nonnegativity. Its [expected value](../../../../../../expected-value-split.md) is

$$
\mathbb E[X]=\frac34\int_0^2(2x^2-x^3)\,dx=\frac34\left[\frac{2x^3}{3}-\frac{x^4}{4}\right]_0^2=1.
$$

Therefore

$$
\boxed{\text{Valid with }\alpha=\frac34,\qquad\mathbb E[X]=1.}
$$

The [probability density function](../../../../../../probability-density-function.md) is symmetric around $1$, providing a second check on the [expected value](../../../../../../expected-value-split.md).

## ↑ Ancestors (13)

1. [I](../i.md)
2. [A](../../a.md)
3. [9](../../../9.md)
4. [Discrete mathematics, probability and continuous mathematics](../../../../discrete-mathematics-probability-and-continuous-mathematics-split.md)
5. [2013](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
