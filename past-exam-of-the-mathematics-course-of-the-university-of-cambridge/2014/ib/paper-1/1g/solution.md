<h1 id="1g/solution">Solution</h1>

↑ **Parent:** [1G](../1g.md)

The [Steinitz exchange lemma](../../../../../steinitz-exchange-lemma.md) says that if $u_1,\ldots,u_r$ are [linearly independent](../../../../../linear-independence.md) and $v_1,\ldots,v_s$ [span](../../../../../linear-span.md) the same [vector space](../../../../../vector-space-split.md), then $r\leq s$ and, after reordering the $v_j$, the list $u_1,\ldots,u_r,v_{r+1},\ldots,v_s$ still spans it.

To prove this, suppose $u_1,\ldots,u_k$ have already replaced $k$ of the spanning vectors. Express $u_{k+1}$ in that spanning list. At least one coefficient of an unreplaced $v_j$ is nonzero: otherwise $u_{k+1}$ lies in the [span](../../../../../linear-span.md) of $u_1,\ldots,u_k$, contradicting [linear independence](../../../../../linear-independence.md). Solve this expression for that $v_j$ and replace it by $u_{k+1}$. The new list still spans. If all $s$ vectors were replaced before the $u_i$ were exhausted, the next $u_i$ would be dependent on its predecessors. Hence $r\leq s$, and the replacement can continue through $u_r$.

For two [bases](../../../../../basis.md) of sizes $r,s$, apply the [Steinitz exchange lemma](../../../../../steinitz-exchange-lemma.md) in both directions to get $r\leq s\leq r$. Thus **every basis has the same size**. Given a [linearly independent](../../../../../linear-independence.md) set and any finite [basis](../../../../../basis.md), the replacement procedure produces a finite spanning list containing that set. Successively delete any remaining vector dependent on the others; none of the prescribed independent vectors need be deleted, since one can instead delete a dependent supplementary vector. Equivalently, greedily retain only supplementary vectors outside the [span](../../../../../linear-span.md) already built. The resulting list is a [basis](../../../../../basis.md) containing the prescribed set.

For the three-dimensional example, the columns have matrix

$$
A_3=\begin{pmatrix}1&0&1\\1&1&0\\0&1&1\end{pmatrix},\qquad \det A_3=2.
$$

Therefore **the three vectors are a basis**. For the four-dimensional example,

$$
(e_1+e_2)-(e_2+e_3)+(e_3+e_4)-(e_4+e_1)=0.
$$

This is a nontrivial [linear dependence](../../../../../linear-dependence.md), so **the four vectors are not a basis**. The distinction is an instance of the [adjacent sums of a cyclic basis](../../../../../adjacent-sums-of-a-cyclic-basis.md) criterion: alternating coefficients close consistently around an even cycle, but not an odd one.

## ↑ Ancestors (10)

1. [1G](../1g.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
