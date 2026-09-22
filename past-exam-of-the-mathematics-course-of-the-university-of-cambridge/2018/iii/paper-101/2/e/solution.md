<h1 id="2/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Let $e_j$ be the sequence with $1$ in coordinate $j$ and zero elsewhere. In the [direct product of rings](../../../../../../direct-product-of-rings.md) $R=k^{\mathbb N}$, the [ideals](../../../../../../ideal.md)

$$
(e_1)\subsetneq(e_1,e_2)\subsetneq(e_1,e_2,e_3)\subsetneq\cdots
$$

form a strict ascending chain: every element of $(e_1,\ldots,e_n)$ vanishes after coordinate $n$, whereas $e_{n+1}$ does not. Hence **$R$ is not a Noetherian ring**.

Nevertheless, each $a=(a_j)\in R$ has a coordinatewise generalized inverse $b=(b_j)$, defined by $b_j=a_j^{-1}$ when $a_j\ne0$ and $b_j=0$ otherwise. It satisfies

$$
a=a^2b.
$$

This is the defining property of a [Von Neumann regular ring](../../../../../../von-neumann-regular-ring.md). Fix any [prime ideal](../../../../../../prime-ideal.md) $P$, and take $a\in P$. Since $ab\in P$, $1-ab\notin P$; but

$$
(1-ab)a=0.
$$

Consequently $a/1=0$ in the [localization at a prime ideal](../../../../../../localization-at-a-prime-ideal.md) $R_P$. All elements of $PR_P$ therefore vanish. By the [local ring](../../../../../../local-ring.md) description in part (a), $PR_P$ is the unique [maximal ideal](../../../../../../maximal-ideal.md), so $R_P$ is a nonzero [field](../../../../../../field.md). A [field](../../../../../../field.md) has only the [ideals](../../../../../../ideal.md) zero and itself, and thus is [Noetherian](../../../../../../noetherian-ring.md).

We have proved the stronger conclusion

$$
\boxed{R_P\text{ is a field for every prime ideal }P\subset R.}
$$

The argument applies to every [prime ideal](../../../../../../prime-ideal.md), without assuming that it comes from a coordinate projection.

## ↑ Ancestors (11)

1. [E](../e.md)
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
