<h1 id="2/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Fix a proposal $y$ with $\widetilde q(y)>0$, and abbreviate $B=M\widetilde q(y)$, $H=h(y)$ and $P=\widetilde p(y)$. The envelope says $0\leq H\leq P\leq B$. Assuming fresh [independent](../../../../../independent-random-variables.md) [uniform distribution](../../../../../continuous-uniform-distribution.md) draws at both stages, the [law of total probability](../../../../../law-of-total-probability.md) gives

$$
\begin{aligned}
\mathbb P(\mathrm{accept}\mid Y=y)
&=\frac HB+\left(1-\frac HB\right)\frac{P-H}{B-H}\\
&=\frac HB+\frac{P-H}{B}
=\boxed{\frac{\widetilde p(y)}{M\widetilde q(y)}}.
\end{aligned}
$$

The second term includes both reaching the residual test and passing it. If $H=B$, the envelope forces $P=B$ and the first test accepts with [probability](../../../../../probability.md) one; the second-stage $0/0$ ratio is never evaluated. This is [squeeze rejection sampling](../../../../../squeeze-rejection-sampling.md).

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the simulation and statistical programming course of the University of Oxford](../../../../split.md)
6. [Simulation and statistical programming course of the University of Oxford](../../../../../simulation-and-statistical-programming-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
