<h1 id="6f/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

First, [finite additivity of a set function](../../../../../../finite-additivity-of-a-set-function.md) gives $f(\varnothing)=0$, since $f(\varnothing)=2f(\varnothing)$. Put $w_s=f(\{s\})$. Decomposing any subset into its singleton elements and using [induction](../../../../../../mathematical-induction.md) gives $f(A)=\sum_{s\in A}w_s$. Fix $s\in S$ and let $r$ be the number of sets $A_i$ containing it. Its total coefficient in the alternating intersection sum is zero if $r=0$, and otherwise is

$$
\sum_{k=1}^r(-1)^{k+1}\binom rk=1-(1-1)^r=1
$$

by the [binomial theorem](../../../../../../binomial-theorem.md). These are exactly the coefficients in $f(\bigcup_iA_i)$. Summing against $w_s$ proves the required [inclusion-exclusion principle](../../../../../../inclusion-exclusion-principle.md) for the additive [set function](../../../../../../set-function.md), including signed weights.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [6F](../../6f.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ia](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
