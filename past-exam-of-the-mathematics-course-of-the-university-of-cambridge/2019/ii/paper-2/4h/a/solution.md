<h1 id="4h/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [recursive set](../../../../../../computable-set.md) $E\subseteq\mathbb N_0$ has an [indicator function](../../../../../../indicator-function.md) computed by a [register machine](../../../../../../register-machine.md) that halts on every input. A [recursively enumerable set](../../../../../../recursively-enumerable-set.md) is the exact halting set of some register machine; equivalently, it is the domain of a [partial computable function](../../../../../../computable-function.md).

If $E$ is recursive, its decider immediately gives machines that halt exactly on $E$ and on $\mathbb N_0\setminus E$, so both sets are recursively enumerable. Conversely, suppose machines $M_E$ and $M_{E^c}$ recognize the two sets. On input $x$, use [dovetailing](../../../../../../dovetailing.md) to run one step of $M_E(x)$ and one step of $M_{E^c}(x)$ alternately. Exactly one must eventually halt. Return one if $M_E$ halts first and zero if $M_{E^c}$ halts first. This is a total decider for $E$, so $E$ is recursive.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4H](../../4h.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
