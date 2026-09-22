<h1 id="4/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For the [composite trapezoidal rule](../../../../../../composite-trapezoidal-rule.md), the mesh width is $h=1/N$ and the nodes are $x_n=n/N$. The endpoint weights are halves and the interior weights are ones, so

$$
\boxed{T_N=\frac1N\left[\frac{3(0)^2}{2}+\sum_{n=1}^{N-1}3\left(\frac nN\right)^2+\frac{3(1)^2}{2}\right]
=\frac3{N^3}\sum_{n=1}^{N-1}n^2+\frac3{2N}.}
$$

This formula is an approximation to the [definite integral](../../../../../../definite-integral.md), not an exact equality with it for finite $N$.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [4](../../../4.md)
4. [Discrete mathematics, continuous mathematics, and probability (resit)](../../../../discrete-mathematics-continuous-mathematics-and-probability-resit-split.md)
5. [2015](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
