<h1 id="2/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For the [exponential distribution](../../../../../exponential-distribution.md) with rate $\lambda$, the [cumulative distribution function](../../../../../cumulative-distribution-function.md) is $F(x)=1-e^{-\lambda x}$ for $x\geq0$, and zero for $x<0$. Its [quantile function](../../../../../quantile-function.md) is

$$
\boxed{F^{-1}(u)=-\frac{\log(1-u)}{\lambda},\qquad0<u<1.}
$$

For [inverse transform sampling](../../../../../inverse-transform-sampling.md), draw $U$ from the [uniform distribution](../../../../../continuous-uniform-distribution.md) on $(0,1)$ and return $-\log(1-U)/\lambda$. Equivalently return $-\log U/\lambda$, since $1-U$ has the same [uniform distribution](../../../../../continuous-uniform-distribution.md). Indeed, for $x\geq0$, $\mathbb P(-\log U/\lambda>x)=\mathbb P(U<e^{-\lambda x})=e^{-\lambda x}$.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [A](../../a.md)
3. [2](../../../2.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the simulation and statistical programming course of the University of Oxford](../../../../split.md)
6. [Simulation and statistical programming course of the University of Oxford](../../../../../simulation-and-statistical-programming-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
