<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The [Noether normalization lemma](../../../../../noether-normalization-lemma.md) is valid over every [field](../../../../../field.md) $k$, including finite fields: a nonzero [finitely generated algebra](../../../../../finitely-generated-algebra.md) $C$ contains elements $y_1,\ldots,y_d$ with [algebraic independence](../../../../../algebraic-independence.md) over $k$ such that $C$ is finite as a [module](../../../../../module-mathematics.md) over the [polynomial ring](../../../../../polynomial-ring.md) $k[y_1,\ldots,y_d]$. We prove it without an infinite-field hypothesis.

Write $C=k[a_1,\ldots,a_n]$ and induct on $n$. If the generators have [algebraic independence](../../../../../algebraic-independence.md), they already give a [polynomial ring](../../../../../polynomial-ring.md) and the assertion is immediate. Otherwise choose a nonzero relation $F(a_1,\ldots,a_n)=0$. Choose an integer $M$ larger than every exponent in the monomials of $F$, and set

$$
b_i=a_i-a_n^{M^i}\quad(1\leq i<n).
$$

In $F(Y_1+T^{M},Y_2+T^{M^2},\ldots,Y_{n-1}+T^{M^{n-1}},T)$, the largest power of $T$ has a nonzero coefficient in $k$. Indeed, a monomial with exponents $(e_1,\ldots,e_n)$ contributes top weight $e_n+\sum_{i<n}e_iM^i$. These weights are distinct by uniqueness of base-$M$ expansion, so only one monomial contributes the highest power. After rescaling, the substituted relation is monic in $T$.

Consequently $a_n$ is an [integral element](../../../../../integral-element.md) over $C'=k[b_1,\ldots,b_{n-1}]$, and $C=C'[a_n]$ is finite over $C'$. Apply the induction hypothesis to $C'$ and compose the finite [module](../../../../../module-mathematics.md) extensions. This proves [Noether normalization by weighted substitutions](../../../../../noether-normalization-by-weighted-substitutions.md). The induction reaches $n=0$, where $C=k$. For an [integral domain](../../../../../integral-domain.md) $C$, taking [fraction fields](../../../../../field-of-fractions.md) makes the resulting extension finite algebraic, so $d$ is the [transcendence degree](../../../../../transcendence-degree.md) of $\operatorname{Frac}(C)/k$. More generally $d=\dim C$: [integral extensions preserve Krull dimension](../../../../../integral-extensions-preserve-krull-dimension.md), and a polynomial algebra in $d$ variables has [Krull dimension](../../../../../krull-dimension.md) $d$.

A useful bridge to the [Hilbert Nullstellensatz](../../../../../hilbert-nullstellensatz.md) is the [Zariski lemma](../../../../../zariski-s-lemma.md). If a [field](../../../../../field.md) $E$ is a [finitely generated algebra](../../../../../finitely-generated-algebra.md) over $k$, normalization makes it finite and integral over a [polynomial ring](../../../../../polynomial-ring.md) $P=k[y_1,\ldots,y_d]$. A subring over which a field is integral is a field: for nonzero $a\in P$, an integral equation for $a^{-1}\in E$, multiplied by $a^{r-1}$, expresses $a^{-1}$ as an element of $P$. Therefore $P$ must be a field. A [polynomial ring](../../../../../polynomial-ring.md) in a positive number of variables is not a field, since a variable has no polynomial inverse. Hence $d=0$ and $E/k$ is a [finite field extension](../../../../../finite-field-extension.md). This proves the [Zariski lemma](../../../../../zariski-s-lemma.md).

Now let $k$ be an [algebraically closed field](../../../../../algebraically-closed-field.md). The [Weak Hilbert Nullstellensatz](../../../../../weak-hilbert-nullstellensatz.md) says that every [maximal ideal](../../../../../maximal-ideal.md) of $k[X_1,\ldots,X_n]$ is uniquely of the form

$$
\boxed{\mathfrak m=(X_1-a_1,\ldots,X_n-a_n),\qquad a\in k^n.}
$$

To prove it, the residue field $k[X]/\mathfrak m$ is a field generated as a $k$-algebra by the images of the variables. The [Zariski lemma](../../../../../zariski-s-lemma.md) makes it finite algebraic over $k$, and algebraic closedness makes it $k$. Thus each $X_i$ has an image $a_i\in k$. The evaluation map has kernel the displayed ideal: subtracting the constant value of a polynomial expresses its difference as a combination of $X_i-a_i$. That kernel is maximal and contained in $\mathfrak m$, so equality holds. Conversely every evaluation kernel is maximal because its quotient is $k$. Uniqueness follows from the variable images. Every proper [ideal](../../../../../ideal.md) is contained in a [maximal ideal](../../../../../maximal-ideal.md), so it has a common zero; equivalently, an ideal with no common zero is the whole ring.

For an [ideal](../../../../../ideal.md) $I\subseteq k[X_1,\ldots,X_n]$, let $V(I)$ be its common-zero set and let $I(V(I))$ be all polynomials vanishing on that set. The [Strong Hilbert Nullstellensatz](../../../../../strong-hilbert-nullstellensatz.md) states

$$
\boxed{I(V(I))=\sqrt I.}
$$

The inclusion $\sqrt I\subseteq I(V(I))$ follows because a [field](../../../../../field.md) has no nonzero [nilpotent elements](../../../../../nilpotent.md). For the other inclusion, take $f$ vanishing on $V(I)$, with $f\ne0$, and form the [Rabinowitsch trick](../../../../../rabinowitsch-trick.md) ideal

$$
J=I\,k[X_1,\ldots,X_n,T]+(1-Tf).
$$

It has no common zero: at a zero of $I$ the second generator has value one. The [Weak Hilbert Nullstellensatz](../../../../../weak-hilbert-nullstellensatz.md) in $n+1$ variables gives $J=(1)$. Hence a finite identity has the form $1=\sum_j h_j(X,T)g_j(X)+h(X,T)(1-Tf)$, with $g_j\in I$. Substitute $T=f^{-1}$ in the [localization of a ring](../../../../../localization-of-a-ring.md) $k[X]_f$. Clearing the finitely many powers of $f$ occurring in denominators gives $f^r\in I$ for some $r$, so $f\in\sqrt I$. The case $f=0$ is immediate. This completes all three proofs. The algebraically closed hypothesis belongs to the two forms of the [Hilbert Nullstellensatz](../../../../../hilbert-nullstellensatz.md); it was not needed for the [Noether normalization lemma](../../../../../noether-normalization-lemma.md) or the [Zariski lemma](../../../../../zariski-s-lemma.md).

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 2](../../paper-2-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
