<h1 id="19h/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Burnside lemma](../../../../../../burnside-s-lemma.md) states that for a finite group $G$ acting on a finite set $X$,

$$
|X/G|=\frac1{|G|}\sum_{g\in G}|X^g|.
$$

To prove it, count

$$
\Omega=\{(g,x)\in G\times X:gx=x\}.
$$

Counting by $g$ gives $\sum_g|X^g|$. Counting by $x$ gives

$$
\sum_{x\in X}|G_x|
=\sum_{\mathcal O}|{\mathcal O}|\,|G_x|
=\sum_{\mathcal O}|G|
=|G|\,|X/G|,
$$

using the orbit-stabilizer theorem on each orbit $\mathcal O$. Dividing by $|G|$ proves the formula.

Let $\pi$ be the character of the [permutation representation](../../../../../../permutation-representation.md) $\mathbb C[X]$. Then $\pi(g)=|X^g|$, and a second application of Burnside's lemma gives

$$
\langle\pi,\pi\rangle_G
=\frac1{|G|}\sum_g|X^g|^2
=\#(G\backslash(X\times X)).
$$

For a two-transitive action there are exactly two orbits on $X\times X$: the diagonal and the ordered pairs of distinct points. Hence $\langle\pi,\pi\rangle=2$. Transitivity says the trivial representation occurs once. Since the squared multiplicities of the irreducible constituents sum to two, there is exactly one further constituent, with multiplicity one, and it is irreducible and nontrivial. Thus

$$
\boxed{\mathbb C[X]\cong\mathbf1\oplus V}
$$

as in the [permutation representation of a two-transitive action](../../../../../../permutation-representation-of-a-two-transitive-action.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [19H](../../19h.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
