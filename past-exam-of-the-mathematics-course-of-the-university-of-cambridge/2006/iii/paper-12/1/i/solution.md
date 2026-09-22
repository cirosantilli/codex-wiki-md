<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For $1\le r\le n$ and a rank-$r$ [uniform set family](../../../../../../uniform-set-family.md) $\mathcal F$, let $\partial\mathcal F$ be its [lower shadow](../../../../../../lower-shadow.md). Count pairs $(B,A)$ with $A\in\mathcal F$, $B\subset A$ and $|B|=r-1$. Every $A$ contributes $r$ pairs, whereas each shadow member lies in at most $n-r+1$ rank-$r$ sets. Thus

$$
r|\mathcal F|\le(n-r+1)|\partial\mathcal F|,
\qquad
\boxed{\frac{|\partial\mathcal F|}{\binom n{r-1}}\ge
\frac{|\mathcal F|}{\binom nr}.}
$$

This is the [Local LYM inequality](../../../../../../local-lym-inequality.md). Complementation gives the upper-shadow form $|\nabla\mathcal F|/\binom n{r+1}\ge|\mathcal F|/\binom nr$ for $r<n$.

To deduce the [LYM inequality](../../../../../../lubell-yamamoto-meshalkin-inequality.md), let $\mathcal A$ be an [antichain](../../../../../../antichain.md), $\mathcal A_r$ its rank-$r$ part, and $U_r$ all rank-$r$ sets containing some member of $\mathcal A$. For $r\ge1$,

$$
U_r=\nabla U_{r-1}\ \dot\cup\ \mathcal A_r.
$$

The union is disjoint because an [antichain](../../../../../../antichain.md) member cannot contain a smaller member; every other set of $U_r$ contains a rank-$(r-1)$ superset of its smaller witnessing member. Apply the upper local inequality and put $u_r=|U_r|/\binom nr$:

$$
u_r\ge u_{r-1}+\frac{|\mathcal A_r|}{\binom nr}.
$$

Since $u_0=|\mathcal A_0|$ and $u_n\le1$, summing gives

$$
\boxed{\sum_{r=0}^n\frac{|\mathcal A_r|}{\binom nr}\le1.}
$$

Thus the deduction uses the local inequality explicitly, rather than quoting a separate maximal-chain argument.

Let $M=\binom n{\lfloor n/2\rfloor}$, the largest rank size. The LYM sum is at least $|\mathcal A|/M$, proving the [Sperner theorem](../../../../../../sperner-s-theorem.md) bound. If $|\mathcal A|=M$, equality forces all its members onto ranks with [binomial coefficient](../../../../../../binomial-coefficient.md) $M$. For even $n$, there is only the middle rank, so the family is that whole rank.

For $n=2m+1$, only ranks $m,m+1$ are possible, each of size $M$. Let $\mathcal B=\mathcal A_{m+1}$. Antichainness gives $\mathcal A_m\cap\partial\mathcal B=\varnothing$, and local LYM gives $|\partial\mathcal B|\ge|\mathcal B|$. Since the two [antichain](../../../../../../antichain.md) parts together have size $M$, equality must hold. The inclusion [graph](../../../../../../graph-split.md) between these ranks is $(m+1)$-regular on each side. Its [edges](../../../../../../edge-of-a-graph.md) from $\mathcal B$ already number $(m+1)|\mathcal B|$, so equality leaves no edge from $\partial\mathcal B$ to the complementary upper [vertices](../../../../../../vertex-graph-theory.md).

The [graph](../../../../../../graph-split.md) is connected: exchanging one element between two $m$-sets joins them through their $(m+1)$-element union, and successive exchanges connect all lower [vertices](../../../../../../vertex-graph-theory.md); every upper vertex has a lower neighbour. Consequently $\mathcal B$ is either empty or the entire upper rank. This [connectedness of adjacent-level incidence in a Boolean lattice](../../../../../../connectedness-of-adjacent-level-incidence-in-a-boolean-lattice.md) excludes mixed extremizers. Hence

$$
\boxed{\text{the maximum antichains are exactly the full middle levels}.}
$$

There is one choice for even $n$ and two for odd $n$. For $n=0$, the sole maximum family is $\{\varnothing\}$, agreeing with this description.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 12](../../../paper-12-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
