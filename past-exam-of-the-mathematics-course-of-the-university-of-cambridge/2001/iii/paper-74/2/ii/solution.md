<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $G=\operatorname{Gal}(K/k)$. Each [field automorphism](../../../../../../field-automorphism.md) preserves the [ring of integers](../../../../../../ring-of-integers.md) and the base [prime ideal](../../../../../../prime-ideal.md), so it permutes the [prime ideals](../../../../../../prime-ideal.md) above $\mathfrak p$. Suppose there were more than one orbit, and fix one orbit $\mathcal C$. By the [Chinese remainder theorem for ideals](../../../../../../chinese-remainder-theorem-for-ideals.md), choose $a\in\mathcal O_K$ such that

$$
a\equiv0\pmod{\mathfrak P}\quad(\mathfrak P\in\mathcal C),\qquad
a\equiv1\pmod{\mathfrak Q}\quad(\mathfrak Q\notin\mathcal C,\ \mathfrak Q\mid\mathfrak p).
$$

The [field norm](../../../../../../field-norm.md) $N_{K/k}(a)=\prod_{\sigma\in G}\sigma(a)$ lies in $\mathcal O_k$. It lies in every [prime ideal](../../../../../../prime-ideal.md) of $\mathcal C$, since for a fixed member each conjugate of $a$ is zero modulo that member. Thus its contraction lies in $\mathfrak p$. On the other hand, for $\mathfrak Q$ outside $\mathcal C$, every $\sigma^{-1}(\mathfrak Q)$ is also outside it, so every $\sigma(a)$ equals one modulo $\mathfrak Q$. The product is consequently one modulo $\mathfrak Q$. This contradicts its membership in $\mathfrak p\mathcal O_K\subseteq\mathfrak Q$. Therefore **the Galois action on the primes above $\mathfrak p$ is transitive**. The [normal extension](../../../../../../normal-extension.md) of [number fields](../../../../../../number-field.md) is separable, so its conjugates are exactly the elements of $G$ used in the product.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 74](../../../paper-74-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
