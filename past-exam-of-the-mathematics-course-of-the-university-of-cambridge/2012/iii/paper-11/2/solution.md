<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Work over the [finite field](../../../../../finite-field.md) $\mathbb F_p$. For each [set family](../../../../../set-family.md) member form the [intersection polynomial](../../../../../intersection-polynomial.md)

$$
f_A(x_1,\ldots,x_n)=\prod_{i=1}^s\left(\sum_{a\in A}x_a-\ell_i\right).
$$

At the [characteristic vector of a set](../../../../../characteristic-vector-of-a-set.md) $B$, its value is $\prod_i(|A\cap B|-\ell_i)$. The given restrictions make $f_A(\chi_B)=0$ for $A\neq B$ and $f_A(\chi_A)\neq0$. Hence these functions are [linearly independent](../../../../../linear-independence.md): evaluate a purported relation at each [set family](../../../../../set-family.md) member to eliminate its coefficient.

Use [multilinear reduction on the Boolean cube](../../../../../multilinear-reduction-on-the-boolean-cube.md), replacing every positive power of $x_i$ by $x_i$. This preserves all evaluations on $\{0,1\}^n$ and cannot increase degree. The [multilinear polynomials](../../../../../multilinear-polynomial.md) of degree at most $s$ have basis $x_S=\prod_{i\in S}x_i$ for $|S|\leq s$. Their dimension is $\sum_{j=0}^{\min(s,n)}\binom nj$, and therefore

$$
\boxed{|\mathcal A|\leq\sum_{j=0}^s\binom nj},
$$

where $\binom nj=0$ for $j>n$. The proof also covers a list whose distinct integers have repeated residues: no assumption of distinct residues is needed for this first bound.

To obtain the sharper conclusion, suppose the common size residue $r$ avoids $0,\ldots,s-1$. If $s>n$, no set on this ground set can have the required residue, so the [set family](../../../../../set-family.md) is empty. Otherwise, add the [modular-size auxiliary polynomials](../../../../../modular-size-auxiliary-polynomials.md)

$$
q_S(x)=x_S\left(\sum_{i=1}^n x_i-r\right),\qquad |S|\leq s-1,
$$

again understood as functions after [multilinear reduction on the Boolean cube](../../../../../multilinear-reduction-on-the-boolean-cube.md). They have degree at most $s$, and all vanish on the [set family](../../../../../set-family.md)'s [characteristic vectors of sets](../../../../../characteristic-vector-of-a-set.md).

The $q_S$ are [linearly independent](../../../../../linear-independence.md). Indeed, evaluate $\sum_S c_Sq_S=0$ on $\chi_T$ with $|T|\leq s-1$:

$$
(|T|-r)\sum_{S\subseteq T}c_S=0.
$$

The first factor is nonzero in the [finite field](../../../../../finite-field.md). Starting with $T=\varnothing$ and proceeding in increasing [cardinality](../../../../../cardinality.md) shows $c_T=0$ for every such $T$.

Moreover, the combined list consisting of the $f_A$ and the $q_S$ is [linearly independent](../../../../../linear-independence.md). Evaluation at each $\chi_A$ first kills the coefficient of $f_A$; the preceding argument then kills all remaining coefficients. Comparing this list with the dimension of the degree-at-most-$s$ space yields

$$
|\mathcal A|+\sum_{j=0}^{s-1}\binom nj\leq\sum_{j=0}^s\binom nj,
\qquad \boxed{|\mathcal A|\leq\binom ns}.
$$

This is a nonuniform common-residue version of the [Frankl-Wilson theorem](../../../../../frankl-wilson-theorem.md); exact equality of all member sizes was never used.

**The exclusion of the small residues is necessary.** A concrete example with $s<n$ is $n=4$, $p=5$, $s=3$, the residue list $0,1,3$, and the [set family](../../../../../set-family.md) of all two-element subsets. Every member has size residue $r=2$, outside that list, while distinct members intersect in zero or one element. But

$$
|\mathcal A|=\binom42=6>\binom43=4.
$$

Here the omitted condition fails at $j=2$. Thus the example satisfies all the other hypotheses, rather than relying on a vacuous $s>n$ case.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 11](../../paper-11-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
