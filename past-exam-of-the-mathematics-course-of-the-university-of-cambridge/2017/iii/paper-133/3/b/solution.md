<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The two commutation relations make $c$ central, and the remaining relation is $ab=cba$. Repeatedly move $a$ past $b$, keeping the central powers in front. Induction first on $s$ and then on $r$ gives

$$
a^r b^s=c^{rs}b^s a^r\qquad(r,s\geq0).
$$

Therefore

$$
\boxed{a^k b^k a^{-k}b^{-k}=c^{k^2}\qquad(k\geq0).}
$$

This is the [commutator identity in the integer Heisenberg group](../../../../../../commutator-identity-in-the-integer-heisenberg-group.md). The order of the factors fixes the positive sign of the exponent.

To check the claimed infinite order, map the generators to matrices

$$
a\mapsto I+E_{12},\qquad b\mapsto I+E_{23},\qquad c\mapsto I+E_{13}.
$$

Their commutator is $I+E_{13}$, which commutes with both other matrices, so all defining relations hold. The image of $c^m$ is $I+mE_{13}$; hence $c$ has infinite order. This realizes the presentation in the [Integer Heisenberg group](../../../../../../integer-heisenberg-group.md) and is sufficient to certify the cyclic subgroup, without needing to prove faithfulness of the whole representation.

With the ambient [word metric](../../../../../../word-metric.md) from $\{a,b,c\}^{\pm1}$, the displayed commutator gives

$$
|c^{k^2}|_H\leq4k.
$$

For any finite generating set $T$ of $\langle c\rangle$, write its elements as powers of $c$ and set $B=\max\{|j|:c^j\in T\}$, with inverses included. Since $T$ generates an [infinite cyclic group](../../../../../../infinite-cyclic-group.md), $B\geq1$. A word of length $m$ in $T$ has exponent at most $Bm$ in absolute value, so

$$
|c^{k^2}|_T\geq\frac{k^2}{B}.
$$

A [quasi-isometric embedding](../../../../../../quasi-isometric-embedding.md) of the inclusion would require $|c^{k^2}|_H\geq\lambda^{-1}|c^{k^2}|_T-\varepsilon$. Combining these bounds would give $4k\geq k^2/(B\lambda)-\varepsilon$ for every $k$, which is impossible. Thus **the inclusion of the central infinite cyclic subgroup is not a [quasi-isometric embedding](../../../../../../quasi-isometric-embedding.md)**. Changing the ambient finite generating set only changes multiplicative constants, by [equivalence of finite word metrics](../../../../../../equivalence-of-finite-word-metrics.md). This is the [quadratic distortion of the Heisenberg center](../../../../../../quadratic-distortion-of-the-heisenberg-center.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 133](../../../paper-133-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
