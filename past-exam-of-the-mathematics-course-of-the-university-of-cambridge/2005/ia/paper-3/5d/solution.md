<h1 id="5d/solution">Solution</h1>

↑ **Parent:** [5D](../5d.md)

A [group action](../../../../../group-action.md) is a map $(g,x)\mapsto g\cdot x$ from $G\times X$ to $X$ satisfying $e\cdot x=x$ and $(gh)\cdot x=g\cdot(h\cdot x)$. Define the [orbit of a group action](../../../../../orbit-of-a-group-action.md) $Gx=\{g\cdot x:g\in G\}$ and the [stabilizer subgroup](../../../../../stabilizer-subgroup.md) $G_x=\{g:g\cdot x=x\}$. The latter is a [subgroup](../../../../../subgroup.md): the identity fixes $x$, products of elements fixing $x$ fix $x$, and inverses do too.

For finite $G$, the [orbit-stabilizer theorem](../../../../../orbit-stabilizer-theorem.md) states

$$
\boxed{|Gx|=\frac{|G|}{|G_x|}.}
$$

To prove it, send a left [coset](../../../../../coset.md) $gG_x$ to $g\cdot x$. If $gG_x=hG_x$, then $h^{-1}g\in G_x$ and $g\cdot x=h\cdot x$. Conversely, equality of the two images implies $h^{-1}g\in G_x$, hence equality of the [cosets](../../../../../coset.md). Every point of the [orbit of a group action](../../../../../orbit-of-a-group-action.md) has such a preimage. This is therefore a [bijection](../../../../../bijection.md), and each [coset](../../../../../coset.md) has $|G_x|$ elements, proving the formula.

For the action on [subgroups](../../../../../subgroup.md), conjugation maps a [subgroup](../../../../../subgroup.md) $K$ to a [subgroup](../../../../../subgroup.md) $gKg^{-1}$ because it preserves products and inverses. Furthermore $eKe^{-1}=K$ and

$$
(gh)K(gh)^{-1}=g(hKh^{-1})g^{-1}.
$$

Thus this is the [conjugation action](../../../../../conjugation-action.md). The [stabilizer subgroup](../../../../../stabilizer-subgroup.md) of $H$ is its [normalizer](../../../../../normalizer.md) $N_G(H)$, and $H\subseteq N_G(H)$ since each $h\in H$ conjugates $H$ onto itself. Hence the number $k$ of distinct [conjugate subgroups](../../../../../conjugate-subgroup.md) is

$$
k=\frac{|G|}{|N_G(H)|}\leq\frac{|G|}{|H|}.
$$

Now suppose $H$ is proper. Put $m=|G|/|H|\geq2$ and list the $k$ distinct [conjugate subgroups](../../../../../conjugate-subgroup.md) as $H_1,\ldots,H_k$. Each has $|H|$ elements and all contain the same identity. Counting the identity just once, even if other elements overlap, gives

$$
\left|\bigcup_{i=1}^kH_i\right|
\leq1+k(|H|-1)
\leq1+m(|H|-1)
=|G|-m+1<|G|.
$$

Thus **some element of $G$ lies in no conjugate of $H$**. This proves [conjugates of a proper subgroup do not cover a finite group](../../../../../conjugates-of-a-proper-subgroup-do-not-cover-a-finite-group.md) by an explicit count; it does not require the conjugates to intersect only at the identity.

## ↑ Ancestors (10)

1. [5D](../5d.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
