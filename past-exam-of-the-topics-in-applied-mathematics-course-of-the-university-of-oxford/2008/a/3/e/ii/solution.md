<h1 id="a/3/e/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [first integral](../../../../../../first-integral.md) and $b_0=1$ yield the linear identity $b'+cb=c(1-g)$. Multiply by the [integrating factor](../../../../../../integrating-factor.md) $e^{cy}$ and integrate from $-\infty$. Since the bounded limit $b(-\infty)=1$ makes $e^{cy}b(y)\to0$ there,

$$
b(y)=c\int_{-\infty}^{y}e^{-c(y-s)}(1-g(s))\,ds
=1-c\int_{-\infty}^{y}e^{-c(y-s)}g(s)\,ds.
$$

Positivity of $g$ makes the last [integral](../../../../../../integral-split.md) nonnegative, and strictly positive at any finite point of a strictly positive [travelling wave](../../../../../../travelling-wave.md). Thus

$$
\boxed{0<b(y)<b_0=1\quad\text{for finite }y,}
$$

with equality approached only at the far-behind boundary. This bound uses the [first integral](../../../../../../first-integral.md) rather than an unsupported assumption that the [bacterial](../../../../../../bacteria.md) profile is monotone.

## ↑ Ancestors (14)

1. [Ii](../ii.md)
2. [E](../../e.md)
3. [3](../../../3.md)
4. [A](../../../../a.md)
5. [2008](../../../../../2008-split.md)
6. [Past exam of the topics in applied mathematics course of the University of Oxford](../../../../../split.md)
7. [Topics in applied mathematics course of the University of Oxford](../../../../../../topics-in-applied-mathematics-course-of-the-university-of-oxford.md)
8. [Year 3 of the mathematics course of the University of Oxford](../../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
