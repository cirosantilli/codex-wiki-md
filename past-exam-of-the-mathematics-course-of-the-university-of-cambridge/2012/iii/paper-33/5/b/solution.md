<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

First fix a deterministic point $y$ different from the initial point. By translation, work with $y=0$ and $B_0=x\ne0$. For $R>|x|$, hitting $0$ before $T_R$ requires hitting every circle of radius $r\in(0,|x|)$ before $T_R$. Part (a) gives

$$
\mathbb P_x(T_0<T_R)\leq\frac{\log R-\log|x|}{\log R-\log r}\longrightarrow0\qquad(r\downarrow0).
$$

Any finite-time hit of $0$ lies before exit from some sufficiently large integer-radius circle, since a continuous path on a finite interval is bounded. A countable union over such radii therefore shows that this fixed point is never hit. This is the [polar point for planar Brownian motion](../../../../../../polar-point-for-planar-brownian-motion.md) property; it is a statement about each fixed point, not about avoiding all points simultaneously.

For the initial point $x$, fix a deterministic $\varepsilon>0$. The [Gaussian distribution](../../../../../../normal-distribution.md) of $B_\varepsilon$ has a density, so $B_\varepsilon\ne x$ almost surely. Conditional on $\mathcal F_\varepsilon$, the future is [Brownian motion](../../../../../../brownian-motion-split.md) starting from $B_\varepsilon$, and the preceding fixed-point result shows that it never hits $x$. Taking $\varepsilon=1/m$ and a countable union proves **there is no return to the starting point at any positive time**.

In contrast, neighborhoods are revisited arbitrarily late. Choose $r>0$ so that the closed disk centered at $x$ of radius $r$ lies in the given open set $U$. From any point $z$ outside this disk, let $R\to\infty$ in part (a), centered at $x$. It gives

$$
\mathbb P_z(T_r<\infty)\geq\lim_{R\to\infty}\frac{\log R-\log|z-x|}{\log R-\log r}=1.
$$

At each deterministic integer time $n$, condition on $B_n$. If it is in the disk there is already a visit to $U$ at time $n$; if it is outside, the [Markov property](../../../../../../markov-property.md) and the last calculation ensure a later visit to that disk, hence to $U$. With [probability](../../../../../../probability.md) one this holds for all $n$ simultaneously. Thus **the set of visits to $U$ is unbounded**. The [recurrence of planar Brownian motion](../../../../../../recurrence-of-planar-brownian-motion.md) concerns neighborhoods even though every fixed point is polar.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 33](../../../paper-33-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
