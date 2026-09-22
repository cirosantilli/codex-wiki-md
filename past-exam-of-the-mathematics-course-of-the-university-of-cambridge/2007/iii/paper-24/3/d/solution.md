<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Use the braid $B=(\sigma_1\sigma_2^{-1})^2$ from part (c). Put meridians $a,b,c$ around its three strands at one end. At a positive crossing, the [Wirtinger presentation](../../../../../../wirtinger-presentation.md) relations induce the [Artin automorphism of a braid](../../../../../../artin-automorphism-of-a-braid.md)

$$
f:\ a\mapsto aba^{-1},\quad b\mapsto a,\quad c\mapsto c.
$$

For the inverse crossing on strands two and three, they give

$$
g:\ a\mapsto a,\quad b\mapsto c,\quad c\mapsto c^{-1}bc.
$$

The first formula is the usual crossing conjugation, and the second is its inverse on the relevant pair. Following one block gives $h=f\circ g$:

$$
h(a)=aba^{-1},\qquad h(b)=c,\qquad h(c)=c^{-1}ac.
$$

The four-crossing braid induces $h^2$. Closing it identifies each ending meridian with its starting meridian. Applying the [Seifert-van Kampen theorem](../../../../../../seifert-van-kampen-theorem.md) to the crossing regions and the closing arcs therefore gives

$$
\pi_1(S^3\setminus K)=\langle a,b,c\mid a=h^2(a),\ b=h^2(b),\ c=h^2(c)\rangle,
$$

where

$$
\begin{aligned}
h^2(a)&=aba^{-1}ca b^{-1}a^{-1},\\
h^2(b)&=c^{-1}ac,\\
h^2(c)&=c^{-1}a^{-1}c\,aba^{-1}c^{-1}ac.
\end{aligned}
$$

Both elementary crossing automorphisms preserve $abc$. Hence $h^2(abc)=abc$, and the first two closure relations imply the third: after substitution $abc=ab\,h^2(c)$, so cancellation gives $c=h^2(c)$.

The first remaining relation can be solved without adding any relation:

$$
a=aba^{-1}ca b^{-1}a^{-1}quad\Longleftrightarrow\quad c=ab^{-1}aba^{-1}.
$$

Substitute this expression into $b=c^{-1}ac$. Free cancellation and multiplying the two sides by inverse words give

$$
ab^{-1}a^{-1}ba=bab^{-1}a^{-1}b.
$$

These are [Tietze transformations](../../../../../../tietze-transformations.md), eliminating a generator defined by one relation and retaining the other. Thus the [figure-eight knot group](../../../../../../figure-eight-knot-group.md) has the requested one-relator presentation

$$
\boxed{\pi_1(S^3\setminus K)\cong
\langle a,b\mid ab^{-1}a^{-1}ba=bab^{-1}a^{-1}b\rangle.}
$$

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 24](../../../paper-24-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
