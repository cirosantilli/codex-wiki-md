<h1 id="9/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Since $X$ is nonnegative, $F_X(x)=0$ for $x<0$. For $x\geq0$, use $\frac{d}{dt}e^{-t^2/2}=-te^{-t^2/2}$ to obtain

$$
F_X(x)=\int_0^xte^{-t^2/2}\,dt=1-e^{-x^2/2}.
$$

Thus the [cumulative distribution function](../../../../../../cumulative-distribution-function.md) is

$$
\boxed{F_X(x)=\begin{cases}0,&x<0,\\1-e^{-x^2/2},&x\geq0.\end{cases}}
$$

In particular it tends to one as $x\to\infty$, confirming normalization of this unit-scale [Rayleigh distribution](../../../../../../rayleigh-distribution.md).

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [9](../../../9.md)
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
