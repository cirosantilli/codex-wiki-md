<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the positive variable $Y$ from part (a). Since $0\leq(S-B)^+\leq S$ and $(S-B)^+\geq S-B$,

$$
0\leq c=\mathbb E[Y(S-B)^+]\leq\mathbb E[YS]=s,
\qquad c\geq\mathbb E[Y(S-B)]=s-b.
$$

Combining these inequalities gives the [one-period call price bounds](../../../../../../one-period-call-price-bounds.md)

$$
\boxed{(s-b)^+\leq c\leq s.}
$$

For the strict assertion, both $\{S>B\}$ and $\{S<B\}$ have positive probability. Positivity of $Y$ gives

$$
c=\mathbb E[Y(S-B)^+]>0,
\qquad c-(s-b)=\mathbb E[Y(B-S)^+]>0.
$$

If $s-b\geq0$, the second inequality is the required strict bound; if $s-b<0$, the first is. Hence $\boxed{c>(s-b)^+}$. The weighted expectations are finite because $P$ and $Y$ are bounded.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 40](../../../paper-40-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
