<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

For the [transfer homomorphism](../../../../../transfer-group-theory.md), choose representatives $T$ of the right [cosets](../../../../../coset.md) $H\backslash G$. For $t\in T$ and $g\in G$, write $tg=h(t,g)t_g$, where $h(t,g)\in H$ and $t_g\in T$. The [permutation](../../../../../permutation.md) $t\mapsto t_g$ represents right multiplication on the [cosets](../../../../../coset.md). Define

$$
\boxed{V_{G,H}(g)=\prod_{t\in T}h(t,g)\pmod{H'}.}
$$

The product has no order ambiguity in the [abelianization](../../../../../abelianization.md) $H/H'$. Replace each representative $t$ by $a_tt$, with $a_t\in H$. The new factor is $a_t h(t,g)a_{t_g}^{-1}$. In the [Abelian](../../../../../abelian-group.md) quotient, the extra products cancel because $t\mapsto t_g$ permutes $T$. Thus the transfer is independent of the transversal. Moreover,

$$
h(t,g_1g_2)=h(t,g_1)h(t_{g_1},g_2).
$$

Multiplying and using the same [permutation](../../../../../permutation.md) of representatives gives $V(g_1g_2)=V(g_1)V(g_2)$. This proves that [group transfer](../../../../../transfer-group-theory.md) is a well-defined [group homomorphism](../../../../../group-homomorphism.md).

For the [Burnside transfer theorem](../../../../../burnside-transfer-theorem.md), let $P\subseteq Z(N_G(P))$ be a Sylow $p$-subgroup. In particular $P$ is [Abelian](../../../../../abelian-group.md). We first prove the fusion fact that two elements of $P$ which are conjugate in $G$ must be equal. Suppose $u\in P$ and $v=g^{-1}ug\in P$. Both $P$ and $g^{-1}Pg$ centralize $v$, and they are [Sylow subgroups](../../../../../sylow-subgroup.md) of $C_G(v)$: they have the maximal $p$-order possible even in $G$. By [Sylow theorems](../../../../../sylow-theorems.md) inside this [centralizer](../../../../../centralizer.md), choose $h\in C_G(v)$ with $h^{-1}g^{-1}Pgh=P$. Thus $gh\in N_G(P)$ and

$$
(gh)^{-1}u(gh)=h^{-1}vh=v.
$$

But $gh$ centralizes $P$ by hypothesis, so $v=u$.

Evaluate transfer to $P$ on $u\in P$. Partition the right [cosets](../../../../../coset.md) of $P$ into cycles under multiplication by $u$. For a cycle of length $r$ beginning at $Pt$, the product of its transfer factors telescopes to $tu^rt^{-1}\in P$. It is conjugate to $u^r\in P$, so the fusion fact makes it equal to $u^r$. The cycle lengths sum to $m=[G:P]$. Since $P$ is [Abelian](../../../../../abelian-group.md), all factors commute and

$$
V_{G,P}(u)=u^m.
$$

The integer $m$ is prime to $p$, and this power map is an automorphism of the finite [Abelian](../../../../../abelian-group.md) $p$-group $P$: choose an inverse exponent modulo the exponent of $P$. Therefore $V_{G,P}:G\to P$ is surjective. Its kernel $K$ is normal and the [first isomorphism theorem](../../../../../first-isomorphism-theorem.md) gives

$$
\boxed{[G:K]=|P|,\qquad |K|=[G:P].}
$$

Thus $K$ is the required [normal p-complement](../../../../../normal-p-complement.md); it also has trivial intersection with $P$.

Now suppose $P$ is cyclic of order $p^a$, where $p$ is the smallest prime divisor of $|G|$. [Conjugation](../../../../../conjugation.md) embeds $N_G(P)/C_G(P)$ into $\operatorname{Aut}(P)$, whose order is $p^{a-1}(p-1)$. Since $P\subseteq C_G(P)$ and $P$ is Sylow in $N_G(P)$, the quotient has order prime to $p$. Any remaining prime factor would divide $p-1$ and hence be smaller than $p$, but would also divide $|G|$, an impossibility. Thus $N_G(P)=C_G(P)$ and $P\subseteq Z(N_G(P))$. The [Burnside transfer theorem](../../../../../burnside-transfer-theorem.md) proves that **a cyclic [Sylow subgroup](../../../../../sylow-subgroup.md) at the least prime divisor gives a normal complement**.

Apply this to a finite nonabelian [simple group](../../../../../simple-group.md). If $p^3\nmid |G|$, its Sylow $p$-subgroup has order $p$ or $p^2$. A cyclic [Sylow subgroup](../../../../../sylow-subgroup.md) would give a normal complement; simplicity would then force either a trivial complement and a $p$-group, or an improper complement, neither possible for a nonabelian [simple group](../../../../../simple-group.md). [Groups](../../../../../group-split.md) of order $p^2$ are [Abelian](../../../../../abelian-group.md): their nontrivial [group center](../../../../../center-of-a-group.md), supplied by the [class equation](../../../../../class-equation.md), is either the whole [group](../../../../../group-split.md) or has cyclic quotient, which also forces the [group](../../../../../group-split.md) [Abelian](../../../../../abelian-group.md). Thus the only remaining Sylow possibility is $P\cong C_p^2$.

The [conjugation](../../../../../conjugation.md) quotient $N_G(P)/C_G(P)$ now embeds in $GL_2(p)$ and is still prime to $p$. Its possible prime divisors come from

$$
|GL_2(p)|=(p^2-1)(p^2-p)=p(p-1)^2(p+1).
$$

If $p$ is odd, every prime divisor of $p-1$ is smaller than $p$, and every prime divisor of the even number $p+1$ is at most $(p+1)/2<p$. Since $p$ was the least prime divisor of $|G|$, the quotient must be trivial. Then the [Burnside transfer theorem](../../../../../burnside-transfer-theorem.md) again contradicts simplicity. If $p=2$, the only nontrivial odd divisor of $|GL_2(2)|=6$ is three. Trivial [conjugation](../../../../../conjugation.md) would again give a normal complement, so three must divide $|G|$; the [Sylow subgroup](../../../../../sylow-subgroup.md) has order four. We have proved the [least-prime divisibility constraint for a finite simple group](../../../../../least-prime-divisibility-constraint-for-a-finite-simple-group.md):

$$
\boxed{p^3\mid |G|\quad\text{or}\quad p=2\text{ and }12\mid |G|.}
$$

For infinitely many instances of the latter alternative only, take

$$
G_m=PSL_2(5^{2m+1}),\qquad m\geq0.
$$

These are simple, as permitted in the question (and also covered by the next solution). For $q=5^{2m+1}$, the [group](../../../../../group-split.md) order is $q(q^2-1)/2$. Since $q\equiv5\pmod8$, $q-1$ is divisible by four but not eight and $q+1$ by two but not four. Hence the order is divisible by four but not eight. Also $q\not\equiv0\pmod3$, so $3\mid q^2-1$. Their smallest prime divisor is two and

$$
\boxed{12\mid |G_m|,\qquad8\nmid |G_m|.}
$$

Their orders strictly increase with $m$, so they give infinitely many distinct examples.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 1](../../paper-1-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
