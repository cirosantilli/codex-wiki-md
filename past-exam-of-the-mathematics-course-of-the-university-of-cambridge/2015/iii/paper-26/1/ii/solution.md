<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [Hasse-Minkowski theorem](../../../../../../hasse-minkowski-theorem.md) says that a nondegenerate [quadratic form](../../../../../../quadratic-form.md) over a [number field](../../../../../../number-field.md) has a nonzero isotropic vector over that field if and only if it has one over every completion. In particular, over $\mathbb Q$ one tests $\mathbb R$ and every $\mathbb Q_\ell$. For the present integral form, a rational isotropic vector can be multiplied by a common denominator to give an integer one. This is the [Hasse-Minkowski principle](../../../../../../hasse-minkowski-theorem.md).

Write $P=p$, $R=p+12$ and $S=p+24$. All three primes are odd and exceed three: $p=2$ or $3$ would make $p+12$ composite. The [second supplementary law for quadratic reciprocity](../../../../../../second-supplementary-law-for-quadratic-reciprocity.md) gives

$$
\left(\frac2P\right)=(-1)^{(P^2-1)/8}.
$$

**Necessity at $P$.** Scale any nonzero vector over $\mathbb Q_P$ so that its coordinates lie in $\mathbb Z_P$ and at least one is a unit. Reduction of its equation modulo $P$ gives $y^2=2z^2$, since twelve is invertible modulo $P$. If the [Legendre symbol](../../../../../../legendre-symbol.md) $(2/P)$ is $-1$, this forces $P\mid y,z$. The original equation then forces $P\mid x$, because its other two terms are divisible by $P^2$. This contradicts the normalization. Thus

$$
\boxed{\text{a nonzero solution requires }p\equiv1\text{ or }7\pmod8.}
$$

**Sufficiency at the coefficient primes.** Suppose $(2/P)=1$. A nonzero solution modulo $P$ is $(x,y,z)=(0,\sqrt2,1)$. Its $y$-derivative is nonzero modulo $P$, so fixing the other two coordinates and applying the [Hensel lemma](../../../../../../hensel-s-lemma.md) lifts it to $\mathbb Q_P$.

Since $S\equiv P\pmod8$, the same [Legendre symbol](../../../../../../legendre-symbol.md) criterion gives $(2/S)=1$. Modulo $S$, the equation reduces to $y^2=2x^2$, and the vector $(1,\sqrt2,0)$ is a simple zero in the $y$ coordinate. It lifts to $\mathbb Q_S$. Modulo $R$, the coefficients of $x^2$ and $z^2$ are respectively $-12$ and $12$, so $(1,0,1)$ is a zero with nonzero $x$-derivative. It lifts to $\mathbb Q_R$.

**The remaining odd primes.** If $\ell$ is odd and divides none of $PRS$, the reduced [ternary quadratic form](../../../../../../ternary-quadratic-form.md) is nondegenerate. An elementary finite-field argument finds a zero with $z=1$: if its coefficients are $A,B,C$, the sets

$$
\{A x^2:x\in\mathbb F_\ell\},\qquad
\{-C-B y^2:y\in\mathbb F_\ell\}
$$

both have $(\ell+1)/2$ elements, so intersect. The resulting vector has nonzero $z$-derivative $2C$, and the [Hensel lemma](../../../../../../hensel-s-lemma.md) lifts it. This [isotropy of nondegenerate ternary quadratic forms over finite fields](../../../../../../isotropy-of-nondegenerate-ternary-quadratic-forms-over-finite-fields.md) verifies every remaining odd completion without an extra congruence condition.

**The dyadic and real places.** Setting $y=1,z=2$ reduces the dyadic problem to

$$
x^2=-3-\frac{84}{P}.
$$

The right side is a [2-adic unit](../../../../../../2-adic-unit.md) congruent to $-3-4=1$ modulo eight. The [unit square classes of the p-adic integers](../../../../../../unit-square-classes-of-the-p-adic-integers.md) computed above show that it is a square in $\mathbb Q_2$. This also explains the printed hint: its integer can be taken as $m=-(p+21)/2$. Over $\mathbb R$, the positive and negative coefficients make the form indefinite; for instance $x=0,z=1,y=\sqrt{S/R}$ gives a nonzero zero.

All completions now have a nonzero isotropic vector. The [Hasse-Minkowski theorem](../../../../../../hasse-minkowski-theorem.md), followed by clearing denominators, proves

$$
\boxed{\text{a nonzero integer solution exists }\iff p\equiv\pm1\pmod8.}
$$

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 26](../../../paper-26-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
