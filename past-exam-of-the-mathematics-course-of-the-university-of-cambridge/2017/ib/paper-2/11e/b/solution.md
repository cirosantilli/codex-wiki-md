<h1 id="11e/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Consider all [ideals](../../../../../../ideal.md) containing $I$ and disjoint from the nonempty [multiplicative subset](../../../../../../multiplicatively-closed-set.md) $S$. This collection is nonempty because it contains $I$. The [ascending chain condition](../../../../../../ascending-chain-condition.md) for the [Noetherian ring](../../../../../../noetherian-ring.md) gives a maximal member $P$: otherwise repeatedly choosing a strictly larger member would give an infinite strictly ascending chain of ideals. Since $S$ is nonempty and $P$ misses it, $P\ne R$.

Suppose $ab\in P$ but $a,b\notin P$. Maximality implies that $P+(a)$ and $P+(b)$ both meet $S$, so write $s=p+ra\in S$ and $t=q+ub\in S$ with $p,q\in P$. Then

$$
st=pq+pub+qra+ruab\in P,
$$

while closure under products gives $st\in S$, a contradiction. Hence

$$
\boxed{P\supseteq I,\quad P\cap S=\varnothing,\quad P\text{ is prime}.}
$$

This proves the [prime ideal avoiding a multiplicative subset](../../../../../../prime-ideal-avoiding-a-multiplicative-subset.md) result without needing $1\in S$. The assumptions themselves rule out $0\in S$, since every ideal contains zero.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [11E](../../11e.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
