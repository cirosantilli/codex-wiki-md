<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Use the uniform [Frankl-Wilson theorem](../../../../../frankl-wilson-theorem.md): if $p$ is a [prime number](../../../../../prime-number.md), $L\subseteq\mathbb F_p$ has $s$ distinct residues, $s\leq\min\{r,n-r\}$, and an $r$-[uniform set family](../../../../../uniform-set-family.md) $\mathcal F$ has distinct-member intersection sizes in $L$ modulo $p$ while $r\bmod p\notin L$, then

$$
|\mathcal F|\leq\binom ns.
$$

Here is a [polynomial method in combinatorics](../../../../../polynomial-method-in-combinatorics.md) proof. For each $A\in\mathcal F$, form the [intersection polynomial](../../../../../intersection-polynomial.md)

$$
f_A(x)=\prod_{\lambda\in L}\left(\sum_{i\in A}x_i-\lambda\right)
$$

over $\mathbb F_p$, and use [multilinear reduction on the Boolean cube](../../../../../multilinear-reduction-on-the-boolean-cube.md) so its degree is at most $s$. At the [characteristic vector](../../../../../characteristic-vector-of-a-set.md) of $B\in\mathcal F$, this evaluates to zero for $A\ne B$ and is nonzero for $A=B$. Consequently these evaluation functions are [linearly independent](../../../../../linear-independence.md).

The [low-degree evaluation rank on a uniform layer](../../../../../low-degree-evaluation-rank-on-a-uniform-layer.md) bounds their space by $\binom ns$. To justify that step without division by a possibly zero residue, form the integer incidence matrix with rows $T\subseteq[n]$, $|T|\leq s$, columns $r$-sets $B$, and entries $\mathbf1_{T\subseteq B}$. Over the [rational numbers](../../../../../rational-number.md), a row with $|T|=j$ equals $\binom{r-j}{s-j}^{-1}$ times the sum of the rows of all $s$-sets containing $T$. Thus its rational [matrix rank](../../../../../matrix-rank.md) is at most $\binom ns$. Every larger minor is an integer [determinant](../../../../../determinant.md) equal to zero and stays zero modulo $p$, so the same upper bound holds over $\mathbb F_p$. This proves the theorem.

For the forbidden midpoint problem, split $\mathcal A$ according to whether its members contain coordinate 1. Leave the containing half unchanged; complement every member of the avoiding half. Both resulting families consist of $2p$-sets containing 1, and complementation preserves their internal intersection sizes because

$$
|A^c\cap B^c|=4p-|A|-|B|+|A\cap B|=|A\cap B|.
$$

Within either transformed family, distinct intersections lie between 1 and $2p-1$ and are not $p$. Their residues are therefore in $L=\{1,\ldots,p-1\}$, whereas the set-size residue is $2p\equiv0$. Apply the [Frankl-Wilson theorem](../../../../../frankl-wilson-theorem.md) to each half and add:

$$
\boxed{|\mathcal A|\leq2\binom{4p}{p-1}}.
$$

**The factor 2 comes from splitting into two families.** The unsplit family can contain disjoint sets, whose intersection residue zero equals the set-size residue and prevents this direct application. Removing the shared coordinate after splitting also gives the stronger [complement splitting for forbidden midpoint intersections](../../../../../complement-splitting-for-forbidden-midpoint-intersections.md) bound $2\binom{4p-1}{p-1}$.

For the construction, fix a $(p+1)$-set $B$ and let $R=[4p]\setminus B$, of size $3p-1$. The [fixed-core construction avoiding midpoint intersections](../../../../../fixed-core-construction-avoiding-midpoint-intersections.md) is

$$
\mathcal F=\{B\cup X:X\in R^{(p-1)}\},\qquad
\mathcal A=\mathcal F\cup\{A^c:A\in\mathcal F\}.
$$

Two members of $\mathcal F$ intersect in at least $p+1$ points; the same is true for two complements. An intersection across the two halves has size $|X\setminus Y|\leq p-1$. No intersection is $p$. The halves are disjoint because one contains all of $B$ and the other none, so

$$
\boxed{|\mathcal A|=2\binom{3p-1}{p-1}}.
$$

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 10](../../paper-10-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
