<h1 id="6/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Choose a linear functional $\ell:E\to\mathbb R$ which is nonzero on every [root](../../../../../../root-of-a-root-system.md); one exists because there are only finitely many [root](../../../../../../root-of-a-root-system.md) hyperplanes to avoid. Declare a [root](../../../../../../root-of-a-root-system.md) positive when $\ell(\alpha)>0$, and negative when $\ell(\alpha)<0$. This orders the [roots](../../../../../../root-of-a-root-system.md) by sign, compatibly with addition whenever the sum is a [root](../../../../../../root-of-a-root-system.md). One can refine it to a lexicographic total order by completing $\ell$ to a coordinate system. Since negation permutes the [roots](../../../../../../root-of-a-root-system.md),

$$
\boxed{R=R^+\sqcup R^-,\qquad R^-=-R^+.}
$$

A [simple root](../../../../../../simple-root.md) is a [positive root](../../../../../../positive-root.md) not expressible as the sum of two [positive roots](../../../../../../positive-root.md). If distinct [simple roots](../../../../../../simple-root.md) $\alpha,\beta$ had $\alpha-\beta$ as a [root](../../../../../../root-of-a-root-system.md), it would be either positive or negative. In the first case $\alpha=\beta+(\alpha-\beta)$ decomposes $\alpha$ into two [positive roots](../../../../../../positive-root.md); in the second $\beta=\alpha+(\beta-\alpha)$ decomposes $\beta$. Both contradict simplicity. If they are equal, their difference is zero and is also not a [root](../../../../../../root-of-a-root-system.md). Hence **the difference of two [simple roots](../../../../../../simple-root.md) is never a [root](../../../../../../root-of-a-root-system.md)**.

For use in the final subpart, the [simple roots](../../../../../../simple-root.md) form a [basis](../../../../../../basis.md), and every [positive root](../../../../../../positive-root.md) is a nonnegative integer combination of them. Here are the needed reasons. Repeatedly decompose a nonsimple [positive root](../../../../../../positive-root.md) into two [positive roots](../../../../../../positive-root.md); their $\ell$ values decrease, and the finite [root](../../../../../../root-of-a-root-system.md) set makes this terminate. This gives the integer combinations. Distinct [simple roots](../../../../../../simple-root.md) have nonpositive [inner product](../../../../../../inner-product.md): a positive [inner product](../../../../../../inner-product.md) would make $\alpha$ and $-\beta$ obtuse, so the qualified root-sum lemma would make $\alpha-\beta$ a [root](../../../../../../root-of-a-root-system.md), just ruled out. Finally, a nontrivial linear relation between [simple roots](../../../../../../simple-root.md) can be split into positive and negative coefficients, giving the same vector $u$ as positive combinations of disjoint sets. Its squared norm, computed using those two expressions, is nonpositive, whereas a nonzero positive combination has positive $\ell$ value. This contradiction proves linear independence. Their span is $E$ because they generate all [roots](../../../../../../root-of-a-root-system.md).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [6](../../6.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
