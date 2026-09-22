<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

For a cell $(i,j)$ in the [Young diagram](../../../../../young-diagram.md) of $\lambda$, its [hook of a Young diagram](../../../../../hook-of-a-young-diagram.md) consists of that cell, the cells to its right in row $i$ and the cells below it in column $j$. Its length is

$$
h_{ij}=\lambda_i-j+\lambda'_j-i+1.
$$

A removable [rim hook](../../../../../rim-hook.md) is a connected border strip $\lambda/\mu$ containing no $2\times2$ square, whose removal leaves a [Young diagram](../../../../../young-diagram.md). Its leg length is the number of rows it meets minus one. The [hook graph](../../../../../hook-graph-of-a-partition.md) is the [Young diagram](../../../../../young-diagram.md) labeled at each cell by $h_{ij}$; here “graph” means this labeled array, not a graph of possible hook-walk moves.

Choose $l\ge\ell(\lambda)$, pad with zeros and form the [beta numbers](../../../../../beta-number-of-a-partition.md)

$$
\boxed{\beta_i=\lambda_i+l-i,\qquad i=1,\ldots,l.}
$$

They are distinct nonnegative integers in decreasing order and recover $\lambda_i=\beta_i-l+i$. For $l=\ell(\lambda)$ they equal the first-column [hook lengths](../../../../../hook-length.md), since $h_{i1}=\lambda_i+l-i$. If $l$ is increased, old [beta numbers](../../../../../beta-number-of-a-partition.md) shift upward by one and a new bead at zero is inserted.

For a prime-modulus [partition abacus](../../../../../abacus-of-a-partition.md) arrange the nonnegative positions in $p$ runners: position $pq+r$ lies at level $q$ on runner $r$, $0\le r<p$. Put beads at the [beta numbers](../../../../../beta-number-of-a-partition.md) and leave the other positions empty. Replacing a bead at $b$ by a bead at a vacant $b-k\ge0$ removes a [rim hook](../../../../../rim-hook.md) of length $k$; its leg length is the number of beads strictly between these positions. This follows by tracing the boundary of the diagram: bead positions record vertical steps and gaps record horizontal steps, and exchanging one bead and gap removes the intervening border strip. In particular a removable $p$-hook is exactly a bead that can slide up one place on its own runner.

The [partition core](../../../../../core-of-a-partition.md) at modulus $p$ is the result of sliding beads up until there are no gaps above any bead on a runner. If runner $r$ initially has $b_r$ beads, its final occupied levels must be $0,1,\ldots,b_r-1$, independently of slide order. Thus its packed [beta set](../../../../../beta-set-of-a-partition.md), and hence its core [partition of an integer](../../../../../partition-of-an-integer.md), is unique. Increasing the number of [beta numbers](../../../../../beta-number-of-a-partition.md) merely re-expresses the same boundary by shifting positions and adding the new initial bead; the packed configuration represents the same [partition of an integer](../../../../../partition-of-an-integer.md). This proves well-definedness both with respect to removal order and to the chosen padding. The number of slides is

$$
w_p(\lambda)=\frac{|\lambda|-|\operatorname{core}_p\lambda|}{p}.
$$

The [partition quotient](../../../../../quotient-of-a-partition.md) components record how far each runner's beads lie above their packed positions, giving the hook-removal interpretation used in Question 5.

A [block of a group algebra](../../../../../block-of-a-group-algebra.md) in [characteristic](../../../../../characteristic-of-a-field.md) $p$ for $FS_n$ is a two-sided ideal $B=FS_ne$ for a [primitive central idempotent](../../../../../primitive-central-idempotent.md) $e$, meaning a nonzero [central idempotent](../../../../../central-idempotent.md) that is not a sum of two nonzero orthogonal [central idempotents](../../../../../central-idempotent.md). The identity is the sum of these block [idempotents](../../../../../idempotent.md) and the [group algebra](../../../../../group-algebra.md) is their direct product. An [indecomposable module](../../../../../indecomposable-module.md) $V$ belongs to $B$ when $eV=V$, equivalently every other block [idempotent](../../../../../idempotent.md) acts as zero. Indeed $V=\bigoplus_e eV$; indecomposability makes exactly one summand nonzero.

The [Nakayama block theorem](../../../../../nakayama-block-theorem.md), historically called the Nakayama Conjecture, states

$$
\boxed{S_F^\lambda\text{ and }S_F^\mu\text{ belong to the same }p\text{-block}
\iff\operatorname{core}_p(\lambda)=\operatorname{core}_p(\mu).}
$$

Equivalently the [ordinary characters](../../../../../ordinary-character.md) assigned to one modular block have a common [partition core](../../../../../core-of-a-partition.md) at modulus $p$. Its [simple modules](../../../../../irreducible-module.md) are the $D^\lambda$ with regular $\lambda$ having that core. Only cores $\kappa$ for which $n-|\kappa|$ is a nonnegative multiple of $p$ occur. The block weight is $(n-|\kappa|)/p$; a core alone determines the block at this fixed degree.

