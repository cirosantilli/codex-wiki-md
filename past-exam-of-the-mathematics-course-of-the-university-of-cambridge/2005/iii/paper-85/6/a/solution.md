<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

This part proves $(c)\Rightarrow(a)$. Write the [Weyl algebra](../../../../../../weyl-algebra.md) generators as $x_1,\ldots,x_n,D_1,\ldots,D_n$, with $[D_i,x_j]=\delta_{ij}$ and the other generator [commutators](../../../../../../commutator.md) zero. The ordered [monomials](../../../../../../monomial.md) $x^\alpha D^\beta$ form a [basis](../../../../../../basis.md) over any [field](../../../../../../field.md): one may construct the [algebra](../../../../../../algebra-split.md) by successively adjoining the commuting derivations $D_i$ to $k[x_1,\ldots,x_n]$, with multiplication $D_if=fD_i+\partial f/\partial x_i$, obtaining unique ordered forms. This also makes $A_n(k)$ infinite-dimensional for $n\ge1$.

Assume $\operatorname{char}k=0$ and let $I$ be a nonzero two-sided [ideal](../../../../../../ideal.md). Choose a nonzero element $a=\sum c_{\alpha\beta}x^\alpha D^\beta\in I$, and a nonzero term of maximal total degree, say $(\alpha_0,\beta_0)$. The relations give

$$
[D_i,x^\alpha D^\beta]=\alpha_i x^{\alpha-e_i}D^\beta,\qquad
[x_i,x^\alpha D^\beta]=-\beta_i x^\alpha D^{\beta-e_i}.
$$

Apply $(\operatorname{ad}D)^{\alpha_0}(\operatorname{ad}x)^{\beta_0}$ to $a$. Every lower-degree term vanishes. A term of the same degree survives only if all its exponents dominate $(\alpha_0,\beta_0)$, which forces equality. Thus the resulting element of $I$ is

$$
(-1)^{|\beta_0|}\alpha_0!\beta_0!c_{\alpha_0\beta_0}\ne0.
$$

The factorials are nonzero in characteristic zero. This is a nonzero [scalar](../../../../../../scalar.md), so $1\in I$ and $I=A_n(k)$. Therefore **$A_n(k)$ is simple in characteristic zero**. This [scalar extraction by iterated Weyl commutators](../../../../../../scalar-extraction-by-iterated-weyl-commutators.md) supplies the full simplicity proof.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [6](../../6.md)
3. [Paper 85](../../../paper-85-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
