<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $R=\mathcal O_K$. We prove [unique factorization of ideals in a number field](../../../../unique-factorization-of-ideals-in-a-number-field.md), rather than assuming this conclusion as a property of a [Dedekind domain](../../../../dedekind-domain.md). Three preliminary facts about $R$ will be useful. Its [additive group](../../../../additive-group.md) is a finite-rank [free abelian group](../../../../free-abelian-group.md), so every [ideal](../../../../ideal.md) is finitely generated and the [ascending chain condition](../../../../ascending-chain-condition.md) holds. It is an [integrally closed domain](../../../../integrally-closed-domain.md), by [integral dependence is transitive](../../../../integral-dependence-is-transitive.md). Finally, every nonzero [prime ideal](../../../../prime-ideal.md) is a [maximal ideal](../../../../maximal-ideal.md). For this last fact, choose $0\ne a\in P$. Multiplication by $a$ is an injective endomorphism of the finite-rank [free abelian group](../../../../free-abelian-group.md) $R$ with nonzero [determinant](../../../../determinant.md), so $R/(a)$ is finite. Consequently $R/P$ is a finite [integral domain](../../../../integral-domain.md) and hence a [field](../../../../field.md).

First, every nonzero proper [ideal](../../../../ideal.md) contains a product of nonzero [prime ideals](../../../../prime-ideal.md). Otherwise choose a maximal counterexample $J$ under inclusion, using the [ascending chain condition](../../../../ascending-chain-condition.md). It cannot be a [prime ideal](../../../../prime-ideal.md). Choose $x,y\notin J$ with $xy\in J$. The strictly larger [ideals](../../../../ideal.md) $J+(x)$ and $J+(y)$ each contain a product of nonzero [prime ideals](../../../../prime-ideal.md), allowing the empty product $R$ when necessary. Multiplying those products gives a product contained in

$$
(J+(x))(J+(y))\subseteq J,
$$

a contradiction.

Next fix a nonzero [prime ideal](../../../../prime-ideal.md) $P$, choose $0\ne a\in P$, and choose a product of nonzero [prime ideals](../../../../prime-ideal.md)

$$
P_1\cdots P_r\subseteq(a)
$$

with $r$ minimal. Because $(a)\subseteq P$, primality and maximality imply $P_j=P$ for some $j$; reorder so that $P_1=P$. Minimality provides $b\in P_2\cdots P_r$ with $b\notin(a)$, taking the remaining product to be $R$ if $r=1$. Thus

$$
x=b/a\notin R,\qquad xP\subseteq R.
$$

Define the [fractional ideal](../../../../fractional-ideal.md)

$$
P^{-1}=\{z\in K:zP\subseteq R\}.
$$

It contains $R$ and $x$. The [ideal](../../../../ideal.md) $PP^{-1}$ lies between $P$ and $R$, so it is $P$ or $R$. If it were $P$, then $xP\subseteq P$. Applying the [determinant trick](../../../../determinant-trick.md) to a finite [generating set of an ideal](../../../../generating-set-of-an-ideal.md) for $P$ gives a [monic polynomial](../../../../monic-polynomial.md) over $R$ satisfied by $x$. Since $R$ is an [integrally closed domain](../../../../integrally-closed-domain.md), this would put $x$ in $R$, a contradiction. Therefore

$$
\boxed{PP^{-1}=R}.
$$

This proves that each nonzero [prime ideal](../../../../prime-ideal.md) is an [invertible fractional ideal](../../../../invertible-fractional-ideal.md), independently of the desired factorization theorem.

Now take a nonzero proper [ideal](../../../../ideal.md) $A$ and a [maximal ideal](../../../../maximal-ideal.md) $P$ containing it. The [ideal](../../../../ideal.md) $B=P^{-1}A$ satisfies

$$
A\subseteq B\subseteq R,\qquad A=PB.
$$

The first inclusion is strict: if $A=B$, the same $x\in P^{-1}\setminus R$ would stabilize $A$, and the [determinant trick](../../../../determinant-trick.md) would again force $x\in R$. Repeating gives a strictly ascending chain until it reaches $R$; the [ascending chain condition](../../../../ascending-chain-condition.md) ensures this happens after finitely many steps. The identities $A=PB$ then express $A$ as a product of nonzero [prime ideals](../../../../prime-ideal.md).

For uniqueness, suppose $P_1\cdots P_r=Q_1\cdots Q_s$. Since the right-hand side is contained in $P_1$, some $Q_j$ is contained in $P_1$. Both are nonzero [maximal ideals](../../../../maximal-ideal.md), so $Q_j=P_1$. Multiplication by $P_1^{-1}$ cancels this factor. Repeat. A nonempty product of proper [prime ideals](../../../../prime-ideal.md) cannot equal $R$, so both products finish together. This proves uniqueness up to reordering, including repeated factors.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the algebraic number theory course of the University of Oxford](../../../split.md)
5. [Algebraic number theory course of the University of Oxford](../../../../algebraic-number-theory-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
