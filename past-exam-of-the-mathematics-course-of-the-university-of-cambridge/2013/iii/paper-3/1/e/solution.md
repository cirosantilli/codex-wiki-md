<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

We prove [Hall subgroup existence in soluble groups](../../../../../../hall-subgroup-existence-in-soluble-groups.md) by induction on $|G|$. The trivial group is immediate. Choose a nontrivial minimal [normal subgroup](../../../../../../normal-subgroup.md) $N$, [elementary abelian](../../../../../../elementary-abelian-group.md) of order $p^a$ by part (c). Induction gives a Hall $\pi$-subgroup of $G/N$; let $K$ be its full preimage.

If $p\in\pi$, then $K$ itself is the required subgroup. If $p\notin\pi$ and $K<G$, apply induction inside the soluble subgroup $K$ to obtain a Hall $\pi$-subgroup $H$ of $K$. Since $[G:K]$ and $[K:H]$ are both $\pi'$-numbers, $H$ is Hall in $G$ too.

It remains to treat $p\notin\pi$ and $K=G$. Then $G/N$ is a $\pi$-group. If $G=N$, the subgroup one works. Otherwise choose a minimal [normal subgroup](../../../../../../normal-subgroup.md) $M/N$ of $G/N$, an [elementary abelian](../../../../../../elementary-abelian-group.md) $q$-group with $q\in\pi$. Let $Q$ be a Sylow $q$-subgroup of $M$. As $|M|=|N|q^b$ and $p\ne q$, we have $M=NQ$. The permitted [Frattini argument](../../../../../../frattini-argument.md) gives

$$
G=N_G(Q)M=N_G(Q)N.
$$

The last equality uses $Q\leq N_G(Q)$ and the normality of $N$.

If $T=N_G(Q)<G$, then $[G:T]=[N:N\cap T]$ is a power of $p$, hence a $\pi'$-number. Apply induction to $T$ and multiply indices as before. If $T=G$, then $Q$ is a nontrivial normal $\pi$-subgroup. Induction in $G/Q$ gives a Hall $\pi$-subgroup whose full preimage in $G$ is Hall, since its additional factor $|Q|$ is a $\pi$-number. These cases exhaust the possibilities, proving **existence for every prime set**. No unproved complement theorem or conjugacy theorem for Hall subgroups was inserted into the proof.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [1](../../1.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
