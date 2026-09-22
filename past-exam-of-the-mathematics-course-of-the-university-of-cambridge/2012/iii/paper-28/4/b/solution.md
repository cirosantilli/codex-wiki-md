<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

One form of [Krasner's lemma](../../../../../../krasner-s-lemma.md) is: if $K$ is a complete non-Archimedean field, $\alpha$ is separable over $K$, and $\beta$ is algebraic with

$$
|\beta-\alpha|<\min_{\alpha'\ne\alpha}|\alpha-\alpha'|,
$$

where $\alpha'$ ranges over the other $K$-conjugates, then $K(\alpha)\subseteq K(\beta)$. If $\alpha\in K$, the conclusion is immediate.

To prove the nontrivial case, let $\sigma$ be an automorphism of an algebraic closure fixing $K(\beta)$. The [unique extension of an absolute value to a finite extension](../../../../../../unique-extension-of-an-absolute-value-to-a-finite-extension.md) implies that $\sigma$ preserves the extended absolute value. Therefore

$$
|\sigma(\alpha)-\alpha|\leq\max\bigl(|\sigma(\alpha)-\beta|,|\beta-\alpha|\bigr)=|\beta-\alpha|.
$$

This is strictly less than the distance to every other conjugate, so $\sigma(\alpha)=\alpha$. As $\alpha$ is separable over $K(\beta)$, being fixed by all these automorphisms puts it in $K(\beta)$. **This proves $\boxed{K(\alpha)\subseteq K(\beta)}$.** The strict inequality is what prevents switching to another conjugate.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 28](../../../paper-28-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
