<h1 id="11g/solution">Solution</h1>

↑ **Parent:** [11G](../11g.md)

An [R-module](../../../../../primary-submodule.md) $M$ is a [free module](../../../../../free-module.md) if it has a basis $(e_i)_{i\in I}$: every $m\in M$ has a unique expression as a finite sum $\sum_i r_ie_i$, with $r_i\in R$. Equivalently, it is a [direct sum](../../../../../direct-sum.md) of copies of $R$. Let $q:M\to M/N$ be the quotient map. When $M/N$ is free, choose a basis $(\overline f_j)$ and lifts $f_j\in M$. The [universal property of a free module](../../../../../universal-property-of-a-free-module.md) defines an $R$-linear map $s:M/N\to M$ by $s(\sum_jr_j\overline f_j)=\sum_jr_jf_j$. It satisfies $q\circ s=\operatorname{id}$, so every $m\in M$ decomposes uniquely as

$$
m=\bigl(m-s(q(m))\bigr)+s(q(m)),\qquad m-s(q(m))\in N.
$$

This gives a [split short exact sequence](../../../../../split-short-exact-sequence.md) and $M\cong N\oplus(M/N)$. If $N$ is also free, the union of its basis and the lifted quotient basis is a basis of $M$: spanning follows from the decomposition, and applying $q$ to a putative relation kills all quotient coefficients before independence in $N$ kills the remaining ones. Thus **free submodule and free quotient imply a free module**.

For the first claim, take $R=\mathbb Z$ and

$$
M=\mathbb Z,\quad N=2\mathbb Z,\qquad M'=\mathbb Z\oplus\mathbb Z/2\mathbb Z,\quad N'=\mathbb Z\oplus\{0\}.
$$

Here $N\cong N'\cong\mathbb Z$ are [free modules](../../../../../free-module.md) and $M/N\cong M'/N'\cong\mathbb Z/2\mathbb Z$. But $M$ is a [torsion-free module](../../../../../torsion-free-module.md), whereas $M'$ contains the nonzero [torsion element](../../../../../torsion-element.md) $(0,\overline1)$. Therefore **claim (1) is false**.

For the second claim, the same lifting construction works without assuming that $N$ is free. Since both isomorphic [quotient modules](../../../../../quotient-module.md) are free, it yields

$$
M\cong N\oplus(M/N)\cong N'\oplus(M'/N')\cong M'.
$$

Thus **claim (2) is true**. Equivalently, this uses the fact that [free modules are projective](../../../../../free-modules-are-projective.md).

## ↑ Ancestors (10)

1. [11G](../11g.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
