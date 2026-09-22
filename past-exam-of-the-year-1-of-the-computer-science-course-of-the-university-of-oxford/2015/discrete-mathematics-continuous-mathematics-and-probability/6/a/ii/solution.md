<h1 id="6/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Write the sum in the question as the right [Riemann sum](../../../../../../riemann-sum.md)

$$
S_N=\sum_{j=1}^N\frac{N}{N^2+j^2}
=\frac1N\sum_{j=1}^N\frac{1}{1+(j/N)^2}.
$$

Relative to the [composite trapezoidal rule](../../../../../../composite-trapezoidal-rule.md), the only change is in the two endpoint weights:

$$
S_N-T_N=\frac{1}{2N}\bigl(f(1)-f(0)\bigr)=-\frac1{4N}.
$$

The [integrand](../../../../../../integrand.md) $f(x)=1/(1+x^2)$ is [continuous](../../../../../../continuous-function.md) on $[0,1]$, so $T_N\to I$. Since an [antiderivative](../../../../../../antiderivative.md) is $\arctan x$,

$$
I=\arctan1-\arctan0=\frac\pi4.
$$

Thus

$$
\boxed{\lim_{N\to\infty}S_N=\frac\pi4.}
$$

## ↑ Ancestors (13)

1. [Ii](../ii.md)
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
