<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

We prove both the general [modular intersection bound for a set family](../../../../../modular-intersection-bound-for-a-set-family.md) and its sharper uniform version, the [Frankl-Wilson theorem](../../../../../frankl-wilson-theorem.md). Let $p$ be [prime](../../../../../prime-number.md), let $L\subseteq\mathbb F_p$ have size $s$, and let $\mathcal F$ be a family of subsets of $[n]$. Suppose each member's [cardinality](../../../../../cardinality.md) modulo $p$ is outside $L$, whereas every intersection of two distinct members has [cardinality](../../../../../cardinality.md) modulo $p$ in $L$. Then **the general modular intersection bound is**

$$
\boxed{|\mathcal F|\leq\sum_{j=0}^s\binom nj,}
$$

with $\binom nj=0$ for $j>n$. If every member has the same size $k$ and $s\leq\min\{k,n-k\}$, the **uniform Frankl-Wilson theorem** sharpens this to

$$
\boxed{|\mathcal F|\leq\binom ns.}
$$

Here $k\bmod p\notin L$, so in particular $s<p$. Primality matters because the argument takes place over the [finite field](../../../../../finite-field.md) $\mathbb F_p$.

For each $A\in\mathcal F$, define the [polynomial](../../../../../polynomial-split.md)

$$
P_A(X_1,\ldots,X_n)=\prod_{\ell\in L}\left(\sum_{i\in A}X_i-\ell\right).
$$

At the [indicator vector](../../../../../indicator-vector.md) $\mathbf1_B$ of another member $B$, this [polynomial](../../../../../polynomial-split.md) is zero if $B\ne A$ and nonzero if $B=A$. Replace every positive power of $X_i$ by $X_i$ in its expanded [monomials](../../../../../monomial.md), obtaining a [multilinear polynomial](../../../../../multilinear-polynomial.md) $\widetilde P_A$ of degree at most $s$. This [multilinear reduction on the Boolean cube](../../../../../multilinear-reduction-on-the-boolean-cube.md) preserves values at every zero-one vector.

The resulting [polynomials](../../../../../polynomial-split.md) are [linearly independent](../../../../../linear-independence.md). Indeed, if $\sum_{A\in\mathcal F}c_A\widetilde P_A=0$, evaluating at $\mathbf1_B$ leaves $c_B\widetilde P_B(\mathbf1_B)=0$; the nonzero diagonal value forces $c_B=0$ for every $B$. But [multilinear polynomials](../../../../../multilinear-polynomial.md) of degree at most $s$ lie in the [vector space](../../../../../vector-space-split.md) with [basis](../../../../../basis.md) $\{\prod_{i\in S}X_i:|S|\leq s\}$, whose dimension is $\sum_{j=0}^s\binom nj$. The bound on the [dimension of a vector space](../../../../../dimension-vector-space.md) gives the general [modular intersection bound for a set family](../../../../../modular-intersection-bound-for-a-set-family.md). This is the [polynomial method in combinatorics](../../../../../polynomial-method-in-combinatorics.md): the intersection conditions produce an evaluation matrix with nonzero diagonal and zero off-diagonal entries.

To prove the sharper uniform bound, we first establish [injectivity of inclusion between adjacent set layers](../../../../../injectivity-of-inclusion-between-adjacent-set-layers.md). Over a [field](../../../../../field.md) with [field characteristic](../../../../../characteristic-of-a-field.md) zero or greater than $d+1$, suppose coefficients $c_S$, indexed by $d$-sets in $[n]$, satisfy

$$
\sum_{\substack{S\subset T\\|S|=d}}c_S=0\quad\text{for every }(d+1)\text{-set }T,\qquad n\geq2d+1.
$$

Then all coefficients are zero. For $d=0$ this is immediate. For $d\geq1$, fix distinct $i,j$ and subtract the equations for $U\cup\{i\}$ and $U\cup\{j\}$, where $U$ is a $d$-set avoiding $i,j$. The result is

$$
\sum_{\substack{S\subset U\\|S|=d-1}}(c_{S\cup\{i\}}-c_{S\cup\{j\}})=0.
$$

Apply [mathematical induction](../../../../../mathematical-induction.md) with degree $d-1$ on the $n-2$ remaining coordinates; its size condition holds because $n-2\geq2(d-1)+1$. This forces $c_{S\cup\{i\}}=c_{S\cup\{j\}}$ for every such $S$. Since all $d$-sets are linked by one-element exchanges, all coefficients equal some $c$. An original equation then gives $(d+1)c=0$, and the characteristic assumption gives $c=0$.

