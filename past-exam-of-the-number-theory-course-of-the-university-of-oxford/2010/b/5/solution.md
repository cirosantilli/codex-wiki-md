<h1 id="b/5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

The [product of ideals](../../../../product-of-ideals.md) $AB$ consists of finite sums $\sum_ja_jb_j$ with $a_j\in A$, $b_j\in B$. [Ideal](../../../../ideal.md) divisibility $P\mid A$ means $A=PC$ for an [integral ideal](../../../../integral-ideal.md) $C$; in this ring it is equivalent to $A\subseteq P$. The [ideal norm](../../../../ideal-norm.md) is $N(A)=|\mathcal O_K/A|$, equivalently its additive lattice index.

If the [prime ideal](../../../../prime-ideal.md) $P$ divides $AB$ but does not divide $A$, choose $a\in A\setminus P$. For every $b\in B$, $ab\in AB\subseteq P$, so primality gives $b\in P$. Thus $B\subseteq P$, proving $P\mid B$.

Every nonzero proper [ideal](../../../../ideal.md) $A$ is contained in a maximal [ideal](../../../../ideal.md) $P$, which is prime. Then $P\mid A$, so $A=PB$. [Norm](../../../../norm.md) multiplicativity gives $N(B)=N(A)/N(P)<N(A)$ because $N(P)\ge2$. Induction on the positive [integer](../../../../integer-split.md) $N(A)$ gives a prime-[ideal](../../../../ideal.md) factorization, ending at [norm](../../../../norm.md) one. For uniqueness, a prime in one factorization divides some prime in the other. Every nonzero [prime ideal](../../../../prime-ideal.md) is maximal, since its quotient is a finite integral domain and hence a [field](../../../../field.md). The two primes therefore coincide. Cancel that common factor using the permitted cancellation law, and continue. This proves uniqueness up to order.

The finite additive [group](../../../../group-split.md) $\mathcal O_K/A$ has order $N(A)$, so that [integer](../../../../integer-split.md) annihilates the class of $1$. Therefore

$$
\boxed{N(A)\in A.}
$$

In particular an [ideal](../../../../ideal.md) of [norm](../../../../norm.md) $m$ contains $(m)$. Such ideals correspond to certain additive subgroups of the finite [group](../../../../group-split.md) $\mathcal O_K/(m)$, so there are finitely many. Finiteness of these quotients follows from an [integral basis](../../../../integral-basis.md); a nonzero [ideal](../../../../ideal.md) contains a nonzero [principal ideal](../../../../principal-ideal.md), whose index is the absolute [field norm](../../../../field-norm.md) of its generator.

For the computation put $s=\sqrt{-6}$. The [Kummer-Dedekind theorem](../../../../kummer-dedekind-theorem.md) says that when $p$ does not divide the power-[basis](../../../../basis.md) index, a factorization $\bar f=\prod_i\bar g_i^{e_i}$ gives $(p)=\prod_i(p,g_i(s))^{e_i}$, with each factor having [norm](../../../../norm.md) $p^{\deg g_i}$. The given full power [basis](../../../../basis.md) has index one. Since $X^2+6\equiv X^2\pmod2$ and $X^2+6\equiv(X-1)(X+1)\pmod7$,

$$
\boxed{(2)=P^2,\quad P=(2,s);\qquad
(7)=QQ',\quad Q=(7,s-1),\ Q'=(7,s+1).}
$$

Here $N(P)=2$ and $N(Q)=N(Q')=7$. A [prime ideal](../../../../prime-ideal.md) dividing an [ideal](../../../../ideal.md) of [norm](../../../../norm.md) $98=2\cdot7^2$ lies above $2$ or $7$, and these are all the prime ideals above them. Unique factorization and [norm](../../../../norm.md) multiplicativity therefore leave exactly

$$
\boxed{PQ^2,\qquad PQQ'=(7)P,\qquad P(Q')^2.}
$$

They are distinct by their prime-[ideal](../../../../ideal.md) valuations, and each has [norm](../../../../norm.md) $98$.

## ↑ Ancestors (12)

1. [5](../5.md)
2. [B](../../b.md)
3. [2010](../../../2010-split.md)
4. [Past exam of the number theory course of the University of Oxford](../../../split.md)
5. [Number theory course of the University of Oxford](../../../../number-theory-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
