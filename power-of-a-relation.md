# Power of a relation

↑ **Parent:** [Binary relation](binary-relation.md)

For a [binary relation](binary-relation.md) $R$ on a [set](set-split.md) $A$, define $R^0=\{(a,a):a\in A\}$ and $R^{n+1}=R\circ R^n$ for nonnegative [integers](integer-split.md) $n$, using [composition of relations](composition-of-relations.md). A pair $(a,b)$ belongs to $R^n$ precisely when a sequence $a=x_0,x_1,\ldots,x_n=b$ has $x_{i-1}Rx_i$ for every $i$. This follows by [mathematical induction](mathematical-induction.md), splitting off one step in the recurrence. Thus $R^n$ records paths with exactly $n$ steps, rather than at most $n$ steps. The [union](set-union.md) $\bigcup_{n\geq1}R^n$ is the [transitive closure of a relation](transitive-closure-relation.md); including $R^0$ gives its [reflexive transitive closure](reflexive-transitive-closure.md). The powers of a single relation agree under the two common composition-order conventions.

## ↑ Ancestors (7)

1. [Binary relation](binary-relation.md)
2. [Finitary relation](finitary-relation.md)
3. [Set theory](set-theory-split.md)
4. [Foundations of mathematics](foundations-of-mathematics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)
