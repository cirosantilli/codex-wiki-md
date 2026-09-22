<h1 id="18h/solution">Solution</h1>

↑ **Parent:** [18H](../18h.md)

The [polynomial](../../../../../polynomial-split.md) $X^m-1$ is separable, since its [derivative](../../../../../derivative.md) $mX^{m-1}$ has no common root with it when the [characteristic](../../../../../characteristic-of-a-field.md) does not divide $m$. Its roots form a cyclic multiplicative group of order $m$. For completeness, any finite subgroup of a field's multiplicative group is cyclic: if its exponent is $e$, all its elements are roots of $X^e-1$, so its size is at most $e$, while the elementary decomposition of a finite abelian group gives an element of order $e$.

Choose a primitive root $\zeta$. Then $L=K(\zeta)$, and every [field automorphism](../../../../../field-automorphism.md) sends $\zeta$ to $\zeta^a$ for a unique unit $a$ modulo $m$. Composition multiplies the exponents, and fixing $\zeta$ fixes all of $L$. This is the required injective homomorphism

$$
\boxed{\operatorname{Gal}(L/K)\hookrightarrow(\mathbb Z/m\mathbb Z)^*.}
$$

For $K=\mathbb F_q$, the least extension $\mathbb F_{q^d}$ containing a primitive $m$th root is characterized by $m\mid q^d-1$, since its multiplicative group is cyclic of order $q^d-1$. Thus $[L:K]$ is the multiplicative order of $q$ modulo $m$. The successive powers of $4$ modulo $11$ are $4,5,9,3,1$, so

$$
\boxed{[\mathbb F_4(\zeta_{11}):\mathbb F_4]=5.}
$$

## ↑ Ancestors (10)

1. [18H](../18h.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
