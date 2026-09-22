<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The work passed downstream in slot $(t-1,t)$ is

$$
D_t=\min\{c,Q_{t-1}+a_t\}=Q_{t-1}+a_t-Q_t.
$$

Because this work is eligible for downstream service in the same slot, the downstream [Lindley recursion](../../../../../../lindley-recursion.md) is

$$
\boxed{R_t=(R_{t-1}+D_t-d)^+.}
$$

Put $T_t=Q_t+R_t$. If $R_{t-1}+D_t\geq d$, then

$$
T_t=Q_{t-1}+R_{t-1}+a_t-d\geq0.
$$

If $R_{t-1}+D_t<d$, then $D_t<d<c$, so the upstream server did not use its full capacity. Consequently $D_t=Q_{t-1}+a_t$ and $Q_t=0$. Also $R_t=0$ and $Q_{t-1}+R_{t-1}+a_t-d<0$. Both cases yield

$$
\boxed{Q_t+R_t=(Q_{t-1}+R_{t-1}+a_t-d)^+.}
$$

This [slower-server tandem workload identity](../../../../../../slower-server-tandem-workload-identity.md) uses both $d<c$ and eligibility for same-slot downstream service. It would not describe a system with an obligatory one-slot transfer delay.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 79](../../../paper-79-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
