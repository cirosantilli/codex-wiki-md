<h1 id="2c/solution">Solution</h1>

↑ **Parent:** [2C](../2c.md)

A family $x_1,\ldots,x_n$ is [linearly independent](../../../../../linear-independence.md) if $\sum_{i=1}^n a_ix_i=0$ forces $a_1=\cdots=a_n=0$. For the three specified vectors, direct substitution gives

$$
\boxed{4x_1-3x_2-2x_3=0.}
$$

The coefficients are not all zero, so **the vectors are linearly dependent**.

For the implication question, using the usual interpretation that a [basis](../../../../../basis.md) contains the listed family as independent entries, the answers in order (i)–(x) are

$$
\boxed{\mathrm T,\ \mathrm T,\ \mathrm F,\ \mathrm F,\ \mathrm T,\ \mathrm F,\ \mathrm T,\ \mathrm T,\ \mathrm T,\ \mathrm T.}
$$

The key distinctions are that the unrestricted zero combination always exists, whereas [linear dependence](../../../../../linear-dependence.md) requires a nontrivial combination; and dependence does not necessarily let the specified third vector be solved in terms of the first two. For example $x=y=e_1$, $z=e_2$ makes (iii) and (iv) false, while $x=e_1,y=e_2,z=e_3$ disproves (vi).

There is a set-versus-family qualification in (v). If “contains” is interpreted as literal set containment, repeated nonzero vectors need only occur once in the [basis](../../../../../basis.md). Then $x=y=e_1,z=e_2$ is dependent as a family but all three belong to the basis $\{e_1,e_2\}$, so (v) becomes false. With three distinct vectors, or with family-containment as above, [basis extension](../../../../../basis-extension.md) gives (v) true. Implication (x) remains true on either reading.

## ↑ Ancestors (10)

1. [2C](../2c.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ia](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
