<h1 id="1f/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [Steinitz exchange lemma](../../../../../../steinitz-exchange-lemma.md) says that if $w_1,\ldots,w_m$ span a [vector space](../../../../../../vector-space-split.md) and $v_1,\ldots,v_r$ are [linearly independent](../../../../../../linear-independence.md), then $r\le m$, and after reordering the $w_j$, the family $v_1,\ldots,v_r,w_{r+1},\ldots,w_m$ still spans. Here is a proof. Suppose the first $k-1$ replacements have been made. Express $v_k$ in that spanning family. Some coefficient of a remaining $w_j$ must be nonzero, since otherwise $v_k$ belongs to the [span](../../../../../../linear-span.md) of $v_1,\ldots,v_{k-1}$, contrary to [linear independence](../../../../../../linear-independence.md). Solve for that $w_j$ and replace it by $v_k$; this preserves spanning. If $r>m$, the first $m$ replacements leave a spanning family $v_1,\ldots,v_m$, contradicting [linear independence](../../../../../../linear-independence.md) of the first $m+1$ vectors. This proves both assertions.

Now suppose $S$ is [linearly independent](../../../../../../linear-independence.md) and spans $\mathbb R^n$. Express each member of the [standard basis](../../../../../../standard-basis.md) using finitely many members of $S$, and let $S_0$ be the finite union of those members. Then $S_0$ spans. No element of $S\setminus S_0$ can exist, since it would be a [linear combination](../../../../../../linear-combination.md) of $S_0$ and violate [linear independence](../../../../../../linear-independence.md). Thus $S$ is finite. Applying the [Steinitz exchange lemma](../../../../../../steinitz-exchange-lemma.md) in both directions to $S$ and the [standard basis](../../../../../../standard-basis.md) gives $|S|\le n$ and $n\le |S|$. Hence $\boxed{|S|=n}$.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1F](../../1f.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
