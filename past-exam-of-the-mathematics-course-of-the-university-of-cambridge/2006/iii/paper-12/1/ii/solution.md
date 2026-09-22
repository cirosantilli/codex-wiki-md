<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Proceed by induction on the ground-set size, starting with the one-element chain $\{\varnothing\}$ in the [Boolean lattice](../../../../../../boolean-lattice.md) on no coordinates. Suppose a [symmetric chain decomposition of a Boolean lattice](../../../../../../symmetric-chain-decomposition-of-a-boolean-lattice.md) on $[n]$ has been constructed. Write one of its chains as

$$
S_r\subset S_{r+1}\subset\cdots\subset S_{n-r},\qquad |S_j|=j.
$$

On adjoining the new coordinate $v=n+1$, replace its two copies by

$$
S_r\subset\cdots\subset S_{n-r}\subset S_{n-r}\cup\{v\}
$$

and, when nonempty,

$$
S_r\cup\{v\}\subset S_{r+1}\cup\{v\}\subset\cdots\subset S_{n-r-1}\cup\{v\}.
$$

The first chain has endpoint ranks $r,n-r+1$, summing to $n+1$. The second has endpoint ranks $r+1,n-r$, also summing to $n+1$. Both are saturated chains, increasing rank by one at every step. If the original chain was a singleton, the second chain is omitted.

These new chains are disjoint: the first contains every old set without $v$ and just the last old set with $v$; the second contains precisely the remaining old sets with $v$. Thus together they cover both lifted copies of the old chain. Different old chains have disjoint copies, so performing this construction for each yields a partition of all subsets of $[n+1]$ into [symmetric chains](../../../../../../symmetric-chain-in-a-boolean-lattice.md). This completes the induction and proves **a [symmetric chain](../../../../../../symmetric-chain-in-a-boolean-lattice.md) partition exists for every $n$**.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
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
