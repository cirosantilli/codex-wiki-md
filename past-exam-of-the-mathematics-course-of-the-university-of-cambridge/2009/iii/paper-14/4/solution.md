<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The [Frankl-Wilson theorem](../../../../../frankl-wilson-theorem.md) in its uniform form says: let $p$ be a [prime number](../../../../../prime-number.md), let $L\subseteq\mathbb F_p$ have size $s\leq\min(k,n-k)$, and let $\mathcal F\subseteq\binom{[n]}k$ have $k\bmod p\notin L$, while $|A\cap B|\bmod p\in L$ for every distinct pair of members. Then

$$
\boxed{|\mathcal F|\leq\binom ns.}
$$

The modular-intersection, nonuniform form of the [Frankl-Wilson theorem](../../../../../frankl-wilson-theorem.md) is as follows. Let $p$ be a [prime number](../../../../../prime-number.md), let $L\subseteq\mathbb F_p$ have $s$ elements, and let $\mathcal F\subseteq\mathcal P([n])$ satisfy $|A|\bmod p\notin L$ for each $A\in\mathcal F$, whereas $|A\cap B|\bmod p\in L$ for distinct $A,B\in\mathcal F$. Then

$$
\boxed{|\mathcal F|\leq\sum_{j=0}^{\min(s,n)}\binom nj.}
$$

This [nonuniform Frankl-Wilson theorem](../../../../../nonuniform-frankl-wilson-theorem.md) allows different sizes and different diagonal residues; in particular it applies when all sizes have one common residue outside $L$.

To prove it by the [polynomial method in combinatorics](../../../../../polynomial-method-in-combinatorics.md), work over the [finite field](../../../../../finite-field.md) $\mathbb F_p$ and associate to each member the [intersection polynomial](../../../../../intersection-polynomial.md)

$$
P_A(x_1,\ldots,x_n)=\prod_{\ell\in L}\left(\sum_{i\in A}x_i-\ell\right).
$$

Replace each positive power of $x_i$ in its expansion by $x_i$ to obtain its [multilinear reduction on the Boolean cube](../../../../../multilinear-reduction-on-the-boolean-cube.md) $\widetilde P_A$. This preserves evaluation on every [characteristic vector](../../../../../characteristic-vector-of-a-set.md), whose coordinates are zero or one, and leaves degree at most $s$. At the [characteristic vector](../../../../../characteristic-vector-of-a-set.md) $\mathbf1_B$,

$$
\widetilde P_A(\mathbf1_B)=\prod_{\ell\in L}(|A\cap B|-\ell).
$$

It is zero for distinct $A,B$, and nonzero for $B=A$ by the diagonal hypothesis. If $\sum_{A\in\mathcal F}c_A\widetilde P_A=0$, evaluating at each $\mathbf1_B$ forces $c_B=0$. Thus the [multilinear polynomials](../../../../../multilinear-polynomial.md) are [linearly independent](../../../../../linear-independence.md). They belong to the [vector space](../../../../../vector-space-split.md) with [basis](../../../../../basis.md) the square-free [monomials](../../../../../monomial.md) $\prod_{i\in S}x_i$ for $|S|\leq s$, whose [dimension](../../../../../dimension-vector-space.md) is the displayed sum. This proves the nonuniform form, including $s=0$, where distinct members are impossible and the empty product is one.

For the sharp uniform form, we need the [low-degree evaluation rank on a uniform layer](../../../../../low-degree-evaluation-rank-on-a-uniform-layer.md). Form the integer [matrix](../../../../../matrix.md) $M$ whose rows are indexed by $S\subseteq[n]$ with $|S|\leq s$, columns by $k$-subsets $T$, and entries $M_{S,T}=\mathbf1_{S\subseteq T}$. These are evaluations of the square-free [monomials](../../../../../monomial.md). Over the [rational numbers](../../../../../rational-number.md), the row of a $j$-subset $S$ satisfies

$$
\sum_{\substack{R\supseteq S\\|R|=s}}M_{R,T}
=\binom{k-j}{s-j}M_{S,T}\qquad\text{for every }T.
$$

Indeed, when $S\subseteq T$ the left side counts the $s$-subsets between $S$ and $T$, and otherwise both sides vanish. Since $s\leq k$, the coefficient is a positive integer. Thus the degree-$s$ rows span all the rows over the [rational numbers](../../../../../rational-number.md), giving $\operatorname{rank}_{\mathbb Q}M\leq\binom ns$. Every square submatrix of larger size has integer [determinant](../../../../../determinant.md) zero, so its [determinant](../../../../../determinant.md) remains zero modulo $p$. Hence

$$
\operatorname{rank}_{\mathbb F_p}M\leq\operatorname{rank}_{\mathbb Q}M\leq\binom ns.
$$

