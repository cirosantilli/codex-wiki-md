<h1 id="5e/solution">Solution</h1>

↑ **Parent:** [5E](../5e.md)

A [group action](../../../../../group-action.md) of $G$ on $X$ is a map $(g,x)\mapsto gx$ such that $ex=x$ and $(gh)x=g(hx)$. The [orbit](../../../../../orbit-of-a-group-action.md) and [stabilizer](../../../../../stabilizer-subgroup.md) of $x$ are

$$
Gx=\{gx:g\in G\},
\qquad
G_x=\{g\in G:gx=x\}.
$$

For a [finite group](../../../../../finite-group.md), the map

$$
gG_x\longmapsto gx
$$

is a well-defined [bijection](../../../../../bijection.md) from the left cosets of $G_x$ to $Gx$. Each coset has $|G_x|$ elements, so the [orbit-stabilizer theorem](../../../../../orbit-stabilizer-theorem.md) is

$$
\boxed{|G|=|Gx|\,|G_x|}.
$$

The [Cauchy theorem for groups](../../../../../cauchy-theorem-for-groups.md) says that if a [prime number](../../../../../prime-number.md) $p$ divides $|G|$, then $G$ has an element of order $p$. To prove it, let

$$
X=\{(g_1,\ldots,g_p)\in G^p:g_1\cdots g_p=e\}.
$$

The first $p-1$ entries determine the last, so $|X|=|G|^{p-1}$, which is divisible by $p$. The [cyclic group](../../../../../cyclic-group.md) $C_p$ acts on $X$ by cyclically rotating the entries; rotation preserves the product condition because

$$
g_2\cdots g_pg_1=g_1^{-1}(g_1\cdots g_p)g_1=e.
$$

Every orbit has size one or $p$. The fixed points are exactly the tuples $(g,\ldots,g)$ with $g^p=e$. Their number is therefore divisible by $p$. Since the identity gives one fixed point, there is another, and its entry has order $p$.

Now let $|G|=33$. Cauchy's theorem gives a subgroup $H$ of order $11$. Let $H$ act by the [conjugation action](../../../../../conjugation-action.md) on the set $\mathcal X$ of subgroups of order $11$. It fixes $H$. If it also fixed $K\ne H$, then $H$ would normalize $K$; since $H\cap K=\{e\}$, the product $HK$ would be a subgroup of order $121$, which is impossible. Every other $H$-orbit in $\mathcal X$ therefore has size $11$, so

$$
|\mathcal X|\equiv1\pmod{11}.
$$

Distinct members of $\mathcal X$ share only the identity and each contributes ten nonidentity elements. Hence $1+10|\mathcal X|\leq33$, forcing $|\mathcal X|=1$. Thus $H$ is a [normal subgroup](../../../../../normal-subgroup.md).

Conjugation now defines a [group homomorphism](../../../../../group-homomorphism.md)

$$
G\longrightarrow\operatorname{Aut}(H).
$$

Because $H\cong C_{11}$, its [automorphism group](../../../../../automorphism-group.md) has order $10$. By the [Lagrange theorem](../../../../../lagrange-s-theorem.md), the image has order dividing both $33$ and $10$, so the image is trivial and $H$ lies in the [center](../../../../../center-of-a-group.md) of $G$. Cauchy's theorem also supplies $x$ of order $3$. If $h$ generates $H$, then $h$ and $x$ commute and $hx$ has order $\operatorname{lcm}(11,3)=33$. Therefore

$$
\boxed{G=\langle hx\rangle\cong C_{33}}.
$$

## ↑ Ancestors (10)

1. [5E](../5e.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
