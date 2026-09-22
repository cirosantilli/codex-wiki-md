<h1 id="16i/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $|F|=p^n$, where $n=[F:\mathbb F_p]$ since $F$ is a finite-dimensional [vector space](../../../../../../vector-space-split.md) over its [prime field](../../../../../../prime-field.md). Every nonzero element satisfies $x^{p^n-1}=1$ by [Lagrange theorem](../../../../../../lagrange-s-theorem.md), so $F$ is exactly the [splitting field](../../../../../../splitting-field.md) of $X^{p^n}-X$ over $\mathbb F_p$. The [derivative](../../../../../../derivative.md) is $-1$, making it a [separable polynomial](../../../../../../separable-polynomial.md). Thus the extension is a [normal field extension](../../../../../../normal-extension.md) and a [separable field extension](../../../../../../separable-extension.md), hence a [Galois extension](../../../../../../finite-galois-extension.md).

The [finite-field Frobenius automorphism](../../../../../../finite-field-frobenius-automorphism.md) $\sigma(x)=x^p$ fixes $\mathbb F_p$ and has $\sigma^n=1$. If $\sigma^d=1$ with $0<d<n$, all $p^n$ elements would be roots of the degree-$p^d$ [polynomial](../../../../../../polynomial-split.md) $X^{p^d}-X$, impossible. It has order $n$, equal to the degree of the [Galois extension](../../../../../../finite-galois-extension.md). Therefore

$$
\boxed{\operatorname{Gal}(F/\mathbb F_p)=\langle\sigma\rangle\cong C_n.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [16I](../../16i.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
