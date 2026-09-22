<h1 id="19i/solution">Solution</h1>

↑ **Parent:** [19I](../19i.md)

The [row orthogonality relations for a character table](../../../../../row-orthogonality-relations-for-a-character-table.md) state that for irreducible characters $\chi,\psi$,

$$
\boxed{\sum_{g\in G}\chi(g)\overline{\psi(g)}
=|G|\delta_{\chi\psi}.}
$$

Equivalently, if $c$ runs through representatives of the conjugacy classes $C$,

$$
\sum_C|C|\chi(c)\overline{\psi(c)}
=|G|\delta_{\chi\psi}.
$$

Fix an irreducible $\chi$. The sum of the elements in a conjugacy class $C$ is central in $\mathbb CG$, so [Schur lemma](../../../../../schur-s-lemma.md) says that it acts in the representation affording $\chi$ by the scalar

$$
\omega_\chi(C)=\frac{|C|\chi(c)}{\chi(1)}.
$$

This [central character value of a conjugacy-class sum](../../../../../central-character-value-of-a-conjugacy-class-sum.md) is an [algebraic integer](../../../../../algebraic-integer.md): the class sum acts by a matrix with integer entries on the [regular representation](../../../../../regular-representation.md), and $\omega_\chi(C)$ is one of its eigenvalues. Also $\overline{\chi(c)}$ is an algebraic integer because character values are sums of roots of unity.

Row orthogonality with $\psi=\chi$ now gives

$$
\frac{|G|}{\chi(1)}
=\sum_C
\frac{|C|\chi(c)}{\chi(1)}\overline{\chi(c)}
=\sum_C\omega_\chi(C)\overline{\chi(c)}.
$$

The right-hand side is an algebraic integer. The left-hand side is rational, and every rational algebraic integer is an integer. Therefore

$$
\boxed{\chi(1)\mid|G|.}
$$

## ↑ Ancestors (10)

1. [19I](../19i.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
