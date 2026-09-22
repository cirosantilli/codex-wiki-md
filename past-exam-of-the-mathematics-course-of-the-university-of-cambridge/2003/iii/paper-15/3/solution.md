<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The usual [field norm](../../../../../field-norm.md) $N_{L/K}$ is defined for a finite field extension. The printed hypothesis “algebraic” alone allows an infinite extension, for which this determinant norm is not defined. We therefore assume $[L:K]<\infty$. For an arbitrary algebraic extension the meaningful elementwise statement is instead $N_{K(b)/K}(b)\in A$, and we prove this as well.

First a [unique factorization domain](../../../../../unique-factorization-domain.md) is an [integrally closed domain](../../../../../integrally-closed-domain.md). Indeed, write an integral fraction as $u/v$ with relatively prime numerator and denominator. A monic integral equation, after multiplication by $v^r$, shows that $v$ divides $u^r$. Unique factorization forces $v$ to be a unit.

Let $m_b(T)=T^r+a_{r-1}T^{r-1}+\cdots+a_0\in K[T]$ be the monic [minimal polynomial](../../../../../minimal-polynomial.md) of $b$. Because $b$ is an [integral element](../../../../../integral-element.md) over $A$, it satisfies a monic polynomial $f\in A[T]$, and $m_b$ divides $f$ in $K[T]$. Every root of $m_b$ in an algebraic closure is therefore integral over $A$. This assertion includes repeated roots when the extension is inseparable. The coefficients of $m_b$ are elementary symmetric expressions in these roots. The [integral elements](../../../../../integral-element.md) form a ring: finitely many integral elements generate a finite $A$-module algebra, and the determinant trick shows every element of that algebra is integral. Thus all $a_i$ are integral over $A$. Since $a_i\in K$ and $A$ is integrally closed, $a_i\in A$.

Multiplication by $b$ on $K(b)$, in the basis $1,b,\ldots,b^{r-1}$, has the companion matrix of $m_b$, whose determinant is $(-1)^ra_0$. If $e=[L:K(b)]$, take a $K(b)$-basis of $L$. Multiplication by $b$ preserves each summand in the resulting [direct sum](../../../../../direct-sum.md) of $e$ copies of $K(b)$, so its determinant over $K$ is

$$
\boxed{N_{L/K}(b)=\bigl((-1)^ra_0\bigr)^e\in A.}
$$

In particular $N_{K(b)/K}(b)=(-1)^ra_0\in A$. The argument requires no separability; in fact it holds for every [integrally closed domain](../../../../../integrally-closed-domain.md), not just a [unique factorization domain](../../../../../unique-factorization-domain.md).

For the connection with dimension, let $B$ be the coordinate ring of an irreducible [affine variety](../../../../../affine-algebraic-set.md). By [Noether normalization](../../../../../noether-normalization.md) there is a finite integral inclusion $A=k[t_1,\ldots,t_d]\subset B$, with $d=\dim B$. Their fraction fields form a finite extension. For any $0\ne b\in B$, its minimal-polynomial constant term $a_0$ is nonzero and lies in $A$. Its equation gives

$$
a_0=-b\bigl(b^{r-1}+a_{r-1}b^{r-2}+\cdots+a_1\bigr)\in bB\cap A.
$$

Thus a nonzero function on the normalized variety produces a nonzero function on the base that vanishes wherever $b$ vanishes. Up to sign, the [field norm](../../../../../field-norm.md) is a power of this $a_0$, so it too belongs to $bB\cap A$.

Under the [finite morphism](../../../../../finite-morphism.md) to $\mathbb A^d$, the image of $V_B(b)$ is therefore contained in the proper [Zariski-closed set](../../../../../zariski-closed-set.md) $V_A(a_0)$ of dimension at most $d-1$. [Finite morphisms](../../../../../finite-morphism.md) preserve the dimension of a closed subvariety and its image. Applying this to a nonzero element of the ideal of any proper closed subvariety proves **proper closed subvarieties have strictly smaller dimension**. This is the useful role of the norm argument: nonzero equations upstairs give nonzero equations downstairs under a finite normalization.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 15](../../paper-15-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
