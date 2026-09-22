<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [cyclotomic extension of a p-adic field](../../../../../../cyclotomic-extension-of-a-p-adic-field.md)

$$
L_1=\mathbb Q_p(\zeta_p)
$$

has degree $p-1$, is Galois with group $(\mathbb Z/p\mathbb Z)^\times$, and is [totally ramified](../../../../../../totally-ramified-extension.md). Indeed, $\zeta_p-1$ is a root of the [Eisenstein polynomial](../../../../../../eisenstein-polynomial.md)

$$
\frac{(X+1)^p-1}{X}.
$$

Put $\alpha=\sqrt[p-1]{-p}$. Its polynomial $X^{p-1}+p$ is Eisenstein, so $L_2=\mathbb Q_p(\alpha)$ is totally ramified of degree $p-1$. Every $(p-1)$st root of unity lies in $\mathbb Q_p$ by the [Teichmuller lifts](../../../../../../teichmuller-representative.md), so every root $\omega\alpha$ of this polynomial lies in $L_2$. Hence $L_2/\mathbb Q_p$ is also [Galois](../../../../../../finite-galois-extension.md).

For either $L_i/\mathbb Q_p$, the norm has every possible valuation because the [residue-field degree](../../../../../../residue-field-degree.md) is one. The [norm units in a tamely totally ramified extension](../../../../../../norm-units-in-a-tamely-totally-ramified-extension.md) lie in the principal units $1+p\mathbb Z_p$: reduction of a unit norm is the $(p-1)$st power of its residue, hence is $1$. Part (b) says that this unit norm subgroup has index $p-1$, exactly the index of $1+p\mathbb Z_p$ in $\mathbb Z_p^\times$. Consequently

$$
N_{L_1/\mathbb Q_p}(L_1^\times)
=p^{\mathbb Z}(1+p\mathbb Z_p)
=N_{L_2/\mathbb Q_p}(L_2^\times).
$$

The uniqueness clause in the [existence theorem of local class field theory](../../../../../../existence-theorem-of-local-class-field-theory.md) now gives

$$
\boxed{L_1=L_2.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 136](../../../paper-136-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
