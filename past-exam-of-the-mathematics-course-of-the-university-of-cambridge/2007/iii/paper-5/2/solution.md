<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

For odd $p$, a [subgroup](../../../../../subgroup.md) $N$ is [powerfully embedded](../../../../../powerfully-embedded-subgroup.md) in $G$ if $[N,G]\le N^p$, where $N^p=\langle n^p:n\in N\rangle$. The condition implies normality since $n^g=n[n,g]\in N$. The [group](../../../../../group-split.md) $G$ is a [powerful p-group](../../../../../powerful-p-group.md) if $[G,G]\le G^p$, equivalently if $G$ itself is [powerfully embedded](../../../../../powerfully-embedded-subgroup.md). For a [finite p-group](../../../../../finite-p-group.md), the [Burnside basis theorem](../../../../../burnside-basis-theorem.md) gives $d(Q)=\dim_{\mathbb F_p}Q/\Phi(Q)$, and $\Phi(Q)=Q^p[Q,Q]$. Thus for powerful $Q$, $d(Q)=\dim Q/Q^p$.

We prove $d(H)\le d(G)$ by induction on $|G|$, with the trivial [group](../../../../../group-split.md) immediate. The supplied embedding result applied to $N=G$ makes $G^p$ [powerfully embedded](../../../../../powerfully-embedded-subgroup.md), and hence powerful. It is a proper [subgroup](../../../../../subgroup.md) when $G\ne1$, because $G^p=\Phi(G)$ is proper in a nontrivial [finite p-group](../../../../../finite-p-group.md). Set

$$
K=H\cap G^p,\quad V=G/G^p,\quad W=G^p/G^{p^2},\quad A=HG^p/G^p\le V.
$$

All the displayed quotients are [elementary abelian](../../../../../elementary-abelian-group.md). The supplied onto [homomorphism](../../../../../homomorphism.md) $\theta:V\to W$, $xG^p\mapsto x^pG^{p^2}$, is therefore linear. Write $v=\dim V=d(G)$, $w=\dim W=d(G^p)$, $r=\dim A$, and $t=\dim\theta(A)$.

Since $H/K$ embeds in $V$, $\Phi(H)\le K$. Also

$$
\Phi(K)\le\Phi(H),\qquad\Phi(K)=K^p[K,K]\le(G^p)^p[G^p,G^p]=G^{p^2}.
$$

Here $(G^p)^p=G^{p^2}$ is the iterated-power convention, valid for powerful [groups](../../../../../group-split.md). Hence the natural map $K/\Phi(K)\to W$ is defined. The image under this map of the subspace $\Phi(H)/\Phi(K)$ contains $\theta(A)$, because for every $h\in H$ its power $h^p$ lies in $\Phi(H)\cap K$. It follows that

$$
\dim K/\Phi(H)\le d(K)-t.
$$

The [exact sequence](../../../../../exact-sequence.md) $1\to K/\Phi(H)\to H/\Phi(H)\to H/K\to1$ consists of [elementary abelian groups](../../../../../elementary-abelian-group.md), and $\dim H/K=r$. By induction inside $G^p$, $d(K)\le d(G^p)=w$. Therefore

$$
d(H)=r+\dim K/\Phi(H)\le r+w-t=w+\dim\ker(\theta|_A)\le w+\dim\ker\theta=v.
$$

This proves **$d(H)\le d(G)$**, including [subgroups](../../../../../subgroup.md) $H$ that are not themselves powerful.

The [rank of a profinite group](../../../../../rank-of-a-profinite-group.md) is $\operatorname{rk}(P)=\sup\{d(K):K\le P\text{ closed}\}$, where $d(K)$ is its least topological generator number. If $P$ has finite rank then every [closed subgroup](../../../../../closed-subgroup.md), including the [open subgroup](../../../../../open-subgroup.md) $H$, has no larger rank. Conversely suppose $H$ has rank $r<\infty$. Its [normal core](../../../../../core-group-theory.md) $C=\bigcap_{g\in P}H^g$ is an [open normal subgroup](../../../../../open-normal-subgroup.md): there are finitely many conjugates because $H$ has finite index. It has rank at most $r$.

For every closed $K\le P$, the [subgroup](../../../../../subgroup.md) $K\cap C$ is normal in $K$ and has at most $r$ topological generators. The quotient $K/(K\cap C)$ embeds in the [finite group](../../../../../finite-group.md) $P/C$. A [finite group](../../../../../finite-group.md) of order at most $M=[P:C]$ has at most $\lfloor\log_2M\rfloor$ generators: in a minimal sequential generating list every strict enlargement at least doubles the [subgroup](../../../../../subgroup.md) order. Lift such quotient generators and adjoin generators of $K\cap C$. Their closed generated [subgroup](../../../../../subgroup.md) contains the [group homomorphism kernel](../../../../../kernel-of-a-group-homomorphism.md) and maps onto the quotient, so equals $K$. Consequently

$$
\boxed{\operatorname{rk}(P)\le r+\lfloor\log_2[P:C]\rfloor<\infty.}
$$

Thus **an [open subgroup](../../../../../open-subgroup.md) has finite rank exactly when the whole [profinite group](../../../../../profinite-group.md) does**.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 5](../../paper-5-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
