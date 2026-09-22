<h1 id="22j/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For a probability distribution $m$ on $\mathbb R$, take the canonical sample space $\Omega=\mathbb R^{\mathbb N}$, the product of the Borel $\sigma$-algebras, and the [product measure](../../../../../../product-measure.md) $\mathbb P=m^{\otimes\mathbb N}$. The coordinate functions $X_j(\omega)=\omega_j$ have joint cylinder probabilities

$$
\mathbb P(X_1\in A_1,\ldots,X_r\in A_r)=\prod_{j=1}^rm(A_j).
$$

The [Kolmogorov extension theorem](../../../../../../kolmogorov-extension-theorem.md) supplies this measure from the consistent finite-dimensional distributions, and uniqueness follows from the generating cylinder sets. Thus the coordinates are [independent and identically distributed](../../../../../../independent-and-identically-distributed-random-variables.md); the same construction works for a given standard Borel state space.

The one-sided [Bernoulli shift](../../../../../../bernoulli-shift.md) is $T(\omega_1,\omega_2,\ldots)=(\omega_2,\omega_3,\ldots)$. It is measurable and preserves all cylinder probabilities. The uniqueness theorem for probability measures extends this to the product $\sigma$-algebra, proving measure preservation.

To prove [ergodicity](../../../../../../ergodicity.md), let $A$ be invariant modulo null sets and approximate it in probability by an event $C$ depending on only the first $r$ coordinates, with $\mathbb P(A\triangle C)<\epsilon$. Such approximations follow from the fact that finite-coordinate cylinder events generate the product $\sigma$-algebra. For $n\geq r$, independence gives $\mathbb P(C\cap T^{-n}C)=\mathbb P(C)^2$. Invariance and measure preservation give

$$
\mathbb P(A)=\mathbb P(A\cap T^{-n}A),\qquad |\mathbb P(A)-\mathbb P(C\cap T^{-n}C)|\leq2\epsilon.
$$

Also $|\mathbb P(A)^2-\mathbb P(C)^2|\leq2\epsilon$. Letting $\epsilon\downarrow0$ proves $\mathbb P(A)=\mathbb P(A)^2$, so **$\boxed{\mathbb P(A)\in\{0,1\}}$**. This is exactly ergodicity.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [22J](../../22j.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
