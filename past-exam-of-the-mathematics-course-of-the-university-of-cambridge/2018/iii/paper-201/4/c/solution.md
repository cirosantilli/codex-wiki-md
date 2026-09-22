<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Put $D_t=B_t-B'_t$. By [independence](../../../../../../independent-random-variables.md) of the two [Brownian motions](../../../../../../brownian-motion-split.md), $D_t/\sqrt2$ is a standard [Brownian motion](../../../../../../brownian-motion-split.md): its [independent increments](../../../../../../independent-increments.md) have the [normal distribution](../../../../../../normal-distribution.md) with [variance](../../../../../../variance-split.md) equal to elapsed time. The [stopping time](../../../../../../stopping-time.md) $\tau$ is the first time $D$ hits $-1$ or $3$.

To justify finiteness without presupposing the desired [hitting probability](../../../../../../hitting-probability.md), each unit-time increment of $D$ has the [normal distribution](../../../../../../normal-distribution.md) $N(0,2)$. An increment of absolute value greater than $4$ forces exit from $[-1,3]$ if the path was inside at its start. These [independent increments](../../../../../../independent-increments.md) give $\mathbb P(\tau>n)\leq(1-p)^n$, where $p=\mathbb P(|N(0,2)|>4)>0$. Hence $\tau<\infty$ [almost surely](../../../../../../almost-sure-convergence.md).

The [stopped martingale](../../../../../../stopped-martingale.md) $D_{t\wedge\tau}$ lies in $[-1,3]$. The [optional stopping theorem](../../../../../../optional-sampling-theorem-for-a-supermartingale.md) at $t\wedge\tau$ gives $\mathbb ED_{t\wedge\tau}=0$, and the [bounded convergence theorem](../../../../../../bounded-convergence-theorem.md) gives $\mathbb ED_\tau=0$. Writing $q=\mathbb P(D_\tau=-1)$, path [continuity](../../../../../../continuous-function.md) gives $0=-q+3(1-q)$. Therefore, as in [Brownian exit from an interval](../../../../../../brownian-exit-from-an-interval.md),

$$
\boxed{\mathbb P(B_\tau=B'_\tau-1)=\frac34.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 201](../../../paper-201-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
