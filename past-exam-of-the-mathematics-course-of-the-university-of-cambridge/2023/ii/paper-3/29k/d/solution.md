<h1 id="29k/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

By continuity of [Brownian motion](../../../../../../brownian-motion-split.md), the event that the last strict crossing of $b$ occurs by time $t$ is

$$
\{T\leq t\}
=\left\{\sup_{u\geq t}(W_u-au)\leq b\right\}.
$$

Apply part (b) with $a$ and $b$ interchanged and its time parameter replaced by $1/t$. This turns the right-hand side into

$$
\mathbb P\!\left(
\sup_{0\leq s\leq1/t}(W_s-bs)\leq a
\right).
$$

Part (c), now with drift $b$, barrier $a$, and horizon $1/t$, gives

$$
\boxed{
\mathbb P(T\leq t)
=\Phi\!\left(a\sqrt t+\frac b{\sqrt t}\right)
-e^{-2ab}\Phi\!\left(\frac b{\sqrt t}-a\sqrt t\right),
\qquad t>0.}
$$

This is the distribution function of the [last passage time above a level for Brownian motion with negative drift](../../../../../../last-passage-time-above-a-level-for-brownian-motion-with-negative-drift.md). Taking $t\downarrow0$ gives

$$
\mathbb P(T=0)=1-e^{-2ab},
$$

the probability that the negatively drifted Brownian path never exceeds $b$, consistent with the [infinite-horizon crossing probability for Brownian motion with negative drift](../../../../../../infinite-horizon-crossing-probability-for-brownian-motion-with-negative-drift.md).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [29K](../../29k.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
