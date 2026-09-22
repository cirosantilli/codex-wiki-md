<h1 id="19h/solution">Solution</h1>

↑ **Parent:** [19H](../19h.md)

[Maschke's theorem](../../../../../maschke-s-theorem.md) says that every invariant subspace of a finite-dimensional complex representation of a finite group has an invariant complement. Average any projection over the group to make it equivariant. Induction on dimension therefore decomposes every representation into irreducibles.

The [character of a representation](../../../../../character-of-a-representation.md) is $\chi_V(g)=\operatorname{tr}(g|_V)$. For a $G$-set $X$, the permutation representation $\mathbb CX$ has basis $X$, and its character is the number of fixed points:

$$
\chi_{\mathbb CX}(g)=|X^g|.
$$

For the regular action,

$$
\chi_{\mathbb CG}(1)=|G|,
\qquad \chi_{\mathbb CG}(g)=0\quad(g\ne1).
$$

The multiplicity of an irreducible $V_i$ is the character inner product

$$
\langle\chi_{\rm reg},\chi_i\rangle
=\chi_i(1)=\dim V_i,
$$

so

$$
\boxed{\mathbb CG\cong\bigoplus_i(\dim V_i)V_i}.
$$

If $V\cong\bigoplus_i n_iV_i$, [Schur lemma](../../../../../schur-s-lemma.md) gives

$$
\boxed{\dim\operatorname{Hom}_G(V,V)=\sum_i n_i^2}.
$$

For $V=\mathbb CG$, this is $\sum_i(\dim V_i)^2=|G|$.

Now suppose $\chi(g)=0$ off the identity. The multiplicity of $V_i$ in $V$ is

$$
\langle\chi,\chi_i\rangle
=\frac{\dim V}{|G|}\dim V_i.
$$

Thus $\dim V/|G|$ is a nonnegative integer and $V$ is that many copies of the regular representation. Finally,

$$
\chi_{W\otimes\mathbb CG}(g)
=\chi_W(g)\chi_{\rm reg}(g)
=(\dim W)\chi_{\rm reg}(g),
$$

so

$$
\boxed{W\otimes\mathbb CG\cong(\dim W)\mathbb CG}.
$$

## ↑ Ancestors (10)

1. [19H](../19h.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
