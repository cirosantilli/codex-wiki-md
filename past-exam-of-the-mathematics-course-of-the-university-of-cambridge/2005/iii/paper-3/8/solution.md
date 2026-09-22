<h1 id="8/solution">Solution</h1>

↑ **Parent:** [8](../8.md)

Choose $m\ge\ell(\lambda)$, pad the [partition of an integer](../../../../../partition-of-an-integer.md) with zeros, and define its [beta numbers](../../../../../beta-number-of-a-partition.md) by

$$
\beta_i=\lambda_i+m-i\quad(1\le i\le m).
$$

They form a strictly decreasing set of nonnegative integers. Conversely, from its decreasing enumeration recover $\lambda_i=\beta_i-m+i$. With $m=\ell(\lambda)$ these are exactly the first-column [hook lengths](../../../../../hook-length.md), since $h_{i1}=\lambda_i+\lambda'_1-i=\lambda_i+m-i$. Padding changes the numbers: increasing $m$ by one replaces $B$ by $\{0\}\cup(B+1)$, and leaves the represented [partition of an integer](../../../../../partition-of-an-integer.md) unchanged.

Arrange positions $0,1,2,\ldots$ on $p$ runners, putting position $r+pk$ on runner $r$ at height $k$. A bead occupies each position in the [beta set](../../../../../beta-set-of-a-partition.md). This is the [abacus of a partition](../../../../../abacus-of-a-partition.md). The [hook criterion in a beta set](../../../../../hook-criterion-in-a-beta-set.md) says that a bead $b$ and a gap $a<b$ correspond to a hook of length $b-a$; replacing $b$ by $a$ removes the corresponding [rim hook](../../../../../rim-hook.md). In particular removing a rim $p$-hook moves a bead from $b$ to the vacant position $b-p$ immediately above it on the same runner. Its leg length counts the beads in the intervening positions of the full linear numbering.

For an explicit example, take $\lambda=(4,2,1)$, $p=3$, and $m=3$. Its [beta set](../../../../../beta-set-of-a-partition.md) is $\{6,3,1\}$. Runner zero has beads at $3,6$, runner one has a bead at $1$, and runner two is empty. Packing upwards gives $\{3,1,0\}$, which represents $(1)$; thus the three-core is $(1)$ and the weight is two.

Every bead slide reduces the sum of occupied positions, so repeated slides terminate. The number $n_r$ of beads on each runner is unchanged. At termination they must occupy exactly

$$
r,r+p,\ldots,r+p(n_r-1)
$$

on runner $r$, since any gap above a bead would allow a further slide. Hence the final [beta set](../../../../../beta-set-of-a-partition.md) is uniquely determined by the initial runner counts, independently of the order of hook removals. Increasing the number of beads by $p$ replaces $B$ by $\{0,\ldots,p-1\}\cup(B+p)$, adds one bead to each runner, and gives exactly the same represented core after packing. General changes in padding follow by applying $B\mapsto\{0\}\cup(B+1)$; packing commutes with this operation up to the cyclic relabelling of runners. Therefore the result is independent of both removal order and padding:

$$
\boxed{\text{the }p\text{-core }C_p(\lambda)\text{ is well-defined}.}
$$

The [weight of a partition](../../../../../weight-of-a-partition.md) is $w_p(\lambda)=(n-|C_p(\lambda)|)/p$.

A [block of a group algebra](../../../../../block-of-a-group-algebra.md) is an indecomposable two-sided summand $FS_ne$, where $e$ is a primitive central [idempotent](../../../../../idempotent.md). The identity decomposes into pairwise orthogonal such [idempotents](../../../../../idempotent.md); a [module](../../../../../module-mathematics.md) belongs to a block when its [idempotent](../../../../../idempotent.md) acts as identity and the other block [idempotents](../../../../../idempotent.md) act as zero. For [ordinary characters](../../../../../ordinary-character.md), use a splitting [p-modular system](../../../../../p-modular-system.md) $(K,\mathcal O,F)$, or extend the residue [field](../../../../../field.md) first: the block [idempotents](../../../../../idempotent.md) lift to $\mathcal O S_n$, and determine which ordinary [irreducible](../../../../../irreducible-representation.md) $KS_n$-modules lie in each $p$-block. The symmetric group is split over its prime [field](../../../../../field.md), so extending $F$ introduces no change to the resulting [partition of an integer](../../../../../partition-of-an-integer.md) labels.

The [Nakayama block theorem](../../../../../nakayama-block-theorem.md), traditionally called the [Nakayama Conjecture for symmetric groups](../../../../../nakayama-block-theorem.md), is

$$
\boxed{\chi^\lambda\text{ and }\chi^\mu\text{ belong to the same }p\text{-block}
\iff C_p(\lambda)=C_p(\mu).}
$$

The simple [modules](../../../../../module-mathematics.md) in that block are exactly the $D^\nu$ with regular labels having that core. At fixed $n$, the common core also fixes the weight. Here is an essay proof route through central [characters](../../../../../character-of-a-representation.md), specifying the main algebraic and combinatorial steps and why each is needed.

