<h1 id="6e/solution">Solution</h1>

↑ **Parent:** [6E](../6e.md)

A left [group action](../../../../../group-action.md) of $G$ on a set $X$ is a map $(g,x)\mapsto g\cdot x$ satisfying $e\cdot x=x$ and $(gh)\cdot x=g\cdot(h\cdot x)$. The [group orbit](../../../../../orbit-of-a-group-action.md) of $x$ is $G\cdot x=\{g\cdot x:g\in G\}$, and its [stabilizer subgroup](../../../../../stabilizer-subgroup.md) is $G_x=\{g\in G:g\cdot x=x\}$. The [stabilizer subgroup](../../../../../stabilizer-subgroup.md) contains the identity, is closed under products, and contains $g^{-1}$ whenever it contains $g$, so it is indeed a [subgroup](../../../../../subgroup.md).

The [orbit-stabilizer theorem](../../../../../orbit-stabilizer-theorem.md) for a finite [group](../../../../../group-split.md) says

$$
\boxed{|G|=|G\cdot x|\,|G_x|.}
$$

To prove it, map a left [coset](../../../../../coset.md) $gG_x$ to $g\cdot x$. This is well-defined because every element of $G_x$ fixes $x$. Conversely, $g\cdot x=h\cdot x$ precisely when $h^{-1}g\in G_x$, which is precisely equality of the two [cosets](../../../../../coset.md). Thus this map is a [bijection](../../../../../bijection.md) between the [cosets](../../../../../coset.md) and the [group orbit](../../../../../orbit-of-a-group-action.md). Each [coset](../../../../../coset.md) has $|G_x|$ elements, by the [bijection](../../../../../bijection.md) $k\mapsto gk$, and the [cosets](../../../../../coset.md) partition $G$, giving the formula.

Apply this to the [rotational symmetry group of a cube](../../../../../rotational-symmetry-group-of-a-cube.md) acting on its six faces. The action is transitive: rotations through right angles about coordinate axes can send the top face to each of the other faces. A rotation fixing a face must fix its outward normal, so it rotates about the axis through that face's center and the opposite face's center. Preservation of its square boundary permits exactly four angles modulo $2\pi$: $0,\pi/2,\pi,3\pi/2$. All four preserve the cube, so this face [stabilizer subgroup](../../../../../stabilizer-subgroup.md) has order four. The [group](../../../../../group-split.md) is finite because a rotation permutes the six face normals and is determined by their images. The [orbit-stabilizer theorem](../../../../../orbit-stabilizer-theorem.md) gives

$$
\boxed{|\operatorname{Rot}(\text{cube})|=6\times4=24.}
$$

These are orientation-preserving rotations; reflections are not being counted.

## ↑ Ancestors (10)

1. [6E](../6e.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
