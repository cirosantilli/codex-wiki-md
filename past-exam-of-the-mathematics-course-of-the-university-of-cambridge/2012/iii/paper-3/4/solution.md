<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

For a partition $\nu$ with at most $m$ parts, let $D_\nu(V)$ be the [Schur module](../../../../../schur-module.md) constructed in Question 3, equivalently the image of a [Young symmetrizer](../../../../../young-symmetrizer.md) on $V^{\otimes|\nu|}$. For a weakly decreasing integer tuple $\lambda$, put $k=\max(0,-\lambda_m)$ and $\nu=\lambda+k(1,\ldots,1)$. Define the [rational Schur module](../../../../../rational-schur-module.md) by

$$
\boxed{D_\lambda(V)=\det^{-k}\otimes D_\nu(V).}
$$

Here $\det^{-k}$ is the one-dimensional representation $g\mapsto\det(g)^{-k}$. This is rational, and it is irreducible under the permitted irreducibility assumption; for nonnegative $\lambda$ it is the original [polynomial](../../../../../polynomial-split.md) [Schur module](../../../../../schur-module.md). Larger shifts give the same module, as will also follow from the [character](../../../../../character-of-a-representation.md) formula below.

Write $s_r(x)=\sum_{i=1}^m x_i^r$ and $p_\alpha(x)=\prod_{r=1}^n s_r(x)^{\alpha_r}$. For a [permutation](../../../../../permutation.md) $\sigma$ of the given cycle type, the [trace of a permuted tensor power](../../../../../trace-of-a-permuted-tensor-power.md) is

$$
\operatorname{tr}_T(\sigma\xi^{\otimes n})
=\prod_{r=1}^n\operatorname{tr}(\xi^r)^{\alpha_r}=p_\alpha(x).
$$

In a tensor basis, the trace contracts the matrix entries of $\xi$ around each cycle of $\sigma$; a cycle of length $r$ contributes $\operatorname{tr}(\xi^r)$. This proof applies to nondiagonalizable [endomorphisms](../../../../../endomorphism.md) as well. The [eigenvalues](../../../../../eigenvalue.md) give $\operatorname{tr}(\xi^r)=s_r(x)$.

The [Schur–Weyl duality](../../../../../schur-weyl-duality.md) decomposition, on which $\sigma$ and $\xi^{\otimes n}$ act on the two respective factors, gives the same trace as

$$
\boxed{p_\alpha(x)=\sum_{\substack{\lambda\vdash n\\\ell(\lambda)\leq m}}
\chi^\lambda(\alpha)\phi_\lambda(\xi).}
$$

For a partition, the [character](../../../../../character-of-a-representation.md) extends polynomially to all [endomorphisms](../../../../../endomorphism.md) because the tensor-power action does. This extension is not asserted for determinant-twisted modules at singular matrices.

We now derive the [alternant character formula for the general linear group](../../../../../alternant-character-formula-for-the-general-linear-group.md). Put $\delta=(m-1,m-2,\ldots,0)$ and

$$
a_\beta(x)=\det(x_i^{\beta_j})_{1\leq i,j\leq m},\qquad
a_\delta(x)=\prod_{i<j}(x_i-x_j).
$$

Use the permitted symmetric-group [character](../../../../../character-of-a-representation.md) result, the [Frobenius alternant character formula](../../../../../frobenius-alternant-character-formula.md):

$$
\chi^\lambda(\alpha)=[x^{\lambda+\delta}]\bigl(a_\delta(x)p_\alpha(x)\bigr).
$$

It concerns [characters](../../../../../character-of-a-representation.md) of $S_n$, rather than assuming the [character](../../../../../character-of-a-representation.md) formula we seek for the general linear group. Substitute the proved trace identity and set

$$
c_{\lambda\mu}=[x^{\lambda+\delta}]\bigl(a_\delta\phi_\mu\bigr).
$$

Then $\chi^\lambda(\alpha)=\sum_\mu c_{\lambda\mu}\chi^\mu(\alpha)$ for every [conjugacy class](../../../../../conjugacy-class.md). Independence of the irreducible symmetric-group [characters](../../../../../character-of-a-representation.md) forces $c_{\lambda\mu}=\delta_{\lambda\mu}$.

Each [character](../../../../../character-of-a-representation.md) $\phi_\mu$ on diagonal matrices is a symmetric homogeneous [polynomial](../../../../../polynomial-split.md) of degree $n$, since conjugation by [permutation](../../../../../permutation.md) matrices permutes its arguments. Thus $a_\delta\phi_\mu$ is alternating of degree $n+\binom m2$. Every [alternating polynomial](../../../../../alternating-polynomial.md) of this degree has a unique expansion in alternants $a_{\lambda+\delta}$: a [monomial](../../../../../monomial.md) with repeated exponents has zero coefficient, while each strictly decreasing nonnegative exponent vector is uniquely $\lambda+\delta$ for a partition $\lambda$ of $n$ with at most $m$ parts. Its coefficient at $x^{\lambda+\delta}$ is the coefficient of that alternant. The identities for $c_{\lambda\mu}$ therefore give $a_\delta\phi_\mu=a_{\mu+\delta}$. We have derived the [Weyl character formula](../../../../../weyl-character-formula.md)

$$
\boxed{\phi_\lambda(\operatorname{diag}(x_1,\ldots,x_m))
=\frac{\det(x_i^{\lambda_j+m-j})}{\det(x_i^{m-j})}.}
$$

For partitions the quotient is the [Schur polynomial](../../../../../schur-polynomial.md), with removable apparent singularities when [eigenvalues](../../../../../eigenvalue.md) coincide. For arbitrary dominant integer tuples, multiply the formula for $\nu$ by $(x_1\cdots x_m)^{-k}$; this shifts every numerator exponent by $-k$ and yields the same boxed formula. The variables must then be nonzero. The expression also shows independence of the shift used to define the [determinant twist](../../../../../determinant-twist.md). Equality of [characters](../../../../../character-of-a-representation.md) identifies these [irreducible modules](../../../../../irreducible-module.md): the group-algebra image on a [direct sum](../../../../../direct-sum.md) of two irreducibles is finite-dimensional and semisimple, and its span of group operators detects the traces on every simple block.

Finally, the [character](../../../../../character-of-a-representation.md) of a [dual representation](../../../../../dual-representation.md) evaluates the original [character](../../../../../character-of-a-representation.md) at $x_i^{-1}$. Reverse the numerator's columns after making this substitution. The exponents become $-\lambda_{m+1-j}+1-j$. Factoring $(x_1\cdots x_m)^{-(m-1)}$ converts these into $\mu_j+m-j$ for $\mu_j=-\lambda_{m+1-j}$. The denominator undergoes the identical column reversal and factor, so both signs and factors cancel. Hence $\phi_\lambda(x^{-1})=\phi_\mu(x)$, and

$$
\boxed{D_\lambda(V)^*\cong D_{(-\lambda_m,-\lambda_{m-1},\ldots,-\lambda_1)}(V).}
$$

This tuple is again weakly decreasing, so it is precisely the required dominant label.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 3](../../paper-3-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
