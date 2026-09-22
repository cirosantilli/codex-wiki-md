<h1 id="1h/solution">Solution</h1>

↑ **Parent:** [1H](../1h.md)

Let $u_1,\ldots,u_m$ and $v_1,\ldots,v_n$ be two finite [bases](../../../../../basis.md) of the [vector space](../../../../../vector-space-split.md) $V$. We prove the underlying exchange argument rather than assuming that [dimension](../../../../../dimension-vector-space.md) is already well-defined.

More generally, suppose $u_1,\ldots,u_m$ are [linearly independent](../../../../../linear-independence.md) and $v_1,\ldots,v_n$ form a [spanning set](../../../../../spanning-set.md). Starting with the spanning list of $v$'s, replace one of its members by $u_1$. Indeed, express $u_1$ as a linear combination of that list; at least one coefficient is nonzero, so we can solve for its corresponding $v_j$ and retain a spanning list. Inductively, suppose the spanning list now consists of $u_1,\ldots,u_r$ and $n-r$ of the original $v$'s. Express $u_{r+1}$ in that list. Some coefficient of a remaining $v$ must be nonzero, since otherwise $u_{r+1}$ would lie in the span of the preceding $u$'s, contradicting [linear independence](../../../../../linear-independence.md). Solve for that $v$ and replace it by $u_{r+1}$.

If $m>n$, after $n$ replacements the spanning list consists of $u_1,\ldots,u_n$, forcing $u_{n+1}$ to lie in their span, again a contradiction. Thus every finite [linearly independent](../../../../../linear-independence.md) list has at most as many members as every finite [spanning set](../../../../../spanning-set.md). This proves the [Steinitz exchange lemma](../../../../../steinitz-exchange-lemma.md) in the form required here. Applying it to the two [bases](../../../../../basis.md) in both orders gives $m\leq n$ and $n\leq m$, hence **$m=n$**. The zero [vector space](../../../../../vector-space-split.md) has only the empty [basis](../../../../../basis.md), which also fits the argument.

## ↑ Ancestors (10)

1. [1H](../1h.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
