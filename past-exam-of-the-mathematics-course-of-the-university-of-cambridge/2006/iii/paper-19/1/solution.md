<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

For $G=U(n)$ take the diagonal [maximal torus](../../../../../maximal-torus.md)

$$
T=\{\operatorname{diag}(z_1,\ldots,z_n):|z_i|=1\}.
$$

The [spectral theorem](../../../../../spectral-theorem.md) for [unitary matrices](../../../../../unitary-matrix.md) says that every element is conjugate to an element of $T$. A diagonal element with pairwise distinct [eigenvalues](../../../../../eigenvalue.md) has centralizer exactly $T$. Its conjugates therefore determine its [eigenvalues](../../../../../eigenvalue.md) up to [permutation](../../../../../permutation.md), and the normalizer quotient is $W=N_G(T)/T\cong S_n$. The [character lattice of a torus](../../../../../character-lattice-of-a-torus.md) $T$ is $\mathbb Z^n$, with $e^\lambda(z)=z_1^{\lambda_1}\cdots z_n^{\lambda_n}$. [Conjugation](../../../../../conjugation.md) on the [matrix unit](../../../../../matrix-unit.md) $E_{ij}$ has [weight](../../../../../weight-representation-theory.md) $e_i-e_j$, so these are the [roots](../../../../../root-of-a-root-system.md). Choose $e_i-e_j$ positive for $i<j$; then

$$
\rho=\frac12(n-1,n-3,\ldots,1-n).
$$

[Dominant integral weights](../../../../../dominant-integral-weight.md) are precisely the integer tuples $\lambda_1\geq\cdots\geq\lambda_n$. Negative entries are allowed: they correspond to [determinant twists](../../../../../determinant-twist.md), so [polynomial representations](../../../../../polynomial-representation-of-the-general-linear-group.md) alone do not exhaust the [irreducible representations](../../../../../irreducible-representation.md) of $U(n)$.

Normalize [Haar measure](../../../../../haar-measure.md) on $G$ and $T$ to have mass one, and put

$$
\Delta(z)=\det(z_i^{n-j})_{i,j=1}^n=\prod_{i<j}(z_i-z_j).
$$

The [Weyl integration formula for U(n)](../../../../../weyl-integration-formula-for-u-n.md) for a [continuous](../../../../../continuous-function.md) [class function](../../../../../class-function.md) is

$$
\boxed{\int_{U(n)}f(g)\,dg
=\frac1{n!}\int_{[0,2\pi)^n} f(\operatorname{diag}(e^{i\theta_1},\ldots,e^{i\theta_n}))
\prod_{i<j}|e^{i\theta_i}-e^{i\theta_j}|^2
\prod_{i=1}^n\frac{d\theta_i}{2\pi}.}
$$

For a general [continuous function](../../../../../continuous-function.md), replace $f(t)$ in the [torus](../../../../../torus.md) integral by $\int_{G/T}f(gtg^{-1})\,d(gT)$, using the normalized invariant quotient measure.

To prove the formula, consider the [conjugation](../../../../../conjugation.md) map $q:G/T\times T\to G$, $q(gT,t)=gtg^{-1}$. On regular [torus](../../../../../torus.md) elements its fibres have exactly $n!$ points: the possible orderings of the distinct [eigenvalues](../../../../../eigenvalue.md). Equip the [group](../../../../../group-split.md) with an invariant [inner product](../../../../../inner-product.md) on its [Lie algebra](../../../../../lie-algebra-split.md) and split $\mathfrak u(n)=\mathfrak t\oplus\mathfrak t^\perp$. After translating the derivative back to the identity, its [torus](../../../../../torus.md) directions contribute the identity, while its transverse directions contribute $\operatorname{Ad}_{t^{-1}}-I$. Each pair $i<j$ supplies a real two-dimensional off-diagonal plane. On that plane $\operatorname{Ad}_t$ is multiplication by $z_i/z_j$, regarded as a plane rotation, so the absolute real [determinant](../../../../../determinant.md) of the transverse derivative is

$$
J(t)=\prod_{i<j}|z_i/z_j-1|^2=|\Delta(z)|^2.
$$

The change-of-variables theorem, divided by the covering multiplicity, now gives the desired weighted integral up to the constant relating the normalized [invariant measures](../../../../../invariant-measure.md). The nonregular locus has measure zero: repeated [eigenvalues](../../../../../eigenvalue.md) are the zero-set of the nonzero discriminant, and the [torus](../../../../../torus.md) coincidence sets likewise have measure zero. Thus its omission causes no change to the integral. To determine the normalization, expand $\Delta$ as a sum of $n!$ distinct [torus characters](../../../../../characters-of-a-real-torus.md). [Fourier orthogonality](../../../../../fourier-orthogonality.md) gives $\int_T|\Delta|^2\,dt=n!$. Applying the formula to $f=1$ fixes the coefficient to $1/n!$. This proves both the class-function and conjugacy-averaged forms.

