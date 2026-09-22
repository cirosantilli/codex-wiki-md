<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Write the diagonal [maximal torus](../../../../../maximal-torus.md) of $U(n)$ as $t=\operatorname{diag}(z_1,\ldots,z_n)$, $|z_i|=1$, and let $\delta=(n-1,n-2,\ldots,0)$. Irreducible complex representations are indexed by dominant integer tuples $\lambda_1\geq\cdots\geq\lambda_n$, their [highest weights](../../../../../highest-weight-of-a-representation.md). The [Weyl character formula](../../../../../weyl-character-formula.md) in integer-exponent form is

$$
\boxed{\chi_\lambda(t)
=\frac{\det(z_i^{\lambda_j+n-j})_{i,j=1}^n}
{\det(z_i^{n-j})_{i,j=1}^n}.}
$$

The ratio initially uses distinct $z_i$, and extends to repeated eigenvalues by continuity. Every unitary matrix is conjugate to such a diagonal matrix, so this determines the [character](../../../../../character-of-a-representation.md) on the entire group. The shift $\delta$ differs from the usual [Weyl vector](../../../../../half-sum-of-positive-roots.md) $\rho=((n-1)/2,(n-3)/2,\ldots,(1-n)/2)$ by a multiple of $(1,\ldots,1)$; the corresponding determinant factors cancel between numerator and denominator.

We first justify the highest-weight information needed in the proof. Restriction to the torus splits a representation into integer [weight spaces](../../../../../weight-space.md). In an irreducible representation choose a lexicographically largest weight $\lambda$ and a nonzero vector $v$ of that weight. A matrix unit $E_{ij}$ with $i<j$ raises the weight by $e_i-e_j$, so it annihilates $v$. The character is invariant under permutations of diagonal coordinates, because permutation matrices conjugate the torus. Hence permutations of $\lambda$ are also weights, and lexical maximality forces $\lambda_1\geq\cdots\geq\lambda_n$.

Irreducibility implies that $v$ generates the representation under the complexified [Lie algebra](../../../../../lie-algebra-split.md). Indeed, a Lie-algebra invariant subspace is preserved by exponentials of skew-Hermitian matrices, which generate $U(n)$. Reorder any product of matrix units into lower-triangular units, diagonal units and upper-triangular units, using

$$
[E_{ij},E_{kl}]=\delta_{jk}E_{il}-\delta_{li}E_{kj}.
$$

Induction on length and on the number of out-of-order pairs gives the required spanning version of the [Poincaré-Birkhoff-Witt theorem](../../../../../poincare-birkhoff-witt-theorem.md). Upper-triangular units kill $v$, and diagonal units act by scalars. Every nonempty product of lower-triangular units lowers its weight by a nonzero sum of positive roots. Therefore the top weight space is exactly $\mathbb Cv$, and its multiplicity is one. This supplies the leading coefficient without assuming a character formula.

For completeness, every dominant integer tuple occurs. Put $d_j=\lambda_j-\lambda_{j+1}\geq0$ and form the representation

$$
(\det)^{\lambda_n}\otimes
\bigotimes_{j=1}^{n-1}(\Lambda^j\mathbb C^n)^{\otimes d_j}.
$$

Its lexicographically highest weight is $\lambda$, with one-dimensional highest space, represented by the tensor products of $e_1\wedge\cdots\wedge e_j$. A negative determinant exponent is a legitimate one-dimensional unitary-group character. Averaging an [inner product](../../../../../inner-product.md) over normalized [Haar measure](../../../../../haar-measure.md) gives invariant orthogonal complements, so the tensor representation splits into irreducible summands. One of them has highest weight $\lambda$. Uniqueness will also follow from the formula and [Schur orthogonality relations](../../../../../schur-orthogonality-relations.md).

Define the alternant $A_\kappa(z)=\det(z_i^{\kappa_j})$ for a strictly decreasing integer tuple $\kappa$. The denominator

$$
A_\delta(z)=\prod_{i<j}(z_i-z_j)
$$

is the [Vandermonde determinant](../../../../../vandermonde-determinant.md), and its modulus is the denominator modulus in the [Weyl integration formula](../../../../../weyl-integration-formula.md). The [Laurent polynomial](../../../../../laurent-polynomial.md) $\chi_\lambda A_\delta$ is alternating. Any alternating Laurent polynomial decomposes as a finite sum

$$
\chi_\lambda A_\delta=\sum_\kappa c_\kappa A_\kappa:
$$

monomials with repeated exponents have zero coefficient, and the remaining permutation orbits are indexed uniquely by strictly decreasing tuples.

The lexicographically highest monomial in the product is $z^{\lambda+\delta}$ with coefficient one. Indeed, the highest monomial of the character is $z^\lambda$ with coefficient one, and the unique lexical maximum among permutations of $\delta$ is $\delta$ itself. It follows that $c_{\lambda+\delta}=1$.

[Fourier orthogonality](../../../../../fourier-orthogonality.md) on the torus, whose probability measure is $\prod_i d\theta_i/(2\pi)$, gives [alternant orthogonality on a unitary torus](../../../../../alternant-orthogonality-on-a-unitary-torus.md):

$$
\int_T A_\kappa\overline{A_\eta}\,dt
=n!\,\delta_{\kappa\eta}.
$$

Expand both determinants: an integral survives exactly when the two exponent tuples are identical up to permutation. Strict decreasing order then forces $\kappa=\eta$, and its $n!$ matching terms each contribute one.

Finally, [Schur orthogonality relations](../../../../../schur-orthogonality-relations.md) give $\int_{U(n)}|\chi_\lambda|^2=1$. Applying the allowed [Weyl integration formula](../../../../../weyl-integration-formula.md) to this class function gives

$$
1=\frac1{n!}\int_T|\chi_\lambda A_\delta|^2\,dt
=\sum_\kappa|c_\kappa|^2.
$$

Since the coefficient $c_{\lambda+\delta}$ already equals one, every other coefficient vanishes. Thus $\chi_\lambda A_\delta=A_{\lambda+\delta}$, proving the formula. If two irreducible representations had the same highest weight, their characters would now coincide; the [Schur orthogonality relations](../../../../../schur-orthogonality-relations.md) imply that they are isomorphic. Apparent singularities at repeated diagonal eigenvalues are removable because the quotient equals the actual finite Laurent-polynomial character. No dimension formula has been assumed.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 18](../../paper-18-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
