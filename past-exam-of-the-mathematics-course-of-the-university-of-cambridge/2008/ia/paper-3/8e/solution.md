<h1 id="8e/solution">Solution</h1>

↑ **Parent:** [8E](../8e.md)

Let a finite [group](../../../../../group-split.md) $G$ act on a set $X$. For $x\in X$, define its [stabilizer subgroup](../../../../../stabilizer-subgroup.md) $G_x=\{g:g\cdot x=x\}$ and its [group orbit](../../../../../orbit-of-a-group-action.md) $Gx=\{g\cdot x:g\in G\}$. The map

$$
gG_x\longmapsto g\cdot x
$$

is well-defined, because multiplying $g$ on the right by an element fixing $x$ does not change its image. It is onto by the definition of the orbit. If $g\cdot x=h\cdot x$, then $h^{-1}g\in G_x$, so $gG_x=hG_x$; hence it is one-to-one. Every [coset](../../../../../coset.md) has $|G_x|$ elements and the [cosets](../../../../../coset.md) partition $G$. This proves the [orbit-stabilizer theorem](../../../../../orbit-stabilizer-theorem.md):

$$
\boxed{|G|=|Gx|\,|G_x|.}
$$

For a [group](../../../../../group-split.md) element $x$, its [cyclic subgroup](../../../../../cyclic-subgroup.md) $H=\langle x\rangle$ has $\operatorname{ord}(x)$ elements. Apply the theorem to the action of $G$ on its left [cosets](../../../../../coset.md) $G/H$, whose stabilizer at $H$ is $H$. It follows that

$$
\boxed{\operatorname{ord}(x)=|H|\text{ divides }|G|.}
$$

This is the needed case of [Lagrange's theorem](../../../../../lagrange-s-theorem.md), obtained directly from the action.

To prove [Cauchy's theorem for finite groups](../../../../../cauchy-theorem-for-groups.md), let $p$ be a prime divisor of $|G|$ and consider

$$
\mathcal X=\{(g_1,\ldots,g_p)\in G^p:g_1\cdots g_p=e\}.
$$

The first $p-1$ entries are arbitrary and determine the last, so $|\mathcal X|=|G|^{p-1}$ is divisible by $p$. Cyclically rotate the entries. This preserves the product constraint even if $G$ is nonabelian, since

$$
g_2\cdots g_pg_1=g_1^{-1}(g_1\cdots g_p)g_1=e.
$$

Thus a [cyclic group](../../../../../cyclic-group.md) of order $p$ acts on $\mathcal X$. By the [orbit-stabilizer theorem](../../../../../orbit-stabilizer-theorem.md), its orbits have size one or $p$. Its fixed tuples are exactly $(g,\ldots,g)$ with $g^p=e$. If $m$ is their number, counting the remaining size-$p$ orbits gives $m\equiv|\mathcal X|\equiv0\pmod p$. The identity provides one fixed tuple, so $m\geq p$ and a nonidentity $g$ with $g^p=e$ exists. The order of this $g$ divides $p$: division of $p$ by its order and minimality of that order prove this directly. Since $p$ is prime and $g\ne e$, the order is exactly $p$. This is the [cyclic-tuple proof of Cauchy theorem](../../../../../cyclic-tuple-proof-of-cauchy-theorem.md).

Now suppose every nonidentity element has order two. Then every element equals its inverse, and for any $a,b\in G$,

$$
ab=(ab)^{-1}=b^{-1}a^{-1}=ba.
$$

Thus [group of exponent two is abelian](../../../../../group-of-exponent-two-is-abelian.md) applies. Starting from the identity [subgroup](../../../../../subgroup.md), choose an element outside the [subgroup](../../../../../subgroup.md) already generated. Because the [group](../../../../../group-split.md) is abelian and that element squares to the identity, adjoining it doubles the [subgroup](../../../../../subgroup.md): it is the disjoint union of the old [subgroup](../../../../../subgroup.md) and its translate by the new element. Repeating until the [finite group](../../../../../finite-group.md) is exhausted shows $|G|=2^r$. Conversely the [direct product of groups](../../../../../direct-product-of-groups.md) $C_2^r$ has order $2^r$ and every nonidentity element has order two. Therefore

$$
\boxed{n=2^r\quad(r=0,1,2,\ldots).}
$$

The case $r=0$ is the trivial [group](../../../../../group-split.md) and satisfies the condition vacuously. These finite examples are [elementary abelian groups](../../../../../elementary-abelian-group.md) of exponent two.

An infinite example is the [group](../../../../../group-split.md) of all binary sequences, with coordinatewise addition modulo two:

$$
\boxed{G=\prod_{j=1}^\infty\mathbb Z/2\mathbb Z.}
$$

Every sequence added to itself is zero, so every nonzero sequence has order exactly two. The sequences having a single $1$ in coordinate $j$ are all distinct, proving that the [group](../../../../../group-split.md) is infinite.

## ↑ Ancestors (10)

1. [8E](../8e.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
