<h1 id="18g/solution">Solution</h1>

↑ **Parent:** [18G](../18g.md)

An element $x$ of an extension $L/K$ is an [algebraic element](../../../../../algebraic-element.md) over $K$ when some nonzero [polynomial](../../../../../polynomial-split.md) in $K[t]$ vanishes at $x$. Let its monic [minimal polynomial](../../../../../minimal-polynomial.md) have degree $d$. [Polynomial](../../../../../polynomial-split.md) division shows $K[x]$ is spanned by $1,x,\ldots,x^{d-1}$, and minimality makes these [vectors](../../../../../vector.md) independent. The [minimal polynomial](../../../../../minimal-polynomial.md) is irreducible; for any nonzero $q(x)$, Bezout's identity between $q$ and that [polynomial](../../../../../polynomial-split.md) gives a [polynomial](../../../../../polynomial-split.md) representative for $q(x)^{-1}$. Thus $K[x]$ is a field, equals $K(x)$, and has degree $d$.

Conversely, if $K(x)$ has finite vector-space [dimension](../../../../../dimension-vector-space.md) $d$, then $1,x,\ldots,x^d$ are linearly dependent over $K$, giving a nonzero annihilating [polynomial](../../../../../polynomial-split.md). Hence

$$
\boxed{x\text{ algebraic over }K\ \Longleftrightarrow\ [K(x):K]<\infty.}
$$

An [algebraic extension](../../../../../algebraic-extension.md) is one in which every element is algebraic. Suppose $M/L$ and $L/K$ are algebraic, and take $\alpha\in M$. A [polynomial](../../../../../polynomial-split.md) relation for $\alpha$ over $L$ uses only finitely many coefficients $a_1,\ldots,a_r$. Each is algebraic over $K$, so adjoining them successively gives a finite extension $E=K(a_1,\ldots,a_r)$, by the proved criterion and the [tower law](../../../../../tower-law.md). The same relation makes $\alpha$ algebraic over $E$, so $E(\alpha)/E$ is finite. Therefore $E(\alpha)/K$ is finite, and its subspace $K(\alpha)$ is finite-dimensional. The criterion makes $\alpha$ algebraic over $K$. Since $\alpha$ was arbitrary, **$M/K$ is algebraic**.

## ↑ Ancestors (10)

1. [18G](../18g.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
