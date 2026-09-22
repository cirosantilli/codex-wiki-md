<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The general modular form, the **[nonuniform Frankl-Wilson theorem](../../../../../nonuniform-frankl-wilson-theorem.md)**, can be stated as follows. Let $p$ be a [prime number](../../../../../prime-number.md), and let $L\subseteq\mathbb F_p$ have $s$ elements. Suppose $\mathcal F\subseteq\mathcal P([n])$ has $|A|\bmod p\notin L$ for every member, while $|A\cap B|\bmod p\in L$ for any distinct members. Then

$$
\boxed{|\mathcal F|\leq\sum_{j=0}^{\min(s,n)}\binom nj}.
$$

The uniform [Frankl-Wilson theorem](../../../../../frankl-wilson-theorem.md) sharpens this to $|\mathcal F|\leq\binom ns$ when all members have size $k$ and $0\leq s\leq\min\{k,n-k\}$. Both forms require a prime modulus and exclusion of the self-intersection residue.

For the general proof, work over the [finite field](../../../../../finite-field.md) $\mathbb F_p$. Associate to each member $A$ the [intersection polynomial](../../../../../intersection-polynomial.md)

$$
f_A(x)=\prod_{\ell\in L}\left(\sum_{i\in A}x_i-\ell\right).
$$

At the [characteristic vectors of sets](../../../../../characteristic-vector-of-a-set.md) $\mathbf1_B$, this is zero if $B\ne A$, and nonzero if $B=A$. Thus these [polynomials](../../../../../polynomial-split.md), regarded as functions on the [Boolean hypercube](../../../../../boolean-hypercube.md), are [linearly independent](../../../../../linear-independence.md): evaluating any relation at $\mathbf1_A$ isolates its coefficient. Apply [multilinear reduction on the Boolean cube](../../../../../multilinear-reduction-on-the-boolean-cube.md), replacing every positive power of a variable by that variable. Values on the [Boolean hypercube](../../../../../boolean-hypercube.md) remain unchanged, and the resulting [multilinear polynomials](../../../../../multilinear-polynomial.md) have degree at most $s$. Their ambient space has a [monomial basis](../../../../../monomial-basis.md) consisting of $x_S=\prod_{i\in S}x_i$ for $|S|\leq s$, with dimension $\sum_{j=0}^{\min(s,n)}\binom nj$. This proves the general bound, including $s=0$.

For completeness, obtain the uniform sharpening without dividing by factorials in a [finite field](../../../../../finite-field.md). For $s\geq1$ put $a=k\bmod p$ and $g(x)=\sum_i x_i-a$. The functions $x_Sg$ with $|S|<s$ are [linearly independent](../../../../../linear-independence.md). Indeed, a relation gives $gh=0$ with $\deg h<s$, so $h$ is supported only on weights in $H=\{j\in[0,n]:j\equiv a\pmod p\}$. With boundary weights $-1,n+1$, this set has a gap of at least $s+1$: either consecutive allowed weights differ by $p\geq s+1$, or its terminal gap does, since $n\geq k+s\geq a+s$. The alternating sum of $h$ over any interval of $s$ free coordinates vanishes by its degree. Across that gap only one endpoint level can contribute, forcing $h$ to vanish there. Delete that level and repeat across the enlarged gap until $H$ is empty. Hence $h=0$, and independence of the square-free [monomials](../../../../../monomial.md) gives the claim. Adjoin these functions to the $f_A$. Evaluation at each family vector eliminates the coefficients of $f_A$, since $g$ vanishes there; the claim eliminates all remaining coefficients. Counting dimensions yields

$$
|\mathcal F|+\sum_{j=0}^{s-1}\binom nj\leq\sum_{j=0}^s\binom nj,\qquad\boxed{|\mathcal F|\leq\binom ns}.
$$

The case $s=0$ permits at most one member directly. The gap argument is an instance of the [modular layer vanishing lemma](../../../../../modular-layer-vanishing-lemma.md).

For the final application, enumerate the distinct sets as $A_1,\ldots,A_m$ and let $v_i=\mathbf1_{A_i}\in\mathbb R^n$ be their [characteristic vectors of sets](../../../../../characteristic-vector-of-a-set.md). If $m\leq1$, the desired bound is immediate for $n\geq1$. Otherwise $|A_i|\geq k$, because $A_i$ intersects another member in $k$ points. At most one member can have size $k$: two distinct $k$-sets cannot have intersection size $k$. The [Gram matrix](../../../../../gram-matrix.md) of these vectors is

$$
G=k\mathbf1\mathbf1^{\mathsf T}+\operatorname{diag}(|A_1|-k,\ldots,|A_m|-k).
$$

For real coefficients $c_i$,

$$
\left\|\sum_i c_iv_i\right\|^2=c^{\mathsf T}Gc=k\left(\sum_i c_i\right)^2+\sum_i(|A_i|-k)c_i^2.
$$

All terms are nonnegative, with $k>0$. If the expression vanishes, every coefficient corresponding to a set of size greater than $k$ is zero. At most one coefficient remains, and the first term forces it to be zero as well. Thus the [characteristic vectors of sets](../../../../../characteristic-vector-of-a-set.md) are [linearly independent](../../../../../linear-independence.md) in $\mathbb R^n$, proving the **[constant-intersection family bound](../../../../../constant-intersection-family-bound.md)**

$$
\boxed{m\leq n}.
$$

This proof explicitly covers the possible member of size exactly $k$; assuming all diagonal corrections were strictly positive would miss that case. Positivity of $k$ is essential: when $k=0$, the empty set and all $n$ singleton sets give $n+1$ members.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 10](../../paper-10-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
