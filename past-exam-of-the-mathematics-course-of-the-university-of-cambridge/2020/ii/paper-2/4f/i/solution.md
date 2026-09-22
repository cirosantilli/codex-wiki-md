<h1 id="4f/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

A subset $E\subseteq\mathbb N$ is [recursive](../../../../../../computable-set.md) when its [indicator function](../../../../../../indicator-function.md) is a [total computable function](../../../../../../total-computable-function.md). It is [recursively enumerable](../../../../../../recursively-enumerable-set.md) when it is the domain of a [partial computable function](../../../../../../computable-function.md), equivalently when an algorithm can enumerate its members.

If $E$ is recursive, its indicator decides both $E$ and its complement, so both sets are recursively enumerable. Conversely, suppose programs enumerate $E$ and $\mathbb N\setminus E$. On input $n$, run the two enumerations in parallel by [dovetailing](../../../../../../dovetailing.md). Exactly one must eventually print $n$; accept in the first case and reject in the second. This algorithm always halts and decides $E$. Hence

$$
\boxed{E\text{ is recursive}\iff E\text{ and }\mathbb N\setminus E\text{ are recursively enumerable}}.
$$

## ↑ Ancestors (11)

1. [I](../i.md)
2. [4F](../../4f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
