<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The span of the $n$ asset payoff functions has [dimension](../../../../../../dimension-vector-space.md) at most $n$. If there were $n+1$ disjoint measurable events $A_1,\ldots,A_{n+1}$ of positive probability, their [indicator functions](../../../../../../indicator-function.md) would be linearly independent as random variables modulo almost-sure equality. Indeed, restricting a zero linear combination to $A_j$ forces its $j$th coefficient to vanish. [Market completeness](../../../../../../complete-market.md) would put all these independent functions inside a span of dimension at most $n$, a contradiction.

This implies the stronger meaningful partition conclusion: **terminal information has at most (n) positive-probability atoms**. Start with the whole sample space and split any event which is not a probability [atom of a measure](../../../../../../atom-measure-theory.md) into two positive-probability measurable subsets. Each split increases the number of disjoint positive events, so no more than $n-1$ splits are possible. The resulting partition has $m\le n$ components, and each is a probability [atom of a measure](../../../../../../atom-measure-theory.md), since otherwise another split would be possible. Null sets can be included in a component without altering any random variable modulo null sets.

On such an atom every measurable real-valued random variable is constant almost surely: if its distribution on that atom were not concentrated at one value, an appropriate level set would split the atom. Hence every terminal claim is described by its $m$ values. This proves the [finite branching bound in a complete market](../../../../../../finite-branching-bound-in-a-complete-market.md) for one period, rather than the vacuous weaker observation that the whole space itself is one event.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 39](../../../paper-39-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
