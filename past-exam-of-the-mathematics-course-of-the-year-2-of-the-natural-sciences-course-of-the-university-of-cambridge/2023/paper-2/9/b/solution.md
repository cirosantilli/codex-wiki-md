<h1 id="9/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let

$$
K=\{e,(12)(34),(13)(24),(14)(23)\}.
$$

The product of any two distinct nonidentity elements is the third, and each squares to $e$, so $K$ is a [Klein four-group](../../../../../klein-four-group.md). Conjugating a double transposition simply relabels its letters, keeping it in the set. Hence $K$ is a [normal subgroup](../../../../../normal-subgroup.md) of $A_4$.

Choose $r=(123)$. The [cosets](../../../../../coset.md) $K,rK,r^2K$ are distinct and cover the twelve elements. With $\zeta=e^{2\pi i/3}$, define

$$
\boxed{\Phi(r^jk)=\zeta^j,\qquad j\in\{0,1,2\},\quad k\in K.}
$$

The coset decomposition makes this well-defined. Normality gives

$$
(r^jk)(r^\ell k')=r^{j+\ell}(r^{-\ell}kr^\ell)k'\in r^{j+\ell}K,
$$

so $\Phi$ preserves products. It is onto $\{1,\zeta,\zeta^2\}\cong C_3$, and

$$
\boxed{\ker\Phi=K,\qquad A_4/K\cong C_3.}
$$

This is the [tetrahedral quotient onto the cyclic group of order three](../../../../../tetrahedral-quotient-onto-the-cyclic-group-of-order-three.md). In terms of (a), it sends $C_0\cup C_2$ to $1$, $C_+$ to $\zeta$, and $C_-$ to $\zeta^2$. The normality check above also follows abstractly because a [group homomorphism kernel](../../../../../kernel-of-a-group-homomorphism.md) is normal.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [9](../../9.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
