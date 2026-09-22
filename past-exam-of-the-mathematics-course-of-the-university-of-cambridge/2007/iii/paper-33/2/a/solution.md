<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write the residual process as

$$
M_t=\sum_{i=1}^n\theta_i\frac{\mathbf1_{\{U_i>t\}}}{1-t}.
$$

For $s<t<1$, the filtration tells us whether each $U_i$ has arrived by time $s$, and its exact arrival time if it has. On $\{U_i>s\}$, its conditional law is uniform on $(s,1)$. [Independence](../../../../../../independent-random-variables.md) of the original $U_i$ means that the histories of the other arrivals do not alter this law. Hence

$$
\mathbb E[\mathbf1_{\{U_i>t\}}\mid\mathcal F_s]
=\mathbf1_{\{U_i>s\}}\frac{1-t}{1-s}.
$$

This conditional identity can also be checked against products of bounded functions of the censored arrival times and extended to $\mathcal F_s$ by the [Monotone class theorem](../../../../../../monotone-class-theorem.md). Summing the identity gives **$\mathbb E[M_t\mid\mathcal F_s]=M_s$**.

Each $M_t$ is adapted and integrable, with

$$
\mathbb E M_t=\sum_i\theta_i=S.
$$

Its paths are smooth between the finitely many arrival times and have downward jumps of size $\theta_i/(1-U_i)$ at arrivals before time one. The indicators use $U_i>t$, so the value at a jump is the post-jump value: paths are right continuous with finite left limits on $[0,1)$. Thus $M$ is a [càdlàg martingale](../../../../../../cadlag-martingale.md), specifically the [uniform-arrival residual mass martingale](../../../../../../uniform-arrival-residual-mass-martingale.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 33](../../../paper-33-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
