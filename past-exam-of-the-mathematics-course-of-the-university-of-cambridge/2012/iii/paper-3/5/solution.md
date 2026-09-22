<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

The [coordinate ring](../../../../../coordinate-ring.md) is $\mathbb C[W]=\operatorname{Sym}(W^*)$. The induced action is contragredient on functions:

$$
(g\cdot p)(w)=p(\rho(g^{-1})w).
$$

It is a [group action](../../../../../group-action.md) by degree-preserving algebra automorphisms, extending the dual action on linear [polynomial functions](../../../../../polynomial-function.md). Its [polynomial invariant ring](../../../../../polynomial-invariant-ring.md) is

$$
\mathbb C[W]^G=\{p\in\mathbb C[W]:g\cdot p=p\text{ for every }g\in G\}.
$$

For a monic [polynomial](../../../../../polynomial-split.md) $f(t)=\prod_{i=1}^d(t-r_i)$, its [polynomial discriminant](../../../../../polynomial-discriminant.md) is $\operatorname{disc}(f)=\prod_{i<j}(r_i-r_j)^2$. This is symmetric in the roots, hence [polynomial](../../../../../polynomial-split.md) in the coefficients, and is zero exactly when a root is repeated.

For the [alternating group](../../../../../alternating-group.md) action, let $e_1,\ldots,e_n$ be the [elementary symmetric polynomials](../../../../../elementary-symmetric-polynomial.md) and put $\Delta=\prod_{i<j}(X_i-X_j)$. If $p$ is $A_n$-invariant and $\tau$ is any [transposition](../../../../../transposition-permutation.md), decompose

$$
p=p_++p_-,\qquad p_+=\frac{p+\tau p}{2},\quad p_-=\frac{p-\tau p}{2}.
$$

Normality and index two of $A_n$ show that $p_+$ is symmetric and $p_-$ transforms by the sign [character](../../../../../character-of-a-representation.md) of $S_n$. Any [alternating polynomial](../../../../../alternating-polynomial.md) vanishes when $X_i=X_j$, so every $X_i-X_j$ divides it. These pairwise nonassociate prime factors have product $\Delta$, so $p_-=\Delta q$ with $q$ symmetric. The [Fundamental theorem of symmetric polynomials](../../../../../fundamental-theorem-of-symmetric-polynomials.md) yields

$$
\mathbb C[X_1,\ldots,X_n]^{A_n}
=\mathbb C[e_1,\ldots,e_n]\oplus\Delta\mathbb C[e_1,\ldots,e_n].
$$

The sum is direct, since a [polynomial](../../../../../polynomial-split.md) that is both symmetric and alternating is zero in [characteristic zero](../../../../../characteristic-zero.md). Also $\Delta^2=D(e_1,\ldots,e_n)$, where $D$ is the discriminant [polynomial](../../../../../polynomial-split.md) of

$$
t^n-e_1t^{n-1}+e_2t^{n-2}-\cdots+(-1)^ne_n.
$$

Thus, more precisely than the requested quotient assertion,

$$
\boxed{\mathbb C[X_1,\ldots,X_n]^{A_n}
\cong\mathbb C[T_1,\ldots,T_n,Z]/(Z^2-D(T_1,\ldots,T_n)).}
$$

Surjectivity follows from the direct-sum expression. Divide any putative kernel element by the monic quadratic in $Z$; its remainder is $a(T)+Zb(T)$. The [direct sum](../../../../../direct-sum.md) forces $a(e)=b(e)=0$, and [algebraic independence](../../../../../algebraic-independence.md) of the $e_i$ gives $a=b=0$. Hence the displayed relation is the entire kernel. The argument also covers $n=2$, where $A_2$ is trivial.

Now let $G$ be finite with no nontrivial [linear characters](../../../../../linear-character.md), and write $R=\mathbb C[W]$, $S=R^G$. The [polynomial ring](../../../../../polynomial-ring.md) $R$ is a [unique factorization domain](../../../../../unique-factorization-domain.md). Factor a nonzero invariant $f$ in $R$; invariance permutes the associate classes of its irreducible factors and makes their exponents constant on each orbit. For an orbit $\mathcal O$, choose representatives and form its [orbit product of polynomial factors](../../../../../orbit-product-of-polynomial-factors.md)

$$
q_{\mathcal O}=\prod_{p\in\mathcal O}p.
$$

For every $g$, $g\cdot q_{\mathcal O}=\theta(g)q_{\mathcal O}$ for a nonzero scalar $\theta(g)$. Applying two group elements proves that $\theta:G\to\mathbb C^\times$ is a homomorphism. The hypothesis forces $\theta=1$, so $q_{\mathcal O}\in S$.

This orbit product is prime in $S$. If it divides $ab$ with $a,b\in S$, one factor $p\in\mathcal O$ divides $a$ or $b$ in $R$. Invariance of that chosen [polynomial](../../../../../polynomial-split.md) makes every factor in the orbit divide it. Their product therefore divides it in $R$, and the quotient is invariant because numerator and denominator are invariant and cancellation is valid in the [integral domain](../../../../../integral-domain.md) $R$. Thus $q_{\mathcal O}$ divides $a$ or $b$ in $S$. Every nonzero $f\in S$ is a scalar times a product of these prime orbit products, and the only units of $S$ are nonzero constants, as they are units in $R$. Therefore **$\mathbb C[W]^G$ is a [unique factorization domain](../../../../../unique-factorization-domain.md)**. This gives a direct proof, without assuming a divisor-class-group theorem.

For a failure in [characteristic zero](../../../../../characteristic-zero.md), let the [cyclic group](../../../../../cyclic-group.md) of order two act on $\mathbb C^2$ by $-I$. Its coordinate invariants are

$$
S=\mathbb C[X^2,XY,Y^2]
\cong\mathbb C[a,b,c]/(ac-b^2).
$$

Every invariant [monomial](../../../../../monomial.md) has even total degree: its exponents are either both even, or both odd, giving the indicated generators. Reducing powers of $b$ to at most one shows that $ac-b^2$ is the only relation, since $a^ic^j$ and $ba^ic^j$ map to distinct [monomials](../../../../../monomial.md). The three quadratic invariants are irreducible in $S$: each nonconstant invariant has degree at least two, so a product of two nonunits has degree at least four. They are pairwise nonassociate, but

$$
\boxed{X^2Y^2=(X^2)(Y^2)=(XY)^2}
$$

gives two different irreducible factorizations. Hence **this invariant ring is not a [unique factorization domain](../../../../../unique-factorization-domain.md)**. The nontrivial sign [character](../../../../../character-of-a-representation.md) is precisely the kind of [character](../../../../../character-of-a-representation.md) excluded in the preceding theorem.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 3](../../paper-3-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
