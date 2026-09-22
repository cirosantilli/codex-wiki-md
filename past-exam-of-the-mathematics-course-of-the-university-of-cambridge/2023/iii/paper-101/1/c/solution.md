<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Suppose for a contradiction that $m>n$. Compose the given [injective module homomorphism](../../../../../../module-homomorphism.md) with the standard injection $B^n\hookrightarrow B^m$ that appends $m-n$ zero coordinates. This gives an injective [endomorphism](../../../../../../endomorphism.md) $T$ of the [finite free module](../../../../../../finite-free-module.md) $B^m$ whose matrix has a zero final row.

Its [characteristic polynomial](../../../../../../characteristic-polynomial.md) has zero constant term, so the [Cayley-Hamilton theorem](../../../../../../cayley-hamilton-theorem.md) gives

$$
T^m+c_{m-1}T^{m-1}+\cdots+c_1T=0.
$$

Injectivity lets us cancel $T$. Repeating this argument eventually gives the identity endomorphism equal to zero. That would imply $B^m=0$, contrary to $B\ne0$. Hence $m\leq n$. This proves the [rank inequality for an injection of finite free modules](../../../../../../rank-inequality-for-an-injection-of-finite-free-modules.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 101](../../../paper-101-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
