<h1 id="6/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

With [step size](../../../../../../step-size.md) $h=1/N$ and nodes $x_j=j/N$, the [composite trapezoidal rule](../../../../../../composite-trapezoidal-rule.md) gives

$$
\boxed{T_N=\frac1N\left[\frac12+
\sum_{j=1}^{N-1}\frac{1}{1+(j/N)^2}+\frac14\right]
=\frac{3}{4N}+\sum_{j=1}^{N-1}\frac{N}{N^2+j^2},\qquad I\approx T_N.}
$$

The endpoint weights are half the interior weights, and the endpoint values are $1$ and $1/2$.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [A](../../a.md)
3. [6](../../../6.md)
4. [Discrete mathematics, continuous mathematics, and probability](../../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
5. [2015](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