First introduce the commuting [Young–Jucys–Murphy elements](../../../../../jucys-murphy-element.md)

$$
J_1=0,\qquad J_i=\sum_{j<i}(j\ i)\in\mathbb ZS_n.
$$

Their commutators vanish because contributions supported on each triple of letters cancel. Symmetric polynomials in the $J_i$ are central: for adjacent transpositions $s_i$, the relations $s_iJ_i=J_{i+1}s_i-1$, $s_iJ_{i+1}=J_is_i+1$ show that $s_i$ commutes with symmetric expressions in $J_i,J_{i+1}$, and it commutes with the other $J_j$. Since these transpositions generate $S_n$, the symmetric expressions commute with the whole [group algebra](../../../../../group-algebra.md).

The substantial generation ingredient is the integral [Jucys–Murphy description of the center of a symmetric-group algebra](../../../../../jucys-murphy-description-of-the-center-of-a-symmetric-group-algebra.md): every conjugacy-class sum is an integral symmetric polynomial in the $J_i$. Its proof expands symmetric monomials in these sums of transpositions and organizes the resulting class sums by the number of moved letters and cycle filtration; triangular elimination supplies integral spanning, rather than merely rational spanning. A useful first identity in this construction is

$$
\prod_{i=1}^n(t+J_i)=\sum_{g\in S_n}t^{\#\text{cycles of }g}g.
$$

Indeed, when adjoining the letter $n$, either choose $t$ and leave it as a singleton cycle, or choose a transposition $(j\ n)$ and insert it into the cycle containing $j$; this gives every [permutation](../../../../../permutation.md) uniquely. The full generation step distinguishes the individual class sums which this first identity groups together. Its integrality is essential: a description only over $\mathbb Q$ could use denominators divisible by $p$ and would not prove generation of the modular center. Since class sums form the integral basis of the center, this integral theorem reduces to the same generation statement over $F$.

Next determine their scalar action. In the characteristic-zero tableau basis of $S^\lambda$, $J_i$ is diagonal with entry the [Content of a Young-diagram cell](../../../../../content-of-a-young-diagram-cell.md) occupied by $i$, namely column minus row. This follows recursively along the multiplicity-free branching chain: the commuting operators preserve each path line, and $J_{i+1}=s_iJ_is_i+s_i$ determines the successive [eigenvalues](../../../../../eigenvalue.md). Consequently a symmetric polynomial $f(J_1,\ldots,J_n)$ acts on $S^\lambda$ by

$$
f\bigl(\{j-i:(i,j)\in\lambda\}\bigr).
$$

This is independent of the ordering of the cells. The scalar identity holds on the integral Specht lattice, so after modular reduction it depends only on the multiset of contents modulo $p$. Every [composition factor](../../../../../composition-factor.md) has this same [central character of a block](../../../../../central-character-of-a-block.md).

Two simple [modules](../../../../../module-mathematics.md) are in the same block exactly when their central [characters](../../../../../character-of-a-representation.md) agree. The center of a block is a commutative local finite-dimensional algebra; its semisimple quotient gives one scalar [character](../../../../../character-of-a-representation.md), while the orthogonal block [idempotents](../../../../../idempotent.md) separate different blocks. By the generation theorem, equality on all symmetric polynomials in the $J_i$ is enough. Conversely, different residue multisets are detected by elementary symmetric polynomials: the monic polynomial $\prod_{(i,j)\in\lambda}(z-(j-i))$ over $F$ recovers the multiplicity of each residue by unique factorization, including multiplicities larger than $p$. Thus block equivalence is exactly equality of the integers

$$
c_r(\lambda)=\#\{(i,j)\in\lambda:j-i\equiv r\pmod p\},\qquad r\in\mathbb Z/p\mathbb Z.
$$

This gives the [residue-content criterion for symmetric-group blocks](../../../../../residue-content-criterion-for-symmetric-group-blocks.md) without assuming that the sum of contents alone distinguishes blocks.

Finally identify residue content with the core. A removable rim $p$-hook has consecutive contents modulo $p$, hence removes one cell of each residue. Therefore shapes with the same core and the same size have the same residue counts. For the converse choose $m$ divisible by $p$ and at least $n$, and write $q_r=n_r-m/p$ for the runner charges. Starting from the empty [partition of an integer](../../../../../partition-of-an-integer.md) gives $q_r=0$. Adding a cell of residue $r$ moves a beta-number bead from residue $r-1$ to residue $r$, increasing $q_r$ and decreasing $q_{r-1}$. The same changes occur in $c_s-c_{s+1}$ when $c_r$ increases by one. Induction on the cells therefore gives

$$
q_r=c_r-c_{r+1}\qquad(r\text{ interpreted modulo }p).
$$

Equal residue counts give equal charges and hence equal packed runner configurations, so they give the same core. This completes both directions of the block criterion. The argument exposes the three essential bridges: integral center generation, its scalar content evaluation, and the abacus identification of residue data with a unique core.

## ↑ Ancestors (10)

1. [8](../8.md)
2. [Paper 3](../../paper-3-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
