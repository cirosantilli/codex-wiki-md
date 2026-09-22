<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

For $H\le G$ of finite [subgroup index](../../../../../index-of-a-subgroup.md), let $H'= [H,H]$ and choose a right-coset transversal $T$ for the [cosets](../../../../../coset.md) $Ht$. For each $g\in G$ write

$$
tg=h(t,g)t_g,\qquad h(t,g)\in H,\quad t_g\in T.
$$

The [transfer homomorphism](../../../../../transfer-group-theory.md) is

$$
\boxed{V_{G,H}(g)=\prod_{t\in T}h(t,g)\pmod{H'}\ \in H/H'.}
$$

The product is taken in the [abelianization](../../../../../abelianization.md), so its order is irrelevant. If another transversal has representative $a_tt$ for $Ht$, with $a_t\in H$, its factor is $a_t h(t,g)a_{t_g}^{-1}$. The map $t\mapsto t_g$ permutes $T$, so the extra factors cancel in $H/H'$. This proves independence of the transversal. Also

$$
h(t,g_1g_2)=h(t,g_1)h(t_{g_1},g_2).
$$

Multiplying over $t$ and again permuting the second indices proves $V(g_1g_2)=V(g_1)V(g_2)$. Thus it is indeed a [group homomorphism](../../../../../group-homomorphism.md).

The [Burnside transfer theorem](../../../../../burnside-transfer-theorem.md) states that if a Sylow $p$-subgroup $P$ of a [finite group](../../../../../finite-group.md) satisfies $P\subseteq Z(N_G(P))$, then $G$ has a normal $p$-complement: a [normal subgroup](../../../../../normal-subgroup.md) of order $|G|/|P|$. The hypothesis first makes $P$ abelian. It also makes fusion inside $P$ trivial. To prove this, suppose $u,v\in P$ and $u^g=v$, using $u^g=g^{-1}ug$. Both $P$ and $P^g$ lie in $C_G(v)$: the former because $P$ is abelian, and the latter because $v\in P^g$. They are [Sylow subgroups](../../../../../sylow-subgroup.md) of that [centralizer](../../../../../centralizer.md). Choose $c\in C_G(v)$ with $(P^g)^c=P$. Then $gc\in N_G(P)$ and $u^{gc}=v^c=v$, while the central-normalizer hypothesis gives $u^{gc}=u$. Thus $u=v$.

Evaluate transfer to the [abelian group](../../../../../abelian-group.md) $P$ on $u\in P$. In the action of $u$ on right [cosets](../../../../../coset.md), a cycle of length $r$ contributes

$$
\prod_{j=0}^{r-1}t_jut_{j+1}^{-1}=t_0u^rt_0^{-1}\in P,
$$

with $t_r=t_0$. This is a conjugate of $u^r$ inside $P$ and hence equals $u^r$ by the fusion argument. Summing the cycle lengths therefore gives

$$
V_{G,P}(u)=u^{[G:P]}.
$$

The exponent is coprime to $p$, so this power map is an [automorphism](../../../../../automorphism.md) of the finite abelian $p$-group $P$. Transfer is consequently onto $P$, and its kernel is normal of [subgroup index](../../../../../index-of-a-subgroup.md) $|P|$ and of order prime to $p$. This proves the theorem. Notice also that a normal $p$-complement consists exactly of the elements of prime-to-$p$ order: they map trivially to the $p$-group quotient, while all elements of the complement have such order. It is therefore unique and a [characteristic subgroup](../../../../../characteristic-subgroup.md).

Now let $G\le A_p$ be primitive of degree $p=2q+1$, with $q$ prime. Every nontrivial [normal subgroup](../../../../../normal-subgroup.md) of a faithful [primitive group action](../../../../../primitive-group-action.md) is transitive: its orbits form a $G$-invariant block partition, and singleton orbits would make it trivial. Such a subgroup has order divisible by $p$. A Sylow $p$-subgroup $P$ has order $p$, since $p!$ contains only one factor $p$. The [normalizer](../../../../../normalizer.md) of a regular $p$-cycle in $S_p$ is the affine group $x\mapsto ax+b$ on $\mathbb F_p$, of order $p(p-1)$. Translations are even, whereas a generating multiplier gives a $(p-1)$-cycle and is odd. Its [normalizer](../../../../../normalizer.md) in $A_p$ therefore has order $p(p-1)/2=pq$.

Suppose $G$ is not simple and choose $1<N\triangleleft G$ proper. It is transitive, so we can choose $P\le N$. The [Frattini argument](../../../../../frattini-argument.md) gives $G=NN_G(P)$: for each $g$, the subgroup $P^g$ is a [Sylow subgroup](../../../../../sylow-subgroup.md) of $N$ and can be conjugated back to $P$ within $N$. Since $N_G(P)$ contains $P$ and lies in the order-$pq$ [normalizer](../../../../../normalizer.md), it has order $p$ or $pq$. If its order were $p$, the Burnside theorem applied to $G$ would give a normal $p$-complement. A nontrivial such complement cannot be transitive because its order is prime to $p$, contradicting primitivity. It must be trivial, giving $G=P$, contrary to the choice of $N$. Thus $|N_G(P)|=pq$.

The intersection $N_N(P)$ again has order $p$ or $pq$. If it had order $pq$, the whole [normalizer](../../../../../normalizer.md) would lie in $N$ and the Frattini equality would give $G=N$. Hence $N_N(P)=P$. Applying Burnside transfer within $N$ gives its normal $p$-complement $K$. By the uniqueness argument, $K$ is a [characteristic subgroup](../../../../../characteristic-subgroup.md) of $N$, and so normal in $G$. Primitivity again forces this prime-to-$p$ subgroup to be trivial. Thus $N=P$ is normal in $G$, and $G=N_G(P)$ has order $pq$. The [even primitive groups of safe-prime degree](../../../../../even-primitive-groups-of-safe-prime-degree.md) conclusion is

$$
\boxed{G\text{ is simple, or }|G|=pq.}
$$

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 1](../../paper-1-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