This reduction of [matrix rank](../../../../../matrix-rank.md) is the reason one must not try to divide by $\binom{k-j}{s-j}$ directly in $\mathbb F_p$.

The evaluations of the $\widetilde P_A$ on the $k$th [uniform layer of the Boolean cube](../../../../../uniform-layer-of-the-boolean-cube.md) lie in the row [linear span](../../../../../linear-span.md) of $M$ over $\mathbb F_p$. They are [linearly independent](../../../../../linear-independence.md) as functions there, because restriction to the columns corresponding to $\mathcal F$ still gives the nonzero diagonal evaluation matrix. Their number is consequently at most $\binom ns$. This completes the proof of the uniform [Frankl-Wilson theorem](../../../../../frankl-wilson-theorem.md) as well.

For the odd-cardinality problem the sharper [Oddtown theorem](../../../../../oddtown-theorem.md) follows directly from [linear algebra](../../../../../linear-algebra-split.md). Let $v_A=\mathbf1_A\in\mathbb F_2^n$ be the [characteristic vector](../../../../../characteristic-vector-of-a-set.md). The parity conditions say

$$
v_A\cdot v_B=0\quad(A\ne B),\qquad v_A\cdot v_A=1.
$$

For any [linear combination](../../../../../linear-combination.md) $\sum_A c_Av_A=0$, take its [dot product](../../../../../dot-product.md) with $v_B$. All off-diagonal terms vanish, leaving $c_B=0$. Hence these vectors are [linearly independent](../../../../../linear-independence.md) in an $n$-dimensional [vector space](../../../../../vector-space-split.md), giving

$$
\boxed{|\mathcal A|\leq n.}
$$

The singleton [sets](../../../../../set-split.md) show that the bound can be attained. Notice why the constant term in the general [nonuniform Frankl-Wilson theorem](../../../../../nonuniform-frankl-wilson-theorem.md) is unnecessary here: these [dot products](../../../../../dot-product.md) already give a diagonal evaluation matrix using only the $n$ coordinate functions.

For even $n$, partition $[n]$ into the pairs $\{1,2\},\{3,4\},\ldots,\{n-1,n\}$ and take every union of a selection of these pairs. This gives exactly $2^{n/2}$ distinct [sets](../../../../../set-split.md), including the empty [set](../../../../../set-split.md). Each has even size; every pairwise [intersection](../../../../../set-intersection.md) is again a union of entire pairs and therefore has even size. **This attains the proposed bound.**

For any [set family](../../../../../set-family.md) satisfying the even-cardinality conditions, let $W$ be the [linear span](../../../../../linear-span.md) of its [characteristic vectors](../../../../../characteristic-vector-of-a-set.md) over $\mathbb F_2$. Now the self-[dot products](../../../../../dot-product.md) vanish as well as the off-diagonal ones. By [bilinearity](../../../../../bilinearity.md), $u\cdot v=0$ for all $u,v\in W$, so $W\subseteq W^\perp$: it is a [self-orthogonal binary subspace](../../../../../self-orthogonal-binary-subspace.md).

For completeness the standard [bilinear form](../../../../../bilinear-form.md) on $\mathbb F_2^n$ is [nondegenerate](../../../../../nondegenerate-bilinear-form.md), because a vector orthogonal to every coordinate vector has every coordinate zero. Thus the map $v\mapsto(w\mapsto v\cdot w)$ from $\mathbb F_2^n$ onto the [dual space](../../../../../dual-space.md) $W^*$ is surjective: every [linear functional](../../../../../linear-functional.md) on $W$ extends to the whole [vector space](../../../../../vector-space-split.md) by extending a [basis](../../../../../basis.md), and every such functional on $\mathbb F_2^n$ is a [dot product](../../../../../dot-product.md) with a vector. Its [kernel](../../../../../kernel-of-a-linear-map.md) is $W^\perp$. The [rank-nullity theorem](../../../../../rank-nullity-theorem.md) consequently gives $\dim W^\perp=n-\dim W$. The inclusion $W\subseteq W^\perp$ implies $\dim W\leq n/2$. Finally, distinct members have distinct [characteristic vectors](../../../../../characteristic-vector-of-a-set.md), all in $W$, and a $k$-dimensional [vector space](../../../../../vector-space-split.md) over $\mathbb F_2$ has exactly $2^k$ elements. Therefore

$$
\boxed{|\mathcal A|\leq|W|=2^{\dim W}\leq2^{n/2}.}
$$

This proves the [Eventown theorem](../../../../../eventown-theorem.md) and also explains the suggested [dimension](../../../../../dimension-vector-space.md) contradiction if the [set family](../../../../../set-family.md) had more than $2^{n/2}$ members.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 14](../../paper-14-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
