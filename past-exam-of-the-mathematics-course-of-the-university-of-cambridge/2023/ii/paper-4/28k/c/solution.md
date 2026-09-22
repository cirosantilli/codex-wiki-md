<h1 id="28k/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Apply part (b) simultaneously at every rational $t$; the intersection of these probability-one events still has probability one. On that event, monotonicity and continuity extend the convergence from the rationals to every real $t$.

More directly, fix $\varepsilon>0$. Since $F$ is a continuous [cumulative distribution function](../../../../../../cumulative-distribution-function.md), choose rational points

$$
t_0<t_1<\cdots<t_k
$$

so that the two tails have $F(t_0)<\varepsilon$ and $1-F(t_k)<\varepsilon$, while every increment $F(t_i)-F(t_{i-1})<\varepsilon$. Part (b) makes $|F_m^*(t_i)-F(t_i)|<\varepsilon$ at all these finitely many points for all sufficiently large $m$. If $t_{i-1}\leq t\leq t_i$, monotonicity gives

$$
F_m^*(t_{i-1})\leq F_m^*(t)\leq F_m^*(t_i),
$$

so $|F_m^*(t)-F(t)|<2\varepsilon$; the same estimate follows in the tails. This proves the [uniform convergence of distribution functions to a continuous limit](../../../../../../uniform-convergence-of-distribution-functions-to-a-continuous-limit.md):

$$
\sup_{t\in\mathbb R}|F_m^*(t)-F(t)|\longrightarrow0
$$

almost surely.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [28K](../../28k.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
