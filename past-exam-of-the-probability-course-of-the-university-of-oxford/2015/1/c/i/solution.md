<h1 id="1/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [Poisson process](../../../../../poisson-process-split.md) gives $N_k\sim\operatorname{Pois}(k)$, with [expected value](../../../../../expected-value-split.md) and [variance](../../../../../variance-split.md) both equal to $k$. Consequently $Y_k=(N_k-k)/\sqrt{k}$. Scaling and translating the argument in the [moment-generating function of a Poisson distribution](../../../../../moment-generating-function-of-a-poisson-distribution.md) gives, for every real $t$,

$$
\begin{aligned}
M_{Y_k}(t)
&=e^{-t\sqrt{k}}M_{N_k}(t/\sqrt{k})\\
&=\boxed{\exp\!\left\{k\left(e^{t/\sqrt{k}}-1-\frac{t}{\sqrt{k}}\right)\right\}.}
\end{aligned}
$$

The centering term must remain inside the exponent: omitting it would leave a divergent first-order contribution.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [C](../../c.md)
3. [1](../../../1.md)
4. [2015](../../../../2015-split.md)
5. [Past exam of the probability course of the University of Oxford](../../../../split.md)
6. [Probability course of the University of Oxford](../../../../../probability-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
