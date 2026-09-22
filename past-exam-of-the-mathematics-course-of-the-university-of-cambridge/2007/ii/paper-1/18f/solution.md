<h1 id="18f/solution">Solution</h1>

↑ **Parent:** [18F](../18f.md)

The [degree of a field extension](../../../../../degree-of-a-field-extension.md) $[K:M]$ is the [dimension of a vector space](../../../../../dimension-vector-space.md) of $K$ over $M$. If $(\alpha_i)$ is an $M$-basis of $K$ and $(\beta_j)$ a $K$-basis of $L$, then $(\alpha_i\beta_j)$ spans $L$ over $M$. An $M$-linear relation among these products, regrouped by $j$, first vanishes coefficientwise by independence of the $\beta_j$, and then by independence of the $\alpha_i$. This proves the [tower law](../../../../../tower-law.md) $[L:M]=[L:K][K:M]$, including cardinal dimensions.

A [finite field](../../../../../finite-field.md) has prime [characteristic](../../../../../characteristic-of-a-field.md) $p$ and is a finite-dimensional [vector space](../../../../../vector-space-split.md) over its prime field $\mathbb F_p$. Thus its size is $p^n$. A subfield of size $p^m$ forces $m\mid n$ by the [tower law](../../../../../tower-law.md). Conversely, if $m\mid n$, the polynomial $X^{p^m}-X$ divides $X^{p^n}-X$; all its $p^m$ distinct roots therefore lie in $K$. They are closed under addition, multiplication and inverses by the [Finite-field Frobenius automorphism](../../../../../finite-field-frobenius-automorphism.md), forming the required subfield.

For an [irreducible polynomial](../../../../../irreducible-polynomial.md) of degree $d$ over $\mathbb F_q$, a root generates $\mathbb F_{q^d}$. Its conjugates are $\alpha,\alpha^q,\ldots,\alpha^{q^{d-1}}$, so this field is already the [splitting field](../../../../../splitting-field.md). The automorphism $x\mapsto x^q$ cycles these roots and has order $d$. Consequently

$$
\boxed{\operatorname{Gal}(f/\mathbb F_q)\cong C_d.}
$$

## ↑ Ancestors (10)

1. [18F](../18f.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
