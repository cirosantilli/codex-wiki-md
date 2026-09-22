<h1 id="vieta-s-formulas">Vieta's formulas</h1>

↑ **Parent:** [Polynomial](polynomial-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Vieta's_formulas)

[Vieta's formulas](vieta-s-formulas.md) connect two descriptions of a [polynomial](polynomial-split.md): its [coefficients](coefficient.md) and its [roots of a polynomial](root-of-a-polynomial.md). They let us read the [sum](sum.md) and [product](product-of-numbers.md) of the [roots of a polynomial](root-of-a-polynomial.md) without finding the individual [roots of a polynomial](root-of-a-polynomial.md), and turn a proposed [factorization of polynomials](factorization-of-polynomials.md) into checkable [coefficient](coefficient.md) identities. The key is that [coefficients](coefficient.md) encode [elementary symmetric polynomials](elementary-symmetric-polynomial.md), which are unchanged by a [permutation](permutation.md) of the [roots of a polynomial](root-of-a-polynomial.md).

For a [polynomial](polynomial-split.md) of [polynomial degree](degree-of-a-polynomial.md) $n\geq1$, with nonzero [leading coefficient](leading-coefficient-of-a-polynomial.md) $a_n$, write its [factorization of polynomials](factorization-of-polynomials.md) in a [splitting field](splitting-field.md) as

$$
p(x)=a_nx^n+a_{n-1}x^{n-1}+\cdots+a_0
=a_n\prod_{i=1}^n(x-r_i).
$$

List every [root of a polynomial](root-of-a-polynomial.md) according to its [multiplicity of a root](multiplicity-of-a-root.md). Then

$$
\boxed{e_k(r_1,\ldots,r_n)=(-1)^k\frac{a_{n-k}}{a_n},\qquad 0\leq k\leq n.}
$$

In particular, $\sum_i r_i=-a_{n-1}/a_n$ and $\prod_i r_i=(-1)^na_0/a_n$. With [coefficients](coefficient.md) in the [real numbers](real-number.md) or [complex numbers](complex-number.md), the [fundamental theorem of algebra](fundamental-theorem-of-algebra.md) ensures that a list of $n$ [roots of a polynomial](root-of-a-polynomial.md) in the [complex numbers](complex-number.md) exists when [multiplicity of a root](multiplicity-of-a-root.md) is counted.[NIST Digital Library of Mathematical Functions; §1.11(ii), root multiplicity paragraph and equation 1.11.10](nist-digital-library-of-mathematical-functions/1-algebraic-and-analytic-methods.md)

For a [monic polynomial](monic-polynomial.md), this is the familiar convention

$$
X^n+c_1X^{n-1}+\cdots+c_n=\prod_{i=1}^n(X-r_i),
$$

where $(-1)^kc_k$ is the $k$th [elementary symmetric polynomial](elementary-symmetric-polynomial.md) in the [roots of a polynomial](root-of-a-polynomial.md); in particular, $\prod_i r_i=(-1)^nc_n$. The ratio by $a_n$ in the general statement matters: multiplying every [coefficient](coefficient.md) by the same nonzero [scalar](scalar.md) preserves both the [roots of a polynomial](root-of-a-polynomial.md) and these ratios.

A short derivation explains every alternating sign. In the [product](product-of-numbers.md) $\prod_i(x-r_i)$, a term of [polynomial degree](degree-of-a-polynomial.md) $n-k$ arises by choosing $-r_i$ from $k$ distinct factor positions and $x$ from the others. Summing the resulting [products](product-of-numbers.md) gives $(-1)^ke_k$. Values at different positions may coincide: the selection is of positions, not distinct root values. Matching [coefficients](coefficient.md) gives the formula. This is the [distributive property](distributive-property.md) organized by the number of chosen root factors.

**Table of contents**

- [Vieta formulas for a cubic](vieta-formulas-for-a-cubic.md)
- [Repeated roots in Vieta's formulas](repeated-roots-in-vieta-s-formulas.md)
- [Complex conjugate roots in Vieta's formulas](complex-conjugate-roots-in-vieta-s-formulas.md)
- [History of Vieta's formulas](history-of-vieta-s-formulas.md)

## ↑ Ancestors (5)

1. [Polynomial](polynomial-split.md)
2. [Algebra](algebra-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Vieta's formulas](vieta-s-formulas.md)
