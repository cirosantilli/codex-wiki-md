<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

A [partition of an integer](../../../../../partition-of-an-integer.md) $n$ is a finite sequence $\lambda_1\geq\cdots\geq\lambda_\ell>0$ with sum $n$; append zeros when comparing lengths. Its [Young diagram](../../../../../young-diagram.md) has cells $(i,j)$ with $1\leq j\leq\lambda_i$. A [Young tableau](../../../../../young-tableau.md) is a bijective filling of these cells by $1,\ldots,n$. Write $R_t,C_t$ for its [row and column stabilizers](../../../../../row-and-column-stabilizers-of-a-young-tableau.md), and fix the convention

$$
r_t=\sum_{r\in R_t}r,\qquad
c_t=\sum_{c\in C_t}\operatorname{sgn}(c)c,\qquad
h_t=c_tr_t.
$$

[Permutations](../../../../../permutation.md) act on entries on the left, with the rightmost factor acting first. This defines the [Young symmetrizer](../../../../../young-symmetrizer.md) used throughout. In the [dictionary order on integer partitions](../../../../../dictionary-order-on-integer-partitions.md), $\lambda>\mu$ means that at the first differing part $\lambda_i>\mu_i$; equality is allowed in $\geq$.

Suppose there is no row-column collision between $t$ of shape $\lambda$ and $u$ of shape $\mu$. Each column of $u$ contains at most one entry from each row of $t$. The first $k$ rows of $t$ therefore contain at most

$$
\sum_j\min(k,\mu'_j)=\sum_{i=1}^k\mu_i
$$

entries, where $\mu'_j$ is a column length. Thus $\sum_{i\leq k}\lambda_i\leq\sum_{i\leq k}\mu_i$ for every $k$: $\mu$ dominates $\lambda$ in [dominance order on partitions](../../../../../dominance-order-on-partitions.md). If $\lambda\geq\mu$ in [dictionary order on integer partitions](../../../../../dictionary-order-on-integer-partitions.md), a first strictly larger part would contradict the corresponding prefix inequality. Hence **$\lambda=\mu$**.

All the bounds must now be equalities. Every column $j$ of $u$ contains exactly one entry from row $i$ of $t$ whenever $i\leq\lambda'_j$. Choose $r_0\in R_t$ sending that entry to the entry of $t$ in cell $(i,j)$. These prescriptions are bijections within the rows. The columns of $r_0u$ then have exactly the same sets of entries as the columns of $t$, so $r_0u=c_0t$ for some $c_0\in C_t$. Consequently

$$
\boxed{u=r_0^{-1}c_0t,\quad r_0^{-1}\in R_t,\quad c_0\in C_t.}
$$

If a collision was present instead, its two entries supply the first alternative. This proves the [row-column collision lemma](../../../../../row-column-collision-lemma.md), including the prescribed order of the two stabilizer factors.

We next prove the [Specht module](../../../../../specht-module.md) classification. By [Maschke's theorem](../../../../../maschke-s-theorem.md), the [group algebra](../../../../../group-algebra.md) $A=\mathbb CS_n$ is a [semisimple algebra](../../../../../semisimple-algebra.md). Use the permitted basic quasi-idempotence of a [Young symmetrizer](../../../../../young-symmetrizer.md),

$$
h_t^2=H_\lambda h_t,\qquad
H_\lambda=\prod_{(i,j)\in\lambda}(\lambda_i-j+\lambda'_j-i+1)\ne0,
$$

and put $e_t=h_t/H_\lambda$. The coefficient of $1$ in $h_t$ is one, because $R_t\cap C_t=\{1\}$, so $e_t\ne0$.

For $\pi\in S_n$, consider $r_t\pi c_t$. A collision between the rows of $t$ and the columns of $\pi t$ gives a [transposition](../../../../../transposition-permutation.md) $\tau\in R_t\cap\pi C_t\pi^{-1}$. Row symmetrization fixes $\tau$, whereas column antisymmetrization changes its sign, so $r_t\pi c_t=0$. If there is no collision, the proved lemma gives $\pi=rc$ with $r\in R_t,c\in C_t$, and

$$
r_t\pi c_t=\operatorname{sgn}(c)r_tc_t.
$$

It follows that $h_t\pi h_t$ is zero or $\operatorname{sgn}(c)H_\lambda h_t$. Since [permutations](../../../../../permutation.md) span $A$, **$e_tAe_t=\mathbb Ce_t$**. In a [semisimple algebra](../../../../../semisimple-algebra.md) this means that $e_t$ is a [primitive idempotent](../../../../../primitive-idempotent.md), so $Ae_t=Ah_t$ is an irreducible left module.

If $\lambda>\mu$ in [dictionary order on integer partitions](../../../../../dictionary-order-on-integer-partitions.md), the collision lemma applied to every $\pi u$ gives $r_tA c_u=0$, and therefore $h_tA h_u=0$. Since

$$
\operatorname{Hom}_A(Ae_t,Ae_u)\cong e_tAe_u,
$$

the two [simple modules](../../../../../irreducible-module.md) cannot be isomorphic. Conversely, [Young tableaux](../../../../../young-tableau.md) of the same shape are related by a [permutation](../../../../../permutation.md), which conjugates their [Young symmetrizers](../../../../../young-symmetrizer.md) and gives isomorphic [left ideals](../../../../../left-ideal.md). Finally, the center of $\mathbb CS_n$ has the conjugacy-class sums as a basis. [Conjugacy classes](../../../../../conjugacy-class.md) are indexed by cycle-type partitions, so its dimension is the number of partitions of $n$. The [Artin–Wedderburn theorem](../../../../../artin-wedderburn-theorem.md) gives exactly that many simple-module isomorphism classes. We have already produced one for each partition. Thus **the $Ah_\lambda$ form a complete set of pairwise nonisomorphic [irreducible modules](../../../../../irreducible-module.md)**.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 3](../../paper-3-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
