<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

For a [rational matrix](../../../../../rational-matrix.md) $A$ with columns $a_1,\ldots,a_n$, [partition regularity](../../../../../partition-regular-matrix.md) means that every [finite colouring](../../../../../finite-coloring.md) of the [positive integers](../../../../../positive-integer.md) admits a positive [monochromatic](../../../../../monochromatic-set.md) [vector](../../../../../vector.md) $x$ with $Ax=0$. Repeated coordinates are allowed. The [columns condition](../../../../../columns-property.md) is an ordered partition $\{1,\ldots,n\}=B_1\sqcup\cdots\sqcup B_s$ into nonempty blocks such that

$$
\sum_{i\in B_1}a_i=0,\qquad
\sum_{i\in B_j}a_i\in\operatorname{span}_{\mathbb Q}\{a_i:i\in B_1\cup\cdots\cup B_{j-1}\}\quad(j\ge2).
$$

[Rado's theorem](../../../../../rado-s-theorem.md) says that **$A$ is partition regular if and only if it satisfies the [columns condition](../../../../../columns-property.md)**. We prove both directions.

For necessity, clear denominators so the columns are [integer](../../../../../integer.md) [vectors](../../../../../vector.md). For every pair of disjoint index sets $I,B$ with $B\ne\varnothing$ for which $\sum_{i\in B}a_i$ is not in the rational [linear span](../../../../../linear-span.md) of the I-columns, choose an [integer](../../../../../integer.md) [linear functional](../../../../../linear-functional.md) $\ell_{I,B}$ that vanishes on those I-columns but not on that sum. Such a functional exists by finite-dimensional [linear algebra](../../../../../linear-algebra-split.md); clear its rational denominators. There are only finitely many pairs, so choose a [prime number](../../../../../prime-number.md) $p$ dividing none of the nonzero [integers](../../../../../integer.md)

$$
\ell_{I,B}\left(\sum_{i\in B}a_i\right).
$$

If there are no offending pairs, any [prime number](../../../../../prime-number.md) suffices.

Colour a [positive integer](../../../../../positive-integer.md) $x=p^{v_p(x)}u$, $p\nmid u$, by $u\bmod p$. This is the [last nonzero digit coloring](../../../../../last-nonzero-digit-coloring.md), using $p-1$ colours. [Partition regularity](../../../../../partition-regular-matrix.md) gives a positive [monochromatic](../../../../../monochromatic-set.md) solution. Group its coordinate indices by their distinct [P-adic valuations](../../../../../p-adic-valuation.md) $e_1<\cdots<e_s$, writing $B_j=\{i:v_p(x_i)=e_j\}$. All units $x_i/p^{e_j}$ have the same nonzero residue $\alpha$ modulo $p$.

For each $j$, let $I=B_1\cup\cdots\cup B_{j-1}$. If its block sum failed the required span condition, apply the chosen $\ell_{I,B_j}$ to $\sum_i a_ix_i=0$. The earlier terms vanish exactly, not just modulo a power of $p$. Divide by $p^{e_j}$; terms with later valuations are still divisible by $p$. Reduction modulo $p$ then yields

$$
0=\alpha\,\ell_{I,B_j}\left(\sum_{i\in B_j}a_i\right)\pmod p,
$$

contrary to the choice of $p$. Thus every required span relation holds, and with $I=\varnothing$ the first block sum is zero. This is the [finite separating-functional proof of the columns condition](../../../../../finite-separating-functional-proof-of-the-columns-condition.md); it avoids an unjustified passage from congruences to rational equality.

For sufficiency, assume the [columns condition](../../../../../columns-property.md). Choose rational coefficients $\lambda_{ij}$, for $j\ge2$ and $i\in B_1\cup\cdots\cup B_{j-1}$, such that

$$
\sum_{i\in B_j}a_i+\sum_{i\in B_1\cup\cdots\cup B_{j-1}}\lambda_{ij}a_i=0.
$$

Choose a [positive integer](../../../../../positive-integer.md) $c$ clearing every denominator, and a [positive integer](../../../../../positive-integer.md) $p\ge\max|c\lambda_{ij}|$, taking $p=1$ if the list is empty. By the allowed [monochromatic m-p-c set theorem](../../../../../monochromatic-m-p-c-set-theorem.md), there are positive generators $z_1,\ldots,z_s$ such that all numbers

$$
cz_h+\sum_{j>h}\mu_jz_j,\qquad \mu_j\in\mathbb Z,\quad |\mu_j|\le p,
$$

are positive and have one colour. This is a full [m-p-c set](../../../../../m-p-c-set.md); positivity is part of its definition, not a rule discarding negative expressions. For $i\in B_h$, put

$$
x_i=cz_h+\sum_{j>h}c\lambda_{ij}z_j.
$$

These coordinates all belong to that [monochromatic](../../../../../monochromatic-set.md) [m-p-c set](../../../../../m-p-c-set.md). Collecting coefficients of $z_j$ gives

$$
\sum_i a_ix_i
=c z_1\sum_{i\in B_1}a_i+
\sum_{j=2}^s c z_j\left(\sum_{i\in B_j}a_i+\sum_{i\in B_1\cup\cdots\cup B_{j-1}}\lambda_{ij}a_i\right)=0.
$$

Thus the [Rado solution inside an m-p-c set](../../../../../rado-solution-inside-an-m-p-c-set.md) proves [partition regularity](../../../../../partition-regular-matrix.md) and completes the theorem.

To obtain the [Finite sums theorem](../../../../../finite-sums-theorem.md) from [Rado's theorem](../../../../../rado-s-theorem.md), introduce a positive variable $y_F$ for every nonempty $F\subseteq\{1,\ldots,k\}$ and impose

$$
y_F-\sum_{i\in F}y_{\{i\}}=0\qquad(|F|\ge2).
$$

Partition the columns of this system into $B_j=\{F:\min F=j\}$. The $B_1$-column sum is zero: in a row indexed by $F$ containing $1$, the contributions of $y_F$ and $y_{\{1\}}$ cancel, and other rows receive neither. For $j>1$, the $B_j$-column sum is

$$
-\sum_{\substack{F:\min F<j\\j\in F}}a_F,
$$

where $a_F$ is the column of $y_F$. Those columns lie in earlier blocks. Hence the [columns condition](../../../../../columns-property.md) holds. A [monochromatic](../../../../../monochromatic-set.md) positive solution gives $x_i=y_{\{i\}}$ and $y_F=\sum_{i\in F}x_i$, proving

$$
\boxed{\operatorname{FS}(x_1,\ldots,x_k)\text{ is monochromatic}.}
$$

For $k=1$ the system has no rows and the conclusion is immediate. The construction is also visible directly in the sufficiency proof: a [monochromatic](../../../../../monochromatic-set.md) $(k,1,1)$-set contains every nonempty sum of its generators, classified by the smallest chosen index.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 12](../../paper-12-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
