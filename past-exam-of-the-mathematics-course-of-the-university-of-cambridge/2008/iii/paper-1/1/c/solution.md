<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For an [orthonormal basis](../../../../../../orthonormal-basis.md) $(e_i)$, define the [Hilbert-Schmidt norm](../../../../../../hilbert-schmidt-norm.md) by $\|T\|_2^2=\sum_i\|Te_i\|^2$. For a possibly uncountable [basis](../../../../../../basis.md), the nonnegative sum means the supremum over finite subsets. [Parseval's identity](../../../../../../parseval-identity.md) gives, for any other [orthonormal basis](../../../../../../orthonormal-basis.md) $(f_j)$,

$$
\sum_i\|Te_i\|^2=\sum_{i,j}|\langle Te_i,f_j\rangle|^2
=\sum_j\|T^*f_j\|^2.
$$

Changing the domain [basis](../../../../../../basis.md) in the last expression proves [basis](../../../../../../basis.md) independence. Polarization gives a basis-independent [inner product](../../../../../../inner-product.md)

$$
\boxed{\langle T,S\rangle_2=\sum_i\langle Te_i,Se_i\rangle
=\operatorname{Tr}(S^*T),}
$$

with the same first-argument linear convention. The sums converge by the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md). The operator-norm bound $\|T\|\leq\|T\|_2$ follows by applying Cauchy-Schwarz to the coordinates of a unit [vector](../../../../../../vector.md).

To prove completeness, let $(T_n)$ be Cauchy in this [norm](../../../../../../norm.md). The operator-norm bound gives a bounded-operator limit $T$. For a finite subset $F$ of the [basis](../../../../../../basis.md),

$$
\sum_{i\in F}\|(T_n-T)e_i\|^2
=\lim_{m\to\infty}\sum_{i\in F}\|(T_n-T_m)e_i\|^2.
$$

For large $n$, the right side is uniformly small by the Cauchy property. Taking the supremum over $F$ shows $T_n-T$ is [Hilbert-Schmidt](../../../../../../hilbert-schmidt-operator.md) and $\|T_n-T\|_2\to0$; it also shows $T$ is [Hilbert-Schmidt](../../../../../../hilbert-schmidt-operator.md). Thus **the [Hilbert-Schmidt operators](../../../../../../hilbert-schmidt-operator.md) form a [Hilbert space](../../../../../../hilbert-space-split.md)**. [Finite-rank operators](../../../../../../finite-rank-operator.md) are dense there: keeping finitely many [basis](../../../../../../basis.md) columns makes the sum of omitted squared column [norms](../../../../../../norm.md) tend to zero. The operator-norm bound then shows that every [Hilbert-Schmidt operator](../../../../../../hilbert-schmidt-operator.md) is compact.

Now let $U$ be a strongly continuous [unitary representation](../../../../../../unitary-representation.md) of the compact metric [group](../../../../../../group-split.md) $G$, as is standard for a representation of a topological [group](../../../../../../group-split.md). Fix $\xi\ne0$ and average the positive [rank-one operator](../../../../../../rank-one-operator.md) $R_{\xi,\xi}$:

$$
K=\int_G U_gR_{\xi,\xi}U_g^*\,dg.
$$

The integrand is continuous in the [Hilbert-Schmidt norm](../../../../../../hilbert-schmidt-norm.md), so this [Bochner integral](../../../../../../bochner-integral.md) exists in the complete space just proved. Normalized [Haar measure](../../../../../../haar-measure.md) and invariance show that $K$ is positive, compact and commutes with every $U_g$. Moreover,

$$
\langle K\xi,\xi\rangle=\int_G|\langle U_g\xi,\xi\rangle|^2\,dg>0:
$$

the integrand is positive near the identity and every nonempty open set has positive [Haar measure](../../../../../../haar-measure.md). Thus $K\ne0$. A nonzero [eigenspace](../../../../../../eigenspace.md) is finite-dimensional and invariant under $U$, by (a). Within it choose a nonzero [invariant subspace](../../../../../../invariant-subspace.md) of smallest dimension; it is irreducible. Its [orthogonal complement](../../../../../../orthogonal-complement.md) is invariant because the representation is unitary, so the finite-dimensional space splits into irreducibles.

Take a maximal orthogonal family of such finite-dimensional irreducible [invariant subspaces](../../../../../../invariant-subspace.md). If their closed span had a nonzero [orthogonal complement](../../../../../../orthogonal-complement.md), the same averaging argument on that complement would produce another member, contradicting maximality. Therefore

$$
\boxed{H=\bigoplus_\alpha H_\alpha,
\quad\dim H_\alpha<\infty,\quad U|_{H_\alpha}\text{ irreducible}.}
$$

This [compact averaging of a rank-one operator](../../../../../../compact-averaging-of-a-rank-one-operator.md) argument does not require $H$ itself to be separable. Strong [continuity](../../../../../../continuous-function.md) is the topological representation hypothesis used in the averaging step.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
