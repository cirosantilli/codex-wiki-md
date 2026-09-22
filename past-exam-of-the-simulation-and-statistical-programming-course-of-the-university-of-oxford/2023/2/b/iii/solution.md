<h1 id="2/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For a [measurable set](../../../../../measurable-set.md) $C$, (i) gives the joint acceptance [probability](../../../../../probability.md)

$$
\mathbb P(Y\in C,\mathrm{accept})
=\int_C\frac{\widetilde q(y)}{Z_q}
\frac{\widetilde p(y)}{M\widetilde q(y)}\,dy
=\frac1{MZ_q}\int_C\widetilde p(y)\,dy.
$$

Divide by $Z_p/(MZ_q)$ from (ii). The resulting [conditional probability](../../../../../conditional-probability.md) is

$$
\boxed{\mathbb P(Y\in C\mid\mathrm{accept})
=\frac1{Z_p}\int_C\widetilde p(y)\,dy
=\int_Cp(y)\,dy.}
$$

Thus every accepted value has target [probability density function](../../../../../probability-density-function.md) $p$. Repeating rejected trials with fresh [independent random variables](../../../../../independent-random-variables.md) does not change this law: the contribution from acceptance on trial $j$ is multiplied by $(1-Z_p/(MZ_q))^{j-1}$, and summing that [geometric series](../../../../../geometric-series.md) gives the same conditional law. Independent repetitions produce [independent](../../../../../independent-random-variables.md) target draws.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
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
