<h1 id="7e/solution">Solution</h1>

↑ **Parent:** [7E](../7e.md)

If $A$ is nonempty, take $a\in A$. The stated implication repeatedly gives $a+jt\in A$ for $j=0,1,\ldots,p-1$. These residues are all distinct: equality of two would give $(j-\ell)t=0$ in the [prime field](../../../../../prime-field.md) $\mathbb Z_p$, and the nonzero $t$ can be cancelled. They therefore exhaust the field. Thus

$$
\boxed{A+t\subseteq A,\quad t\ne0\quad\Longrightarrow\quad A=\varnothing\text{ or }A=\mathbb Z_p.}
$$

Equivalently, a nonzero element generates the additive [cyclic group](../../../../../cyclic-group.md) of prime order.

Now assume $0<k<p$. If $A+s=A+t$ with $s\ne t$, translating by $-s$ gives $A=A+(t-s)$, contradicting the preceding result. Hence all $p$ translates are distinct. Translation defines equivalence classes on the collection of all $k$-element subsets: two subsets are equivalent if one is a translate of the other, and each class contains exactly $p$ subsets. Since there are $\binom pk$ such subsets, their partition into classes gives

$$
\boxed{p\mid\binom pk\qquad(1\leq k\leq p-1).}
$$

This is the [free translation action on nontrivial subsets of a prime cyclic group](../../../../../free-translation-action-on-nontrivial-subsets-of-a-prime-cyclic-group.md).

The [binomial theorem](../../../../../binomial-theorem.md) now gives, in the [prime field](../../../../../prime-field.md),

$$
(a+1)^p=a^p+1+\sum_{j=1}^{p-1}\binom pj a^j= a^p+1.
$$

Starting with $0^p=0$ and applying this identity successively to the representatives $0,1,\ldots,p-1$ proves $a^p=a$ for every residue $a$. For nonzero $a$, cancellation gives

$$
\boxed{a^p=a\text{ in }\mathbb Z_p;\qquad a^{p-1}=1\text{ if }a\ne0,}
$$

which is [Fermat's little theorem](../../../../../fermat-little-theorem.md), or $a^p\equiv a\pmod p$ for every integer $a$ and $a^{p-1}\equiv1$ when $p\nmid a$.

The same vanishing of intermediate [binomial coefficients](../../../../../binomial-coefficient.md) proves $(R+S)^p=R^p+S^p$ for any commuting elements in a ring whose [ring characteristic](../../../../../characteristic-of-a-ring.md) is $p$, in particular for polynomials over $\mathbb Z_p$. Applying this repeatedly to the terms of $Q$, and applying [Fermat's little theorem](../../../../../fermat-little-theorem.md) to each coefficient, gives the [Frobenius endomorphism](../../../../../frobenius-endomorphism.md) identity

$$
Q(x)^p=\sum_{j=0}^n(a_jx^j)^p=\sum_{j=0}^na_j^px^{pj},\qquad \boxed{Q(x)^p=\sum_{j=0}^na_jx^{pj}=Q(x^p).}
$$

This is an equality of formal [polynomials](../../../../../polynomial-split.md). It does not assert $x^p=x$ as a polynomial; that latter equality holds only after evaluating at elements of $\mathbb Z_p$.

## ↑ Ancestors (10)

1. [7E](../7e.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ia](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
