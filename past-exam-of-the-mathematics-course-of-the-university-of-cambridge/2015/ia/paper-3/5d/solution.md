<h1 id="5d/solution">Solution</h1>

↑ **Parent:** [5D](../5d.md)

A left [group action](../../../../../group-action.md) is a map $(g,x)\mapsto g\cdot x$ with $e\cdot x=x$ and $(gh)\cdot x=g\cdot(h\cdot x)$. The [group orbit](../../../../../orbit-of-a-group-action.md) and [stabiliser subgroup](../../../../../stabilizer-subgroup.md) are

$$
\operatorname{Orb}(x)=\{g\cdot x:g\in G\},\qquad G_x=\{g\in G:g\cdot x=x\}.
$$

The identity belongs to $G_x$. If $g,h\in G_x$, then $(gh)\cdot x=g\cdot x=x$; also $g^{-1}\cdot x=g^{-1}\cdot(g\cdot x)=x$. Thus $G_x$ is a [subgroup](../../../../../subgroup.md).

For the [orbit-stabilizer theorem](../../../../../orbit-stabilizer-theorem.md), the map $gG_x\mapsto g\cdot x$ from left [cosets](../../../../../coset.md) to the [group orbit](../../../../../orbit-of-a-group-action.md) is a bijection: $g\cdot x=h\cdot x$ if and only if $h^{-1}g\in G_x$, which is precisely $gG_x=hG_x$. Each left [coset](../../../../../coset.md) has $|G_x|$ elements, since multiplication by $g$ is a bijection from $G_x$ to $gG_x$, and the left [cosets](../../../../../coset.md) partition $G$. For finite $G$ this proves

$$
\boxed{|G|=|G_x|\,|\operatorname{Orb}(x)|.}
$$

## ↑ Ancestors (10)

1. [5D](../5d.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
