<h1 id="19i/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

By [character orthogonality](../../../../../../character-orthogonality.md), the squared multiplicities are the [character inner product](../../../../../../character-inner-product.md) norm of the [restriction of a character](../../../../../../restriction-of-a-character.md):

$$
\sum_{i=1}^r a_i^2
=\langle\chi\mathbin{\downarrow}_H,\chi\mathbin{\downarrow}_H\rangle_H
=\frac1{|H|}\sum_{h\in H}|\chi(h)|^2.
$$

Since $\chi$ is an [irreducible character](../../../../../../irreducible-character.md), its norm on $G$ is one, and hence

$$
\sum_i a_i^2
\leq\frac1{|H|}\sum_{g\in G}|\chi(g)|^2
=\frac{|G|}{|H|}=[G:H].
$$

The omitted summands are nonnegative, so the [character restriction norm bound](../../../../../../character-restriction-norm-bound.md) is an equality precisely when

$$
\boxed{\chi(g)=0\quad\text{for every }g\in G\setminus H.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [19I](../../19i.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
