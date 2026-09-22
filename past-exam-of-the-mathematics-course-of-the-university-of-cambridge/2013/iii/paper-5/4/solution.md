<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

For a decreasing integer tuple $\lambda=(\lambda_1,\ldots,\lambda_m)$, let $\mu_i=\lambda_i-\lambda_m$. Then $\mu$ is a partition and the [highest-weight classification of rational GL representations](../../../../../highest-weight-classification-of-rational-gl-representations.md) defines

$$
D_\lambda(V)=(\det V)^{\lambda_m}\otimes D_\mu(V).
$$

This is a [determinant twist](../../../../../determinant-twist.md) of a [Schur module](../../../../../schur-module.md). Every irreducible rational $GL_m$ representation becomes [polynomial](../../../../../polynomial-split.md) after multiplication by a sufficiently large positive [determinant](../../../../../determinant.md) power, which clears all matrix-entry denominators. The [polynomial](../../../../../polynomial-split.md) degree decomposition and [Schur–Weyl duality](../../../../../schur-weyl-duality.md) then identify it with a Schur [module](../../../../../module-mathematics.md). Undoing the twist gives exactly one decreasing integer tuple $\lambda$. Distinct tuples have distinct highest torus weights, so these are the complete pairwise nonisomorphic irreducible [rational representations](../../../../../rational-representation.md).

The [Weyl character formula](../../../../../weyl-character-formula.md) specializes to

$$
\varphi_\lambda(\operatorname{diag}(x_1,\ldots,x_m))=
\frac{\det(x_j^{\lambda_i+m-i})}{\det(x_j^{m-i})}
=(x_1\cdots x_m)^{\lambda_m}s_\mu(x).
$$

It is a symmetric [Laurent polynomial](../../../../../laurent-polynomial.md) in the [eigenvalues](../../../../../eigenvalue.md). Equality extends from the dense set of [diagonalizable](../../../../../diagonalizable-matrix.md) matrices to all invertible matrices: both the [character](../../../../../character-of-a-representation.md) and the expression in the characteristic-polynomial coefficients are [regular functions](../../../../../regular-function.md) on $GL_m$. For a [polynomial representation](../../../../../polynomial-representation-of-the-general-linear-group.md) this also extends to every endomorphism of $V$. **For a general [rational representation](../../../../../rational-representation.md), the printed claim at singular endomorphisms needs this qualification**: for example $\det^{-1}$ is undefined at a singular matrix. The displayed formula is valid on $GL_m$, and on all of $\operatorname{End}(V)$ when $\lambda_m\ge0$.

To compute the degree, set $x_j=e^{tc_j}$ with distinct $c_j$ and take $t\to0$. For $\ell_i=\lambda_i+m-i$ and $d=\binom m2$, the [leading coefficient of an exponential alternant](../../../../../leading-coefficient-of-an-exponential-alternant.md) is

$$
\det(e^{t\ell_i c_j})=
\frac{t^d}{\prod_{k=0}^{m-1}k!}\prod_{i<j}(\ell_i-\ell_j)\prod_{i<j}(c_i-c_j)+O(t^{d+1}).
$$

Indeed, expand every exponential in powers of $t$. The first nonzero [determinant](../../../../../determinant.md) uses the distinct powers $0,1,\ldots,m-1$; its coefficient is the product of the two [Vandermonde determinants](../../../../../vandermonde-determinant.md) divided by $\prod k!$. Taking the same expansion in the denominator cancels the powers and the $c$ factors, giving the [Weyl dimension formula](../../../../../weyl-dimension-formula.md)

$$
\boxed{\deg\varphi_\lambda=\dim D_\lambda(V)=\prod_{i<j}\frac{\lambda_i-\lambda_j+j-i}{j-i}.}
$$

This proof works for negative $\lambda_m$ as well, since [determinant](../../../../../determinant.md) twists have dimension one.

Every finite-dimensional rational [module](../../../../../module-mathematics.md) is completely reducible. The [characters](../../../../../character-of-a-representation.md) of its irreducible constituents are linearly independent: each Schur Laurent [character](../../../../../character-of-a-representation.md) has its highest dominant monomial $x^\lambda$ with coefficient $1$, and only lower weights besides it. In a finite relation, choose a lexicographically highest remaining weight; its coefficient must vanish, and iterate. Therefore equal [characters](../../../../../character-of-a-representation.md) give equal multiplicities of every irreducible constituent, proving **rational [modules](../../../../../module-mathematics.md) with the same [character](../../../../../character-of-a-representation.md) are isomorphic**.

Finally the [symmetric algebra](../../../../../symmetric-algebra.md) of $V\oplus\Lambda^2V$ has the formal torus [character](../../../../../character-of-a-representation.md)

$$
\operatorname{ch}\!\left(\bigoplus_{j\ge0}S^j(V\oplus\Lambda^2V)\right)
=\prod_i(1-x_i)^{-1}\prod_{i<j}(1-x_ix_j)^{-1}.
$$

Each factor sums the symmetric powers of a one-dimensional weight space; the [exterior square](../../../../../exterior-square.md) has weights $x_ix_j$ for $i<j$. The permitted Schur identity makes this $\sum_\lambda s_\lambda(x)$. In each fixed scalar degree there are only finitely many terms, so complete reducibility and [character](../../../../../character-of-a-representation.md) independence apply degree by degree without a convergence assumption. Thus the [multiplicity-free symmetric-algebra model for polynomial GL representations](../../../../../multiplicity-free-symmetric-algebra-model-for-polynomial-gl-representations.md) contains **each irreducible [polynomial representation](../../../../../polynomial-representation-of-the-general-linear-group.md) exactly once**. The word irreducible is necessary: arbitrary reducible [polynomial](../../../../../polynomial-split.md) [modules](../../../../../module-mathematics.md), such as two copies of the trivial [module](../../../../../module-mathematics.md), do not each occur once in a multiplicity-free sum.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 5](../../paper-5-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
