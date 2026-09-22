<h1 id="10e/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A [finite nonabelian simple group](../../../../../../finite-nonabelian-simple-group.md) cannot be a [p-group](../../../../../../p-group.md): a nontrivial finite [p-group](../../../../../../p-group.md) has nontrivial [centre of a group](../../../../../../center-of-a-group.md), since its [class equation](../../../../../../class-equation.md) makes every noncentral conjugacy class size divisible by $p$, and hence makes the centre size a positive multiple of $p$. That centre is a [normal subgroup](../../../../../../normal-subgroup.md), so must be the whole group if $G$ is a [simple group](../../../../../../simple-group.md), making it abelian; an abelian [simple group](../../../../../../simple-group.md) has prime order. Therefore every [Sylow subgroup](../../../../../../sylow-subgroup.md) here is nontrivial and proper. It cannot be normal, so $n_p>1$.

To obtain a [simple group embedding from Sylow conjugation](../../../../../../simple-group-embedding-from-sylow-conjugation.md), the [conjugation action on Sylow subgroups](../../../../../../conjugation-action-on-sylow-subgroups.md) gives a [group homomorphism](../../../../../../group-homomorphism.md) $\rho:G\to S_{n_p}$. This [group action](../../../../../../group-action.md) is transitive by the [Sylow theorems](../../../../../../sylow-theorems.md) and is nontrivial since $n_p>1$. Its [kernel of a group homomorphism](../../../../../../kernel-of-a-group-homomorphism.md) is a [normal subgroup](../../../../../../normal-subgroup.md), so the defining property of a [simple group](../../../../../../simple-group.md) makes the [kernel of a group homomorphism](../../../../../../kernel-of-a-group-homomorphism.md) trivial: $\rho$ is an embedding. Now compose with the [sign of a permutation](../../../../../../sign-of-a-permutation.md) $S_{n_p}\to\{\pm1\}$. A nontrivial composite would again be [injective](../../../../../../injective-function.md) because $G$ is a [simple group](../../../../../../simple-group.md), embedding $G$ in a group of order two, impossible for a nonabelian group. Thus $\rho(G)$ lies in the [alternating group](../../../../../../alternating-group.md) $A_{n_p}$. By [Lagrange's theorem](../../../../../../lagrange-s-theorem.md),

$$
\boxed{|G|\mid |A_{n_p}|=\frac{n_p!}{2}}.
$$

The argument only invokes the factorial formula once $n_p\ge2$; the impossible case $n_p=2$ itself is also excluded by the embedding.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [10E](../../10e.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