For every $S$ with $|S|\leq s-1$, now form the [multilinear polynomial](../../../../../multilinear-polynomial.md)

$$
G_S=\sum_{i\notin S}X_{S\cup\{i\}}+(|S|-k)X_S,\qquad X_S=\prod_{i\in S}X_i.
$$

This is the multilinear reduction of $X_S(\sum_iX_i-k)$, so it vanishes at every [indicator vector](../../../../../indicator-vector.md) of a $k$-set. These $G_S$ are [linearly independent](../../../../../linear-independence.md): in a nonzero linear relation choose the largest degree $d$ of a coefficient-bearing $S$. The degree-$(d+1)$ terms have coefficients $\sum_{S\subset T,\ |S|=d}c_S$. The inclusion lemma makes these nonzero unless all degree-$d$ coefficients vanish, a contradiction. It applies because $d\leq s-1$, $p>s$, and $n\geq2s$.

The $G_S$ are also independent jointly with the $\widetilde P_A$. Evaluating a relation at the [indicator vectors](../../../../../indicator-vector.md) of the family first forces every coefficient of $\widetilde P_A$ to vanish, since the $G_S$ vanish there; their own independence then kills the remaining coefficients. All these [polynomials](../../../../../polynomial-split.md) have degree at most $s$, so

$$
|\mathcal F|+\sum_{j=0}^{s-1}\binom nj\leq\sum_{j=0}^s\binom nj.
$$

Subtracting the lower-degree contribution proves the sharp [Frankl-Wilson theorem](../../../../../frankl-wilson-theorem.md). For $s=0$ the general bound already gives $|\mathcal F|\leq1=\binom n0$, so no auxiliary [polynomials](../../../../../polynomial-split.md) are needed.

For the even cross-intersection assertion, work instead in the [vector space over a finite field](../../../../../vector-space-over-a-finite-field.md) $\mathbb F_2^n$ and let

$$
U=\operatorname{span}\{\mathbf1_A:A\in\mathcal A\},\qquad V=\operatorname{span}\{\mathbf1_B:B\in\mathcal B\}.
$$

The parity assumption is exactly $\mathbf1_A\cdot\mathbf1_B=0$ in $\mathbb F_2$. By [bilinearity](../../../../../bilinearity.md), all vectors in $U$ are orthogonal to all vectors in $V$, giving $V\subseteq U^\perp$. The coordinate [dot product](../../../../../dot-product.md) is [nondegenerate](../../../../../nondegenerate-bilinear-form.md) over $\mathbb F_2$, so $\dim U^\perp=n-\dim U$. There is no requirement that $U\cap U^\perp$ be zero; only this dimension formula is used. Each distinct set has a distinct [indicator vector](../../../../../indicator-vector.md), and a dimension-$d$ binary [vector space](../../../../../vector-space-split.md) has $2^d$ elements. Therefore **the even cross-intersection bound is**

$$
\boxed{|\mathcal A|\,|\mathcal B|\leq2^{\dim U}\,2^{\dim V}\leq2^n.}
$$

This is the [even cross-intersection bound](../../../../../even-cross-intersection-bound.md), including empty families, for which the product is zero.

For odd intersections, append a final coordinate one to every [indicator vector](../../../../../indicator-vector.md):

$$
\widehat a=(\mathbf1_A,1),\qquad \widehat b=(\mathbf1_B,1)\quad\text{in }\mathbb F_2^{n+1}.
$$

Their [dot product](../../../../../dot-product.md) is $|A\cap B|+1=0$ in $\mathbb F_2$. Applying the same [orthogonal complement over the binary field](../../../../../orthogonal-complement-over-the-binary-field.md) argument to their spans, now in dimension $n+1$, gives **the required odd cross-intersection bound**:

$$
\boxed{|\mathcal A|\,|\mathcal B|\leq2^{n+1}.}
$$

Appending the coordinate preserves distinctness of the vectors, so the span-cardinality estimates remain valid. This proves the [odd cross-intersection bound](../../../../../odd-cross-intersection-bound.md) directly by reducing the odd condition to an even one in a larger [vector space](../../../../../vector-space-split.md).

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 109](../../paper-109-split.md)
3. [Iii](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
