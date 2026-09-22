<h1 id="9/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Condition first on $X$. A [Poisson distribution](../../../../../../poisson-distribution.md) with parameter $k$ has conditional [probability generating function](../../../../../../probability-generating-function.md) $e^{k(s-1)}$, including the degenerate zero case when $k=0$. The [law of total expectation](../../../../../../law-of-total-expectation.md) gives

$$
G_Z(s)=\mathbb E\bigl[e^{X(s-1)}\bigr]=G_X(e^{s-1})=\boxed{\exp\!\left(\mu\bigl(e^{s-1}-1\bigr)\right)}.
$$

For $0\leq s\leq1$ the inner argument is in $(0,1]$, so this use of the generating function is justified directly. The result is a [compound Poisson distribution](../../../../../../compound-poisson-distribution.md) with a [Poisson distribution](../../../../../../poisson-distribution.md) of unit parameter for each jump, also called a [Neyman Type A distribution](../../../../../../neyman-type-a-distribution.md) in this case. It is generally not an ordinary [Poisson distribution](../../../../../../poisson-distribution.md).

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [9](../../../9.md)
4. [Discrete mathematics, continuous mathematics, and probability](../../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
5. [2018](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
