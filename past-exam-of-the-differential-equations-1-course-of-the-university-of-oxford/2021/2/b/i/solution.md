<h1 id="2/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

With the standard constant starting [Picard iterate](../../../../../picard-iterate.md), $y_0(x)=1$, the next two [Picard iterates](../../../../../picard-iterate.md) are

$$
y_1(x)=1+\int_1^x\left(s+\frac{s}{1}\right)\,ds=x^2
$$

and, for $x>0$,

$$
\begin{aligned}
y_2(x)&=1+\int_1^x\left(s+\frac{s}{s^2}\right)\,ds\\
&=1+\frac{x^2-1}{2}+\log x.
\end{aligned}
$$

Thus

$$
\boxed{y_0(x)=1,\qquad y_1(x)=x^2,\qquad y_2(x)=\frac{x^2+1}{2}+\log x.}
$$

The restriction $x>0$ for $y_2$ is essential for the [integral](../../../../../integral-split.md) from $1$ to $x$: the preceding iterate $y_1$ vanishes at $0$, where the new integrand $s+1/s$ is undefined.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the differential equations 1 course of the University of Oxford](../../../../split.md)
6. [Differential equations 1 course of the University of Oxford](../../../../../differential-equations-1-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
