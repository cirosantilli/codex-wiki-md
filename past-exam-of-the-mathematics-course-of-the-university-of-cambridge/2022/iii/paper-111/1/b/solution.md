<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Assume deletion. If $w=s_1\cdots s_m$ is reduced and $\ell(sw)<m$, then the word $s,s_1,\ldots,s_m$ is not reduced. Deletion removes two letters. It must remove the initial $s$: otherwise left cancellation by $s$ would give a word for $w$ shorter than $m$. Deleting $s$ and one $s_i$ gives the exchange condition.

Assume exchange, and suppose $sw$ and $wt$ are both ascents of $w$. Write $w=s_1\cdots s_m$ reduced. Then $s_1\cdots s_mt$ is reduced. If $swt$ is not a two-step ascent, left exchange deletes one letter from this expression. Deleting one of the $s_i$ would, after right cancellation by $t$, express $sw$ with at most $m-1$ letters, contradicting $\ell(sw)=m+1$. Thus exchange deletes the final $t$, and $swt=w$. This is the [folding condition](../../../../../../folding-condition.md).

Finally assume folding. Consider a shortest counterexample to deletion and draw the array of lengths of all consecutive subwords $s_i\cdots s_j$. Adjacent entries differ by at most one because each generator is an involution. Starting at the first place where the full word fails to be geodesic and following the boundary between ascents and descents produces a square in which left and right multiplication are both ascents but the diagonal is not a two-step ascent. Folding identifies the opposite vertices of this square. Cancelling the common prefix and suffix says that two letters of the original word may be deleted. This contradicts the choice of a counterexample and proves deletion. This standard argument is the [folding-grid proof of the deletion condition](../../../../../../folding-grid-proof-of-the-deletion-condition.md).

Hence

$$
\boxed{(D)\Longleftrightarrow(E)\Longleftrightarrow(F).}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 111](../../../paper-111-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
