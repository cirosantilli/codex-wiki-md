<h1 id="2e/solution">Solution</h1>

↑ **Parent:** [2E](../2e.md)

For nonnegative [integers](../../../../../integer.md) $n,m$, prove the [hockey-stick identity](../../../../../hockey-stick-identity.md) by [mathematical induction](../../../../../mathematical-induction.md) on $m$. The [induction base case](../../../../../induction-base-case.md) $m=0$ is $\binom n0=\binom{n+1}0=1$. If the formula holds through $m-1$, [Pascal's identity](../../../../../pascal-s-rule.md) gives

$$
\sum_{j=0}^m\binom{n+j}j
=\binom{n+m}{m-1}+\binom{n+m}m
=\binom{n+m+1}m.
$$

This supplies the [inductive step](../../../../../inductive-step.md).

A [binary string](../../../../../binary-string.md) containing exactly $n$ zeroes and $j$ ones has length $n+j$. Choosing its $j$ one-positions gives $\binom{n+j}j$ possibilities. Different values of $j$ give disjoint collections, so [counting binary strings with bounded ones](../../../../../counting-binary-strings-with-bounded-ones.md) yields

$$
\boxed{\sum_{j=0}^m\binom{n+j}j=\binom{n+m+1}m.}
$$

This includes $n=0$: the $m+1$ strings are the empty string and the all-one strings of lengths one through $m$.

## ↑ Ancestors (10)

1. [2E](../2e.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ia](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
