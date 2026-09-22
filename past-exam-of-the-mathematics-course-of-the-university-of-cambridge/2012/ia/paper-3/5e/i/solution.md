<h1 id="5e/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For a [group action](../../../../../../group-action.md) of $G$ on $X$, let $G_x=\{g:gx=x\}$ be the [stabilizer subgroup](../../../../../../stabilizer-subgroup.md) of $x$, and $Gx$ its [group orbit](../../../../../../orbit-of-a-group-action.md). The [orbit-stabilizer theorem](../../../../../../orbit-stabilizer-theorem.md) is the [bijection](../../../../../../bijection.md)

$$
G/G_x\longrightarrow Gx,\qquad gG_x\longmapsto gx.
$$

It is well defined because elements in the same left [coset](../../../../../../coset.md) differ by an element fixing $x$. Conversely, $gx=hx$ implies $h^{-1}g\in G_x$, so the [cosets](../../../../../../coset.md) coincide. Surjectivity is the definition of the [group orbit](../../../../../../orbit-of-a-group-action.md). For a [finite group](../../../../../../finite-group.md), counting the [cosets](../../../../../../coset.md) gives

$$
\boxed{|G|=|Gx|\,|G_x|.}
$$

To obtain [Cayley theorem](../../../../../../cayley-s-theorem.md), let $G$ act on its own underlying set by left multiplication. The map $\lambda_g:x\mapsto gx$ is a [permutation](../../../../../../permutation.md), with inverse $\lambda_{g^{-1}}$, and $\lambda_g\lambda_h=\lambda_{gh}$. If $\lambda_g$ is the identity [permutation](../../../../../../permutation.md), evaluating at the identity element gives $g=e$. Thus $g\mapsto\lambda_g$ is an injective [group homomorphism](../../../../../../group-homomorphism.md). When $|G|=n$, labeling this set by $n$ letters identifies its image with a [subgroup](../../../../../../subgroup.md) of $S_n$. **Every finite group embeds in the symmetric group on its own elements.**

## ↑ Ancestors (11)

1. [I](../i.md)
2. [5E](../../5e.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ia](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
