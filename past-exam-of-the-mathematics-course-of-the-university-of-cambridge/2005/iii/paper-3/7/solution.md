<h1 id="7/solution">Solution</h1>

↑ **Parent:** [7](../7.md)

A [rim hook](../../../../../rim-hook.md) is a connected skew diagram containing no $2\times2$ square, whose removal leaves a [partition of an integer](../../../../../partition-of-an-integer.md) diagram. Its leg length is its number of occupied rows minus one. The [Murnaghan–Nakayama rule](../../../../../murnaghan-nakayama-rule.md) states that, if a [permutation](../../../../../permutation.md) has cycle type $(k,\rho)$, then

$$
\boxed{\chi^\lambda(k,\rho)=
\sum_{\eta:\lambda/\eta\text{ a rim hook of size }k}
(-1)^{\operatorname{leg}(\lambda/\eta)}\chi^\eta(\rho).}
$$

Iteration removes one hook for each cycle length; the empty diagram has [character](../../../../../character-of-a-representation.md) one at the empty cycle type.

For shape $(3,3,3)$ and cycle type $(4,3,2)$, there are exactly two removable four-cell [rim hooks](../../../../../rim-hook.md). The remaining shapes are $(3,2)$ and $(2,2,1)$; the removed hooks have leg lengths one and two respectively. In shape $(3,2)$ the only removable three-cell [rim hook](../../../../../rim-hook.md) leaves $(1,1)$ and has leg length one. In shape $(2,2,1)$ the only such hook leaves $(2)$ and again has leg length one. Since the [characters](../../../../../character-of-a-representation.md) of $(1,1)$ and $(2)$ at a transposition are $-1$ and $1$, we obtain

$$
\chi^{(3,2)}(3,2)=1,\qquad
\chi^{(2,2,1)}(3,2)=-1,
$$

and hence

$$
\boxed{\chi^{(3^3)}((1234)(56)(789))=-1-1=-2.}
$$

The cycle lengths can be taken in any order; using $4,3,2$ makes the two branches of the computation explicit.

Now consider the ordinary induction product $[\alpha][\beta]$. A [hook partition](../../../../../hook-partition.md) is $(x,1^y)$, equivalently a [partition of an integer](../../../../../partition-of-an-integer.md) whose second row has length at most one. If a hook shape $\nu$ occurs in the [Littlewood–Richardson rule](../../../../../littlewood-richardson-rule.md), then $\alpha\subseteq\nu$, forcing $\alpha$ itself to be a hook. In the skew hook $\nu/\alpha$, the new cells consist of a segment in the first row and a segment down the first column, with no shared column between those two segments. Every first-row entry must be $1$: its rightmost entry is the first letter of the [lattice word](../../../../../lattice-word.md), hence is $1$, and weak row increase forces all entries to its left to be $1$ too. The column segment has strictly increasing entries. Thus only $1$ can be repeated, forcing the content $\beta$ to be a hook as well. This also proves the assertion when the top segment is empty, since then every entry lies in a strictly increasing column.

Write the two nonempty hook factors as $\alpha=(a,1^k)$ and $\beta=(b,1^l)$, with $k=n-r-a$ and $l=r-b$. Let the prospective resulting hook have top-row length $x$ and leg length $y$. Its new top segment has $H=x-a$ cells and its new column segment has $V=y-k$ cells. The content consists of $b$ ones and the single letters $2,\ldots,l+1$. All those larger letters must be in the new column; its strict increase allows either no $1$ or exactly one $1$. There are therefore only two possibilities:

$$
(H,V)=(b,l)\quad\text{or}\quad(b-1,l+1).
$$

In the first case fill the top segment with $b$ ones and the column with $2,3,\ldots,l+1$. In the second, use $b-1$ top ones and column $1,2,\ldots,l+1$. Each filling is unique and has a [lattice word](../../../../../lattice-word.md), including the case $b=1$ with an empty top segment in the second filling. This proves

$$
\boxed{[a,1^{n-r-a}][b,1^{r-b}]
=[a+b,1^{n-a-b}]+[a+b-1,1^{n-a-b+1}]
+\text{non-hook constituents}.}
$$

Both displayed multiplicities are one.

To deduce the full-cycle value from this product result, rather than quote the [Murnaghan–Nakayama rule](../../../../../murnaghan-nakayama-rule.md) again, form the virtual [character](../../../../../character-of-a-representation.md)

$$
F_n=\sum_{j=0}^{n-1}(-1)^j\chi^{(n-j,1^j)}.
$$

For every proper [Young subgroup](../../../../../young-subgroup.md) $S_m\times S_{n-m}$ and every pair of its [irreducible characters](../../../../../irreducible-character.md), the hook-product calculation gives

$$
\left\langle F_n,\operatorname{Ind}_{S_m\times S_{n-m}}^{S_n}
(\chi^\alpha\boxtimes\chi^\beta)\right\rangle=0.
$$

If a factor is not a hook there are no hook constituents; if both are hooks, their two consecutive leg lengths cancel in this alternating inner product. By [Frobenius reciprocity](../../../../../frobenius-reciprocity.md) and the completeness of the product [irreducible characters](../../../../../irreducible-character.md), $F_n$ restricts to zero on every such subgroup. Any [permutation](../../../../../permutation.md) with more than one cycle preserves a nonempty proper subset and is conjugate into one of these subgroups. Thus $F_n$ is supported only on the class of $n$-cycles.

Its inner product with the trivial [character](../../../../../character-of-a-representation.md) is one, since only the one-row hook contributes. That class has size $(n-1)!$, so $F_n(\rho)/n=1$, giving $F_n(\rho)=n$. For any [irreducible character](../../../../../irreducible-character.md), the support calculation then yields

$$
\langle F_n,\chi^\nu\rangle=\overline{\chi^\nu(\rho)}.
$$

By [character orthogonality](../../../../../character-orthogonality.md), the left side is $(-1)^{n-x}$ for $\nu=(x,1^{n-x})$ and zero otherwise. These are real integers, proving

$$
\boxed{\chi^\nu(\rho)=
\begin{cases}(-1)^{n-x},&\nu=(x,1^{n-x}),\\0,&\nu\text{ is not a hook}.\end{cases}}
$$

For $n=1$ the same conclusion holds directly. This derives the requested special case from the [Littlewood–Richardson rule](../../../../../littlewood-richardson-rule.md) and [Frobenius reciprocity](../../../../../frobenius-reciprocity.md).

## ↑ Ancestors (10)

1. [7](../7.md)
2. [Paper 3](../../paper-3-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
