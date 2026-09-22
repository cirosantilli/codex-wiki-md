# Subgroup generator bound for a powerful finite p-group

↑ **Parent:** [Powerful p-group](powerful-p-group.md)

For odd $p$, a [subgroup](subgroup.md) $H$ of a finite [powerful p-group](powerful-p-group.md) $G$ satisfies $d(H)\le d(G)$. Here $d$ is the [dimension](dimension-vector-space.md) of the [Frattini quotient](frattini-quotient.md). Set $K=H\cap G^p$, $V=G/G^p$, $W=G^p/G^{p^2}$, and $A=HG^p/G^p$. The onto power map $\theta:V\to W$ sends $A$ into the image of $H^p$ in $K/\Phi(K)$. Since $\Phi(K)\le G^{p^2}$, this image has [dimension](dimension-vector-space.md) at least $\dim\theta(A)$. Also $\Phi(K)\le\Phi(H)\le K$. Induction on $|G|$, applied to the powerful [subgroup](subgroup.md) $G^p$, gives $d(K)\le\dim W$. Consequently

$$
d(H)\le\dim A+\dim W-\dim\theta(A)\le\dim W+\dim\ker\theta=\dim V=d(G).
$$

The last inequality is [rank-nullity theorem](rank-nullity-theorem.md).

## ↑ Ancestors (8)

1. [Powerful p-group](powerful-p-group.md)
2. [Finite p-group](finite-p-group.md)
3. [Finite group theory](finite-group-theory-split.md)
4. [Group theory](group-theory-split.md)
5. [Algebra](algebra-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)
