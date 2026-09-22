<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For positive bounds, [integration by parts](../../../../../integration-by-parts.md) with $u=\log x$ and $dv=x^2dx$ gives

$$
\boxed{F(a,b)=\left[\frac{x^3}{3}\log x-\frac{x^3}{9}\right]_{a}^{b}.}
$$

For negative bounds, specify the [complex logarithm on the negative real axis](../../../../../complex-logarithm-on-the-negative-real-axis.md). With argument $\pi$, namely the upper-bank boundary value of the [principal logarithm](../../../../../principal-complex-logarithm.md), $\log x=\log(-x)+i\pi$. Substitute $t=-x$ in the real part:

$$
\boxed{\int_c^d x^2\log x\,dx=F(-d,-c)+\frac{i\pi}{3}(d^3-c^3).}
$$

More generally, a continuous branch taking argument $(2k+1)\pi$ replaces $i\pi$ by $(2k+1)i\pi$. The imaginary part depends on that choice. The analytic principal branch excludes the negative axis itself, so the boundary-value convention is part of this interpretation.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [5](../../5.md)
3. [Discrete mathematics, continuous mathematics and probability](../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
4. [2017](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
