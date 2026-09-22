<h1 id="3/3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Continuity ensures that the maximum on $[0,1]$ is attained, so its first attainment time $\tau$ lies in $[0,1]$. To exclude the endpoint, use [Brownian time reversal on a finite interval](../../../../../../../brownian-time-reversal-on-a-finite-interval.md):

$$
R_s=B_1-B_{1-s},\qquad0\leq s\leq1.
$$

This is a standard [Brownian motion](../../../../../../../brownian-motion-split.md) on this interval. Indeed, its increments are increments of $B$ on disjoint intervals taken in reverse order, hence are independent centered normal variables with the required variances, and its paths are continuous.

If $B_1$ is the maximum, then $R_s\geq0$ for every $s$. But by the [Brownian reflection principle](../../../../../../../reflection-principle-wiener-process.md) and symmetry,

$$
\mathbb P\left(\min_{0\leq s\leq1}R_s\geq0\right)=0:
$$

the running maximum of $-R$ has the distribution of $|R_1|$, whose probability of being zero is zero. In particular the event $\tau=1$ has probability zero. **Thus $\tau<1$ with probability one.** Uniqueness of the maximizing time is not needed for this proof.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [3](../../3.md)
3. [3](../../../3.md)
4. [Paper 26](../../../../paper-26-split.md)
5. [Iii](../../../../split.md)
6. [2014](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
