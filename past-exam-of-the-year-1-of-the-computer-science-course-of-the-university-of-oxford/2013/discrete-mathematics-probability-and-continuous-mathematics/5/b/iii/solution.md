<h1 id="5/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For $N$ equal intervals, the [composite trapezoidal rule](../../../../../../composite-trapezoidal-rule.md) is

$$
T_N=\frac1N\left[\frac12+\sum_{n=1}^{N-1}\left(\frac nN\right)^2\right]
=\frac1{N^3}\sum_{n=1}^{N-1}n^2+\frac1{2N}.
$$

Adding the missing $N^2/N^3$ term therefore gives the exact relation

$$
\frac1{N^3}\sum_{n=1}^N n^2=T_N+\frac1{2N}.
$$

Since $x^2$ is continuous, its [Riemann sums](../../../../../../riemann-sum.md), and hence its endpoint-averaged trapezoidal sums, converge to its [definite integral](../../../../../../definite-integral.md). Thus $T_N\to1/3$ and $1/(2N)\to0$, giving

$$
\boxed{\lim_{N\to\infty}\frac1{N^3}\sum_{n=1}^N n^2=\frac13.}
$$

No pre-existing formula for the sum of squares is needed.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [5](../../../5.md)
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
