<h1 id="19i/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Mackey's theorem](../../../../../../mackey-restriction-formula.md), or Mackey restriction formula, says that if $H,K\leq G$, $W$ is a complex $K$-representation, and $D$ is a set of representatives for the [double cosets](../../../../../../double-coset.md) $H\backslash G/K$, then

$$
\boxed{
\operatorname{Res}_H^G\operatorname{Ind}_K^G W
\cong
\bigoplus_{x\in D}
\operatorname{Ind}_{H\cap xKx^{-1}}^H
\operatorname{Res}_{H\cap xKx^{-1}}^{xKx^{-1}}({}^xW).}
$$

Here ${}^xW$ is the representation of the [conjugate subgroup](../../../../../../conjugate-subgroup.md) $xKx^{-1}$ defined by

$$
{}^xW(xkx^{-1})=W(k).
$$

For the proof, use the group-algebra model

$$
\operatorname{Ind}_K^G W
=\mathbb C[G]\otimes_{\mathbb C[K]}W.
$$

The partition of $G$ into double cosets gives the direct-sum decomposition of $(H,K)$-bimodules

$$
\mathbb C[G]
=\bigoplus_{x\in D}\mathbb C[HxK].
$$

Put $L_x=H\cap xKx^{-1}$. For each $x$, define

$$
T_x:
\mathbb C[H]\otimes_{\mathbb C[L_x]}{}^xW
\longrightarrow
\mathbb C[HxK]\otimes_{\mathbb C[K]}W,
\qquad
h\otimes w\longmapsto hx\otimes w.
$$

If $\ell=xkx^{-1}\in L_x$, then

$$
T_x(h\ell\otimes w)
=h\ell x\otimes w
=hxk\otimes w
=hx\otimes kw
=T_x(h\otimes\ell w),
$$

so $T_x$ is well defined. It is visibly $H$-equivariant and surjective, and choosing representatives for $H/L_x$ shows that both sides have dimension $[H:L_x]\dim W$; hence it is an isomorphism. Summing the $T_x$ proves the formula.

The [Frobenius reciprocity](../../../../../../frobenius-reciprocity.md) theorem states that for an $H$-representation $U$ and a $G$-representation $V$,

$$
\boxed{
\operatorname{Hom}_G(\operatorname{Ind}_H^G U,V)
\cong
\operatorname{Hom}_H(U,\operatorname{Res}_H^G V).}
$$

For the corresponding [character of a representation](../../../../../../character-of-a-representation.md), this is

$$
\boxed{
\langle\operatorname{Ind}_H^G\chi,\psi\rangle_G
=\langle\chi,\operatorname{Res}_H^G\psi\rangle_H.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [19I](../../19i.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
