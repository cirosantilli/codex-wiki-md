<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

A [standard Young tableau](../../../../../standard-young-tableau.md) has its entries increasing from left to right in each row and from top to bottom in each column. For the convention $h_t=c_tr_t$, use [column-reading order of standard Young tableaux](../../../../../column-reading-order-of-standard-young-tableaux.md): read columns from left to right, each from top to bottom, and compare the resulting words lexicographically. This makes the requested product direction explicit. The order and the symmetrizer multiplication convention must be chosen together.

We prove the vanishing claim. Suppose the rows of $t$ and the columns of $u$ have no collision. The argument in Question 1 shows that every column of $u$ contains one entry from each eligible row of $t$. Its first column thus selects one entry from every row. Each selected entry is at least the first entry of that row in $t$. Sorting the selected entries, as the [standard tableau](../../../../../standard-young-tableau.md) $u$ does, gives a column componentwise at least the first column of $t$: increasing individual entries cannot decrease any order statistic. If the columns are equal, equality of their sums forces every selected entry to be that row's first entry. Delete this common column and repeat. At the first differing column, its first differing entry in $u$ is therefore larger; otherwise $u=t$. Thus absence of a collision implies $u\geq t$ in [column-reading order of standard Young tableaux](../../../../../column-reading-order-of-standard-young-tableaux.md).

If $t>u$, there must instead be a [transposition](../../../../../transposition-permutation.md) in $R_t\cap C_u$. It fixes $r_t$ and negates $c_u$, giving $r_tc_u=0$. Hence

$$
\boxed{h_th_u=c_t(r_tc_u)r_u=0\qquad(t>u).}
$$

This is [triangular vanishing of Young-symmetrizer products](../../../../../triangular-vanishing-of-young-symmetrizer-products.md); it does not assert vanishing in the opposite order.

Normalize to $e_t=h_t/H_\lambda$. List all [standard tableaux](../../../../../standard-young-tableau.md) in increasing shape [dictionary order on integer partitions](../../../../../dictionary-order-on-integer-partitions.md), and within each shape in increasing [column-reading order of standard Young tableaux](../../../../../column-reading-order-of-standard-young-tableaux.md). Then $e_ie_j=0$ for $i>j$, using Question 1 between different shapes and the result above within a shape. The [left ideals](../../../../../left-ideal.md) $Ae_i$ have an internal [direct sum](../../../../../direct-sum.md): if $\sum_i z_i=0$ with $z_i\in Ae_i$, multiply on the right by $e_1$ to get $z_1=0$, since $z_1e_1=z_1$ and every later $z_ie_1=0$. Repeat with $e_2,e_3,\ldots$. This proves directness without incorrectly treating all the [idempotents](../../../../../idempotent.md) as mutually orthogonal.

Let $f_\lambda$ count the [standard tableaux](../../../../../standard-young-tableau.md) of shape $\lambda$ and let $d_\lambda=\dim S^\lambda$. In the [regular representation](../../../../../regular-representation.md) a [simple module](../../../../../irreducible-module.md) of dimension $d_\lambda$ occurs $d_\lambda$ times, by the [Artin–Wedderburn theorem](../../../../../artin-wedderburn-theorem.md). The [direct sum](../../../../../direct-sum.md) just constructed contains $f_\lambda$ copies of $S^\lambda$, so $f_\lambda\leq d_\lambda$ for every shape. We supply the needed counting identity independently of the dimension conclusion.

The [Robinson–Schensted correspondence](../../../../../robinson-schensted-correspondence.md) bijects [permutations](../../../../../permutation.md) with pairs of [standard tableaux](../../../../../standard-young-tableau.md) of the same shape. Here is its [row insertion](../../../../../row-insertion.md) construction and inverse. Insert the successive [permutation](../../../../../permutation.md) entries into an increasing row by replacing its first entry larger than the incoming entry, bumping that replaced entry into the next row; if no entry is larger, append at the row end. Continue until a new cell is created. Record the insertion time in that cell of a second tableau. For completeness, the successive bumped entries strictly increase, and their column indices weakly decrease: an entry below a bumped entry was originally larger, so the next replacement occurs no farther right. The entry newly placed in each row is smaller than the entry removed and larger than the entry above it. At a strictly earlier column, that last inequality follows from row increase in the preceding row; at the same column, it follows from the preceding bump. Hence the insertion tableau keeps increasing rows and columns. If a new cell is appended below the first row, the preceding bump guarantees that the row above reaches that column, so the shape stays a [Young diagram](../../../../../young-diagram.md). Recording times also increase in rows and columns, since every new cell is an outer corner of the current diagram. Thus both tableaux are standard at the end. Conversely, remove the cell with the largest recording label. Reverse its bumping path upward, replacing in each preceding row the rightmost entry smaller than the moving entry and moving the displaced entry upward. This recovers the last inserted letter; iterating recovers the entire [permutation](../../../../../permutation.md). The two rules undo one another at each row. Thus

$$
n!=\sum_{\lambda\vdash n}f_\lambda^2.
$$

Semisimplicity also gives $n!=\sum_\lambda d_\lambda^2$. Since $0\leq f_\lambda\leq d_\lambda$ termwise, equality of these sums forces $f_\lambda=d_\lambda$ for every shape. The internal [direct sum](../../../../../direct-sum.md) has dimension $n!$ and hence fills $A$:

$$
\boxed{A=\bigoplus_{\lambda\vdash n}\ \bigoplus_{t\in\operatorname{SYT}(\lambda)}Ah_t,
\qquad \dim S^\lambda=\#\operatorname{SYT}(\lambda).}
$$

There is also a useful numerical form. Right multiplication by $e_t$ is an [idempotent](../../../../../idempotent.md) with image $Ae_t$. In the [permutation](../../../../../permutation.md) basis of $A$, each diagonal coefficient is the coefficient of $1$ in $e_t$, namely $1/H_\lambda$. Its trace equals its rank, so **$\dim S^\lambda=n!/H_\lambda$**. Together with the count just obtained this recovers the [hook-length formula](../../../../../hook-length-formula.md).

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 3](../../paper-3-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