We can now derive the [character](../../../../../character-of-a-representation.md) formula from integration, rather than merely quote it. Use the basic highest-weight theorem: a finite-dimensional [irreducible representation](../../../../../irreducible-representation.md) has a unique [highest weight](../../../../../highest-weight-of-a-representation.md) $\lambda$ with a one-dimensional highest-weight space; all its other [weights](../../../../../weight-representation-theory.md) are $\lambda$ minus a nonnegative sum of [positive roots](../../../../../positive-root.md). Its [character](../../../../../character-of-a-representation.md) is Weyl invariant. Also, [character orthogonality for compact groups](../../../../../character-orthogonality-for-compact-groups.md) gives $\int_G|\chi_\lambda|^2=1$. This [orthogonality](../../../../../orthogonal-vectors.md) follows by averaging the [representation](../../../../../group-representation.md) on $\operatorname{End}(V_\lambda)$: the integral projects onto [intertwining operators](../../../../../intertwining-operator.md), whose [dimension](../../../../../dimension-vector-space.md) is one by the [Schur lemma](../../../../../schur-s-lemma.md).

Let $\delta=(n-1,n-2,\ldots,0)$ and, for a strictly decreasing integer tuple $\eta$, put $A_\eta(z)=\det(z_i^{\eta_j})$. The finite [Laurent polynomial](../../../../../laurent-polynomial.md) $\Delta\chi_\lambda$ is alternating. Every alternating [Laurent polynomial](../../../../../laurent-polynomial.md) is a [linear combination](../../../../../linear-combination.md) of the $A_\eta$: collect its monomials by [permutation](../../../../../permutation.md) orbits, and observe that an orbit with repeated exponents has zero coefficient by antisymmetry. Different $A_\eta$ are [orthogonal](../../../../../orthogonal-vectors.md) on $T$ and each has squared norm $n!$.

The coefficient of $z^{\lambda+\delta}$ in $\Delta\chi_\lambda$ is exactly one. Indeed, a contribution from the term $z^{w\delta}$ would require a [weight](../../../../../weight-representation-theory.md) $\lambda+\delta-w\delta$ in $V_\lambda$. For $w\ne1$, the vector $\delta-w\delta$ is a nonzero nonnegative combination of the positive [simple roots](../../../../../simple-root.md), so that [weight](../../../../../weight-representation-theory.md) lies above $\lambda$ and is impossible. The identity [permutation](../../../../../permutation.md) supplies the highest-weight coefficient one. Consequently

$$
\Delta\chi_\lambda=A_{\lambda+\delta}+\sum_{\eta\ne\lambda+\delta}c_\eta A_\eta.
$$

Apply the integration formula to $|\chi_\lambda|^2$. [Torus](../../../../../torus.md) [orthogonality](../../../../../orthogonal-vectors.md) gives

$$
1=\frac1{n!}\int_T|\Delta\chi_\lambda|^2\,dt
=1+\sum_{\eta\ne\lambda+\delta}|c_\eta|^2.
$$

All the other coefficients vanish, proving

$$
\boxed{\chi_\lambda(z)=\frac{\det(z_i^{\lambda_j+n-j})}{\det(z_i^{n-j})}.}
$$

The quotient extends across repeated [eigenvalues](../../../../../eigenvalue.md) because its product with the denominator is the already defined [continuous](../../../../../continuous-function.md) [character](../../../../../character-of-a-representation.md). Equivalently, alternant divisibility makes it a [Laurent polynomial](../../../../../laurent-polynomial.md) invariant under [permutations](../../../../../permutation.md); multiply by a [determinant](../../../../../determinant.md) power if negative exponents must first be removed.

Finally, $\delta-\rho=\frac{n-1}{2}(1,\ldots,1)$ is fixed by the [Weyl group](../../../../../weyl-group.md), so its common factor cancels in the quotient. Since $A_\rho=e^\rho\prod_{\alpha>0}(1-e^{-\alpha})$, the [determinant](../../../../../determinant.md) expression is exactly

$$
\chi_\lambda=\frac{\sum_{w\in W}\varepsilon(w)e^{w(\lambda+\rho)-\rho}}{\prod_{\alpha>0}(1-e^{-\alpha})}.
$$

Using $\delta$ in the derivation avoids treating a possibly half-integral $\rho$ as an actual [character](../../../../../character-of-a-representation.md) of the [torus](../../../../../torus.md). At the identity, taking the leading Vandermonde term of the two [determinants](../../../../../determinant.md) gives the accompanying [dimension](../../../../../dimension-vector-space.md) formula

$$
\dim V_\lambda=\prod_{i<j}\frac{\lambda_i-\lambda_j+j-i}{j-i}.
$$

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 19](../../paper-19-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
