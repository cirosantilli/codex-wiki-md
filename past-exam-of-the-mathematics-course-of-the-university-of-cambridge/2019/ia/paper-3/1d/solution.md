<h1 id="1d/solution">Solution</h1>

↑ **Parent:** [1D](../1d.md)

Conjugating a [cycle](../../../../../permutation-cycle.md) merely relabels its entries:

$$
g(a_1\ a_2\ \cdots\ a_k)g^{-1}
=(g(a_1)\ g(a_2)\ \cdots\ g(a_k)).
$$

Thus conjugate [permutations](../../../../../permutation.md) have the same [cycle type](../../../../../cycle-type.md). Conversely, if $\sigma$ and $\tau$ have the same cycle type, match the entries of each cycle of $\sigma$ bijectively and in cyclic order with those of a cycle of $\tau$ of the same length. Extending these matches to a permutation $g$ gives $g\sigma g^{-1}=\tau$.

Let $C_{S_n}(\sigma)$ be the [centralizer](../../../../../centralizer.md) of $\sigma$. Its $S_n$-conjugacy class remains one $A_n$-conjugacy class exactly when $C_{S_n}(\sigma)$ contains an [odd permutation](../../../../../odd-permutation.md). Indeed, in that case $C_{A_n}(\sigma)$ has index two in $C_{S_n}(\sigma)$, so the [orbit-stabilizer theorem](../../../../../orbit-stabilizer-theorem.md) gives

$$
|\operatorname{Cl}_{A_n}(\sigma)|
=\frac{|A_n|}{|C_{A_n}(\sigma)|}
=\frac{|S_n|}{|C_{S_n}(\sigma)|}
=|\operatorname{Cl}_{S_n}(\sigma)|.
$$

If the centralizer contains only even permutations, the $A_n$ class has half the size and the $S_n$ class splits into two $A_n$ classes.

The even cycle types in $S_5$ are

$$
1^5,\qquad 3\,1^2,\qquad 2^2 1,\qquad 5.
$$

The classes of the identity, a three-cycle, and a double transposition do not split: their centralizers contain an odd permutation. The centralizer of a five-cycle is its cyclic subgroup of order five, which lies in $A_5$, so that class splits in two. Therefore

$$
\boxed{A_5\text{ has }1+1+1+2=5\text{ conjugacy classes}}.
$$

## ↑ Ancestors (10)

1. [1D](../1d.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
