<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

A finite [minimal normal subgroup](../../../../../../minimal-normal-subgroup.md) is a [characteristically simple group](../../../../../../characteristically-simple-group.md), and has the [direct-product structure of a finite minimal normal subgroup](../../../../../../direct-product-structure-of-a-finite-minimal-normal-subgroup.md)

$$
N=T_1\times\cdots\times T_k
$$

with isomorphic [simple groups](../../../../../../simple-group.md) $T_i$. For completeness, choose a minimal nontrivial [normal subgroup](../../../../../../normal-subgroup.md) $T$ of $N$. Its distinct $G$-conjugates are [minimal normal subgroups](../../../../../../minimal-normal-subgroup.md) of $N$, so they centralize one another. Their product is normal in $G$, hence equals $N$. If $T$ is abelian the product is abelian and minimal primary [characteristic subgroups](../../../../../../characteristic-subgroup.md) make $N$ elementary abelian. Otherwise each $T$ has trivial center: its center is a [characteristic subgroup](../../../../../../characteristic-subgroup.md) of $T$, hence normal in $N$, and minimality would make $T$ abelian. Each new conjugate then meets the product of previous conjugates trivially, because it centralizes that product and is centerless. The product is direct. Every [normal subgroup](../../../../../../normal-subgroup.md) of a direct factor is normal in $N$, so minimality of that factor makes it simple.

Assume now that $N$ acts primitively and nonregularly. Any nontrivial [normal subgroup](../../../../../../normal-subgroup.md) of this faithful primitive action is transitive. Thus each $T_i$ is transitive. If $k\ge2$, the transitive commuting [groups](../../../../../../group-split.md) $T_1$ and $T_2$ are regular: an element of one fixing $\alpha$ commutes with the other and hence fixes its entire orbit. But the [centralizer](../../../../../../centralizer.md) of a regular [group](../../../../../../group-split.md) has order $n$, as its elements are determined by the [image](../../../../../../image-of-a-function.md) of $\alpha$. Therefore all remaining factors lie in the order-n [centralizer](../../../../../../centralizer.md) of $T_1$, and the transitive [group](../../../../../../group-split.md) $T_2$ already fills it. There can be only two factors, with $|N|=n^2$. Now $|N_\alpha|=n$, whereas its common nontrivial subdegree $r$ divides both $n$ and $n-1$. Hence $r=1$, making $N_\alpha$ trivial, a contradiction. Thus $k=1$, and $N$ is simple. An abelian transitive [group](../../../../../../group-split.md) is regular, so $N$ is nonabelian.

Finally $C_G(N)$ is normal in the primitive [group](../../../../../../group-split.md) $G$. If nontrivial it would be transitive, and commuting with transitive $N$ would force $N$ regular. Thus $C_G(N)=1$, and [conjugation](../../../../../../conjugation.md) embeds $G$ in $\operatorname{Aut}(N)$. The centerless simple [group](../../../../../../group-split.md) $N$ is identified with its [inner automorphism group](../../../../../../inner-automorphism.md). Therefore

$$
\boxed{N\text{ is nonabelian simple},\qquad N\le G\le\operatorname{Aut}(N).}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
