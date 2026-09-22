<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $A=\max_{0\leq t\leq1}B_t$, a random level. The [Brownian reflection principle](../../../../../../reflection-principle-wiener-process.md) gives $A\overset d=|B_1|$, so $A>0$ [almost surely](../../../../../../almost-sure-convergence.md). Also $A-B_1\overset d=|B_1|$: this follows by applying reflection to the reversed increment process $(B_1-B_{1-s})_{0\leq s\leq1}$, which has the law of a standard [Brownian motion](../../../../../../brownian-motion-split.md). Thus $B_1<A$ [almost surely](../../../../../../almost-sure-convergence.md) as well.

By continuity and [compactness](../../../../../../compact-space.md), $A$ is attained at some time strictly between zero and one, so $H_A<1$. It is not exceeded anywhere on $[0,1]$; since $B_1<A$, continuity even excludes an exceedance in a positive interval just after time one. Consequently $T_A>1$. Both conclusions hold on a single probability-one [event](../../../../../../event.md), giving the [fixed-level versus simultaneous Brownian passage-time equality](../../../../../../fixed-level-versus-simultaneous-brownian-passage-time-equality.md) distinction:

$$
\boxed{\mathbb P\bigl(T_a=H_a\text{ for every }a\geq0\bigr)=0.}
$$

Thus **the simultaneous assertion is false**. Equality for each deterministic level, and even simultaneously for all rational levels, cannot be extended to all real levels by an uncountable intersection.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [6](../../6.md)
3. [Paper 201](../../../paper-201-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
