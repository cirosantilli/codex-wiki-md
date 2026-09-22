<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

**The [Frankl-Wilson theorem](../../../../../frankl-wilson-theorem.md).** Let $p$ be a [prime number](../../../../../prime-number.md), let $L\subseteq\mathbb F_p$ have $s$ elements, and let $\mathcal F\subseteq\mathcal P([n])$. Suppose that $|A|\bmod p\notin L$ for every $A\in\mathcal F$, whereas $|A\cap B|\bmod p\in L$ for all distinct members. Then

$$
\boxed{|\mathcal F|\leq\sum_{j=0}^{s}\binom nj,}
$$

with terms beyond $n$ understood as zero.

Work over the [finite field](../../../../../finite-field.md) $\mathbb F_p$. For each member define its [intersection polynomial](../../../../../intersection-polynomial.md)

$$
f_A(x_1,\ldots,x_n)=\prod_{\ell\in L}\left(\sum_{i\in A}x_i-\ell\right).
$$

Replace every positive power $x_i^d$ by $x_i$ to obtain a [multilinear polynomial](../../../../../multilinear-polynomial.md) $\widetilde f_A$ of [polynomial degree](../../../../../degree-of-a-polynomial.md) at most $s$. This [Boolean multilinearization](../../../../../boolean-multilinearization.md) preserves its values at every [characteristic vector of a set](../../../../../characteristic-vector-of-a-set.md). At the [characteristic vector of a set](../../../../../characteristic-vector-of-a-set.md) $B$,

$$
\widetilde f_A(\mathbf1_B)=\prod_{\ell\in L}(|A\cap B|-\ell).
$$

It is zero if $A\ne B$ and nonzero if $A=B$. Evaluating a proposed linear relation at each $\mathbf1_B$ therefore establishes [linear independence](../../../../../linear-independence.md) of the $\widetilde f_A$. The [vector space](../../../../../vector-space-split.md) of [multilinear polynomials](../../../../../multilinear-polynomial.md) of [polynomial degree](../../../../../degree-of-a-polynomial.md) at most $s$ has the [basis](../../../../../basis.md) of [monomials](../../../../../monomial.md) $\prod_{i\in T}x_i$, $|T|\leq s$, of size $\sum_{j=0}^{s}\binom nj$. This proves the [Frankl-Wilson theorem](../../../../../frankl-wilson-theorem.md) by the [polynomial method in combinatorics](../../../../../polynomial-method-in-combinatorics.md). The empty product for $s=0$ is $1$, and the argument still applies.

**The [constant-intersection family bound](../../../../../constant-intersection-family-bound.md), directly.** Write $\mathcal F=\{F_1,\ldots,F_q\}$ and assume $n\geq1$. The cases $q\leq1$ are immediate. If $\lambda=0$, the nonempty members are pairwise disjoint and there can also be the empty set, giving

$$
\boxed{q\leq n+1.}
$$

For $\lambda>0$, every member has size at least $\lambda$. If every member has size strictly greater than $\lambda$, form the real [matrix](../../../../../matrix.md) $X$ whose rows are their [characteristic vectors of sets](../../../../../characteristic-vector-of-a-set.md). Its [Gram matrix](../../../../../gram-matrix.md) satisfies

$$
XX^{\mathsf T}=\operatorname{diag}(|F_1|-\lambda,\ldots,|F_q|-\lambda)+\lambda\mathbf1\mathbf1^{\mathsf T}.
$$

For any nonzero real [vector](../../../../../vector.md) $z$,

$$
z^{\mathsf T}XX^{\mathsf T}z
=\sum_i(|F_i|-\lambda)z_i^2+\lambda\left(\sum_i z_i\right)^2>0.
$$

Thus the rows are [linearly independent](../../../../../linear-independence.md) and $q\leq n$. If a member $F_1$ has size $\lambda$, it lies inside every other member. The sets $F_i\setminus F_1$, $i>1$, are nonempty and pairwise disjoint, so $q-1\leq n-\lambda$. This also gives

$$
\boxed{q\leq n\quad(\lambda>0).}
$$

These bounds are sharp: the singletons together with $\varnothing$ attain $n+1$ at $\lambda=0$, while all complements of singletons attain $n$ at $\lambda=n-2>0$ when $n\geq3$.

**The [constant t-wise intersection dichotomy](../../../../../constant-t-wise-intersection-dichotomy.md).** In its substantive form the last argument requires $m\geq t$. The printed statement does not explicitly impose this. Without it the $t$-fold condition can be vacuous and the claimed dichotomy is false: take $t=3$, $m=2$, $n=1$, $A_1=\varnothing$, $A_2=\{1\}$ and $\lambda=1$. There is no $3$-tuple to test, no common $1$-set, and $k=0$, so $m=2>k+t-2=1$. We therefore prove the intended assertion for $m\geq t$ and record this necessary qualification.

If $\lambda=0$, the first alternative always holds with $S=\varnothing$. Suppose $\lambda>0$. Choose $t-2$ indices attaining the minimum intersection size $k$, and write

$$
K=\bigcap_{i\in I}A_i,\qquad |I|=t-2,\quad |K|=k.
$$

For each of the $q=m-t+2\geq2$ remaining indices put $B_j=K\cap A_j$. The hypothesis gives $|B_j\cap B_\ell|=\lambda$ for distinct remaining indices. This reduces the [constant t-wise intersection dichotomy](../../../../../constant-t-wise-intersection-dichotomy.md) to a [constant-intersection family bound](../../../../../constant-intersection-family-bound.md) on the $k$-element set $K$. The two possibilities are treated below.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 11](../../paper-11-split.md)
3. [Iii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
