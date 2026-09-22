<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The supplied hint interchanges its item and bidder indices in the first-value identity. If the first greedy choice assigns item $n$ to bidder $m$, the correct quantity is $w=v_m(\{n\})$, and the identity is

$$
\boxed{A(v)=w+A(v').}
$$

Indeed, the eventual bundle of bidder $m$ has the form $S'_m\cup\{n\}$, whose value is $w+v'_m(S'_m)$; the other bidders' values are unchanged. Every later [marginal contribution](../../../../../../marginal-contribution.md) for bidder $m$ is exactly its marginal in the residual problem, and this is also true for every other bidder. Thus the remainder of the greedy run is the greedy run on $v'$, with the same tie choices. The residual values are nonnegative and increasing; they remain [submodular set functions](../../../../../../submodular-set-function.md) as allowed in the question.

We prove the [greedy half-approximation for submodular welfare](../../../../../../greedy-half-approximation-for-submodular-welfare.md) by induction on the number of items. The zero-item case has $A(v)=\operatorname{Opt}(v)=\sum_i v_i(\varnothing)\geq0$, so the claimed inequality holds. This base case also handles the fact that the question does not explicitly normalize empty-bundle values to zero.

For the induction step, let

$$
\delta=v_m(\{n\})-v_m(\varnothing)\geq0
$$

be the first greedy marginal. Since the choice maximizes all available marginals,

$$
v_i(\{n\})-v_i(\varnothing)\leq\delta\leq w\qquad\text{for every bidder }i.
$$

Take an optimal allocation and let $i$ be the owner of item $n$. If $i\ne m$, remove that item from $i$'s bundle and give it to $m$. By [submodularity](../../../../../../submodular-set-function.md), the loss to its old owner is

$$
v_i(S_i)-v_i(S_i\setminus\{n\})
\leq v_i(\{n\})-v_i(\varnothing)\leq\delta.
$$

Monotonicity makes the recipient's gain nonnegative. The modified allocation, now with $n$ assigned to $m$, therefore has value at least $\operatorname{Opt}(v)-\delta$. If $i=m$, no modification is necessary and this bound still holds. Removing $n$ and translating bidder $m$'s value by $w$ produces a feasible residual allocation, so

$$
\operatorname{Opt}(v')\geq\operatorname{Opt}(v)-\delta-w
\geq\operatorname{Opt}(v)-2w.
$$

Induction applied to that residual problem now gives

$$
A(v)=w+A(v')\geq w+\tfrac12\operatorname{Opt}(v')
\geq\tfrac12\operatorname{Opt}(v).
$$

Thus **the greedy algorithm is a one-half approximation**. Empty-bundle constants cause no difficulty because all are nonnegative and $\delta\leq w$.

At each of $n$ stages evaluate the marginal for at most $m$ bidders and $n$ remaining items. This requires $O(mn^2)$ value queries, and polynomial additional work with bundle bit-vectors and cached current values. Hence it is a [polynomial time](../../../../../../polynomial-time.md) [approximation algorithm](../../../../../../approximation-algorithm.md) in the value-oracle model, assuming [polynomial time](../../../../../../polynomial-time.md) bid evaluations. If every bundle bid is explicitly listed, this query bound is polynomial in that larger explicit input as well. The exponentially many possible bundles do not require enumerating allocations.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 35](../../../paper-35-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
