<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A [subset](../../../../subset.md) $E\subseteq\mathbb R$ is a [Lebesgue measurable set](../../../../lebesgue-measurable-set.md) when it satisfies [Carathéodory's criterion](../../../../caratheodory-s-criterion.md): for every $T\subseteq\mathbb R$,

$$
m^*(T)=m^*(T\cap E)+m^*(T\setminus E).
$$

Suppose $m^*(A)=0$ and let $B\subseteq A$, allowing $B=A$. The [monotonicity of Lebesgue outer measure](../../../../monotonicity-of-lebesgue-outer-measure.md) follows directly from covers: every cover of a larger set covers a smaller set. Thus $m^*(B)=m^*(T\cap B)=0$, while $m^*(T\setminus B)\leq m^*(T)$. Consequently

$$
m^*(T\cap B)+m^*(T\setminus B)\leq m^*(T).
$$

The reverse inequality is [countable subadditivity of Lebesgue outer measure](../../../../countable-subadditivity-of-lebesgue-outer-measure.md) applied to $T=(T\cap B)\cup(T\setminus B)$. Equality follows, even if $m^*(T)=\infty$. Therefore **$A$ and every [subset](../../../../subset.md) $B\subseteq A$ are [Lebesgue measurable sets](../../../../lebesgue-measurable-set.md) of measure zero**. This is the [completeness of Lebesgue measure](../../../../completeness-of-lebesgue-measure.md), obtained without presupposing measurability of the outer-null set.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the integration course of the University of Oxford](../../../split.md)
5. [Integration course of the University of Oxford](../../../../integration-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
