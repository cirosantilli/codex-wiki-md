<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write the [molecular copy numbers](../../../../../../molecular-copy-number.md) as $\mathbf x=(x_1,x_2,x_3,x_4)$ and use the [power-law reaction propensity](../../../../../../power-law-reaction-propensity.md) convention of the paper. The seven propensities and [stoichiometric vectors](../../../../../../stoichiometric-vector.md) are

$$
\begin{array}{c|c|c}
r&a_r(\mathbf x)&\nu_r\\ \hline
1&\alpha_1x_1^2/V&(-2,0,0,0)\\
2&\alpha_2x_1&(0,1,0,0)\\
3&\alpha_3x_2^2/V&(0,-1,0,0)\\
4&\alpha_4V&(0,0,1,0)\\
5&\alpha_5x_3x_4/V&(0,0,-1,-1)\\
6&\alpha_6x_2&(0,0,0,1)\\
7&\alpha_7x_2x_4/V&(0,-1,0,0).
\end{array}
$$

A channel is assigned zero propensity whenever its update would leave the [nonnegative integer](../../../../../../natural-number.md) lattice.

The [Gillespie algorithm](../../../../../../gillespie-algorithm.md) starts from $\mathbf x=(5,0,0,0)$ and $t=0$. At the current state compute $a_0=\sum_{r=1}^7a_r$. If $a_0=0$, terminate the path. Otherwise draw [independent random variables](../../../../../../independent-random-variables.md) $U_1,U_2$ from the [uniform distribution](../../../../../../continuous-uniform-distribution.md) on $(0,1)$, set the next waiting time to

$$
\tau=-\frac{\log U_1}{a_0},
$$

and choose the least index $r$ satisfying

$$
\sum_{j=1}^ra_j\geq U_2a_0.
$$

Then update $t\leftarrow t+\tau$ and $\mathbf x\leftarrow\mathbf x+\nu_r$, and repeat. The minimum of the seven competing reaction clocks has an [exponential distribution](../../../../../../exponential-distribution.md) of rate $a_0$, while reaction $r$ wins with probability $a_r/a_0$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 356](../../../paper-356-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
