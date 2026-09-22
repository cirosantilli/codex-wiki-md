<h1 id="b/6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Suppose first that $d=|z_0|>\epsilon$. Apply part (a) with inner radius $\epsilon$ and outer radius $R>d$:

$$
\mathbb P(\text{hit radius }\epsilon\text{ before radius }R)
=\frac{\log(R/d)}{\log(R/\epsilon)}\longrightarrow1
\quad(R\to\infty).
$$

Each event implies finite hitting time of the $\epsilon$ circle, so that hitting probability is one. If $d=\epsilon$, the hitting time is zero. If $d<\epsilon$, it is the exit time from a bounded disk. The martingale $|Z_t-z_0|^2-2t$, stopped before that exit, gives a finite mean exit-time bound $(\epsilon^2-d^2)/2$. Thus the asserted hitting time is almost surely finite in this case too.

For alternating visits, choose two closed smaller disks $K_i$ strictly inside the given open disks $D_i$, so their distance is positive. Define successive first hitting times of $K_1,K_2,K_1,K_2,\ldots$. Translation invariance and the [Strong Markov property](../../../../../strong-markov-property.md) apply the just-proved hitting result from every successive starting point. A countable intersection makes all these times finite almost surely, with the required disk memberships.

These increasing times cannot accumulate at a finite time. On a compact time interval a continuous Brownian path is uniformly continuous, whereas every consecutive visit must cross the fixed positive distance between $K_1$ and $K_2$. Therefore

$$
\boxed{T_n\uparrow\infty\quad\text{almost surely}.}
$$

This is the [recurrence of planar Brownian motion](../../../../../recurrence-of-planar-brownian-motion.md) in neighborhoods; it does not assert that every individual point is hit.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [6](../../6.md)
3. [B](../../../b.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the stochastic differential equations and Brownian motion in complex analysis course of the University of Oxford](../../../../split.md)
6. [Stochastic differential equations and Brownian motion in complex analysis course of the University of Oxford](../../../../../stochastic-differential-equations-and-brownian-motion-in-complex-analysis-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
