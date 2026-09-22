<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $L=\mathbb Q(\alpha)$, where $\alpha$ is an [algebraic integer](../../../../../../algebraic-integer.md) with monic [minimal polynomial](../../../../../../minimal-polynomial.md) $f\in\mathbb Z[X]$, and put $I=[\mathcal O_L:\mathbb Z[\alpha]]$. The [Kummer-Dedekind theorem](../../../../../../kummer-dedekind-theorem.md) applies to a [prime number](../../../../../../prime-number.md) $p$ with $p\nmid I$. Write its reduction as a product of [polynomial factors](../../../../../../polynomial-factor.md) over $\mathbb F_p$:

$$
\overline f=\prod_{j=1}^r g_j^{e_j},
$$

where the $g_j$ are distinct monic [irreducible polynomials](../../../../../../irreducible-polynomial.md), choose monic integral lifts $G_j$. Then the distinct [prime ideals](../../../../../../prime-ideal.md) above $p$ are $\mathfrak p_j=(p,G_j(\alpha))$, and

$$
\boxed{p\mathcal O_L=\prod_{j=1}^r\mathfrak p_j^{e_j},\qquad f(\mathfrak p_j/p)=\deg g_j.}
$$

Thus the multiplicity of a factor is its [ramification index of a prime ideal](../../../../../../ramification-index-of-a-prime-ideal.md), and its degree is the [residue degree](../../../../../../residue-degree.md). The hypothesis on the [order in a number field](../../../../../../order-in-a-number-field.md) is essential: one cannot infer [prime ideal factorization](../../../../../../prime-ideal-factorization.md) from an arbitrary defining polynomial at a prime dividing its index. There is also a relative version over a base [number field](../../../../../../number-field.md) $K$: if $\mathcal O_L$ and $\mathcal O_K[\alpha]$ agree after localization at $\mathfrak p$, factor the [minimal polynomial](../../../../../../minimal-polynomial.md) over $\mathcal O_K/\mathfrak p$ and use $(\mathfrak p,G_j(\alpha))$ with the same conclusions.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 32](../../../paper-32-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
