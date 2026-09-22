<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $T=R\setminus P$. Since $P$ is a [prime ideal](../../../../../../prime-ideal.md), $T$ is a [multiplicative subset](../../../../../../multiplicatively-closed-set.md) containing $1$ and excluding $0$. The [localization at a prime ideal](../../../../../../localization-at-a-prime-ideal.md) is

$$
\boxed{R_P=T^{-1}R.}
$$

Concretely, its elements are equivalence classes of pairs $(r,s)\in R\times T$, written $r/s$, with

$$
\frac r s=\frac {r'}{s'}\quad\Longleftrightarrow\quad
u(s'r-sr')=0\text{ for some }u\in T.
$$

This extra multiplier is essential when $R$ has [zero divisors](../../../../../../zero-divisor.md). Addition and multiplication are

$$
\frac r s+\frac {r'}{s'}=\frac{rs'+r's}{ss'},\qquad
\frac r s\frac {r'}{s'}=\frac{rr'}{ss'}.
$$

The equivalence criterion is compatible with these operations: after multiplying by the multipliers witnessing changes of representatives, the corresponding numerators agree. The [commutative ring](../../../../../../commutative-ring.md) axioms follow from those of $R$; the identity is $1/1$.

The canonical [ring homomorphism](../../../../../../ring-homomorphism.md) $\iota:R\to R_P$, $r\mapsto r/1$, supplies the [algebra over a commutative ring](../../../../../../algebra-over-a-commutative-ring.md) structure, with scalar action $a(r/s)=ar/s$. It also has the [universal property of localization](../../../../../../universal-property-of-localization.md): whenever a [ring homomorphism](../../../../../../ring-homomorphism.md) $\psi:R\to A$ sends $T$ to [units](../../../../../../unit-in-a-ring.md), the unique extension is $r/s\mapsto\psi(r)\psi(s)^{-1}$.

For later use, $R_P$ is a [local ring](../../../../../../local-ring.md) with [maximal ideal](../../../../../../maximal-ideal.md) $PR_P$. Reduction of numerators and denominators gives a surjective [ring homomorphism](../../../../../../ring-homomorphism.md) $R_P\to\operatorname{Frac}(R/P)$ with kernel $PR_P$, so this [ideal](../../../../../../ideal.md) is proper and maximal. Every fraction outside it has numerator outside $P$ and is a [unit](../../../../../../unit-in-a-ring.md), with inverse $s/r$. Thus it is the unique [maximal ideal](../../../../../../maximal-ideal.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 101](../../../paper-101-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
