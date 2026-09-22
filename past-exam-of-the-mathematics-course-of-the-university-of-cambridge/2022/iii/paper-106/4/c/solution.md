<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [Commutative Gelfand--Naimark theorem](../../../../../../commutative-gelfand-naimark-theorem.md) says that every commutative unital [C-star algebra](../../../../../../c-star-algebra.md) $A$ is isometrically star-isomorphic to $C(\Delta(A))$, where $\Delta(A)$ is its compact [character space](../../../../../../character-space-of-an-algebra.md) and the map is the [Gelfand transform](../../../../../../gelfand-representation.md)

$$
\Gamma(a)(\chi)=\chi(a).
$$

Indeed, maximal ideals give enough characters to identify $\sigma(a)$ with the range of $\widehat a$. The C-star identity and the [spectral radius formula](../../../../../../spectral-radius-formula.md) give

$$
\lVert\widehat a\rVert_\infty^2
=r(a^*a)=\lVert a^*a\rVert=\lVert a\rVert^2,
$$

so $\Gamma$ is isometric and has closed range. Characters send $a^*$ to $\overline{\chi(a)}$, so the range is self-conjugate; it contains constants and separates distinct characters. The complex [Stone-Weierstrass theorem](../../../../../../stone-weierstrass-theorem.md) makes the range dense in $C(\Delta(A))$, and closedness makes it all of that algebra. This proves the theorem.

An element $x$ of a C-star algebra is positive when it is self-adjoint and $\sigma(x)\subseteq[0,\infty)$. Consider the commutative C-star subalgebra $C^*(1,x)$. Under its Gelfand–Naimark isomorphism, $x$ becomes a nonnegative continuous function $\widehat x$. The function $\sqrt{\widehat x}$ is continuous and nonnegative, so its inverse image $y$ is positive and satisfies

$$
\boxed{y^2=x.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 106](../../../paper-106-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