One route to the proof separates the combinatorial core invariant from the algebraic center invariant. Let $c_r(\lambda)$ be the number of cells of residue $r=j-i\pmod p$. A length-$p$ [rim hook](../../../../../rim-hook.md) has one cell of every residue: along its border strip the contents are consecutive integers. Therefore removal subtracts one from every $c_r$. More precisely, choose the number $l$ of [beta numbers](../../../../../beta-number-of-a-partition.md) divisible by $p$ and write the runner charges as $q_r=b_r-l/p$. Reading the boundary, or adding a cell and checking its two changed beta positions, gives

$$
q_r=c_r-c_{r+1}\qquad(r\bmod p).
$$

The charges determine the packed runners and hence the core. For fixed $n$, two equal cores have the same weight, so their full residue multisets are equal. Conversely equal residue multisets give equal charges and the same core. This establishes

$$
\operatorname{core}_p\lambda=\operatorname{core}_p\mu\iff (c_0(\lambda),\ldots,c_{p-1}(\lambda))=(c_0(\mu),\ldots,c_{p-1}(\mu))
$$

for [partitions of an integer](../../../../../partition-of-an-integer.md) of the same integer. The fixed-degree condition matters.

For the center invariant, use the commuting [Jucys–Murphy elements](../../../../../jucys-murphy-element.md) $J_k=\sum_{i<k}(i\ k)$, with $J_1=0$. In the [Young seminormal form](../../../../../young-seminormal-form.md) basis, $J_k$ has eigenvalue equal to the content of the cell containing $k$. A [symmetric polynomial](../../../../../symmetric-polynomial.md) in them therefore acts on $S^\lambda$ as the same scalar for every [Young tableau](../../../../../young-tableau.md): its value on the multiset of all contents of $\lambda$. The integral Specht lattice makes this a scalar identity before modular reduction, so modulo $p$ these central scalars depend only on the residue multiset, and every [composition factor](../../../../../composition-factor.md) inherits them.

The substantive center theorem used in this proof is that the center of the symmetric-group algebra, integrally and over a [field](../../../../../field.md), consists of [symmetric polynomials](../../../../../symmetric-polynomial.md) in the [Jucys–Murphy elements](../../../../../jucys-murphy-element.md). Centrality of elementary [symmetric polynomials](../../../../../symmetric-polynomial.md) follows from

$$
\prod_{k=1}^n(t+J_k)=\sum_{g\in S_n}t^{\#\text{cycles}(g)}g;
$$

the coefficients are central class-sum combinations. The reverse inclusion requires the integral triangular class-sum argument: expand symmetric monomials in the $J_k$ as products of [transpositions](../../../../../transposition-permutation.md), group the leading terms by reduced [cycle type](../../../../../cycle-type.md), and eliminate these leading [class sums](../../../../../conjugacy-class-sum.md) in the resulting unitriangular order. The integral coefficients, with no division by multiples of $p$, are crucial; knowing the center only over $\mathbb Q$ would not prove the modular assertion. This is the central algebraic ingredient of this proof route.

Thus equal residue multisets yield equal [characters](../../../../../character-of-a-representation.md) of the entire modular center. Different residue multisets are separated already by the coefficients of the central [polynomial](../../../../../polynomial-split.md) $\prod_k(t+J_k)$: its scalar on the shape $\lambda$ reduces to $\prod_r(t+r)^{c_r(\lambda)}$, whose unique factorization records the multiplicities exactly, even in [characteristic](../../../../../characteristic-of-a-field.md) $p$. In a finite-dimensional split algebra, two [simple modules](../../../../../irreducible-module.md) are in the same block exactly when their central [characters](../../../../../character-of-a-representation.md) agree: the center of each block is local, while different block [idempotents](../../../../../idempotent.md) separate different blocks. It follows that equal cores give one block and different cores give distinct blocks. This proves both directions rather than just observing that core is constant on known blocks.

Finally, each ordinary Specht lattice has a single reduced central [character](../../../../../character-of-a-representation.md), so all constituents of its reduction lie in that one block. Question 1 supplies every [simple module](../../../../../irreducible-module.md) and its label; the regular labels therefore identify all the simples in each core block. The constructions use integer coefficients and absolutely [irreducible](../../../../../irreducible-representation.md) prime-field [modules](../../../../../module-mathematics.md), so the block description descends to the arbitrary characteristic-$p$ [field](../../../../../field.md) in the question. This completes the main steps of the block proof without presupposing semisimplicity in positive [characteristic](../../../../../characteristic-of-a-field.md).

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 4](../../paper-4-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
