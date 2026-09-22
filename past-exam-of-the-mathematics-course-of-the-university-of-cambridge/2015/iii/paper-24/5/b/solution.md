<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Fix [forcing names](../../../../../../forcing-name.md) $\tau,\tau_1,\ldots,\tau_n\in M$ for the set $w$ and the parameters. Define a name

$$
\sigma=\{(\eta,p):\exists q\ ((\eta,q)\in\tau,\ p\leq q,
\ p\Vdash\varphi(\eta,\tau,\tau_1,\ldots,\tau_n))\}.
$$

Only $\eta$ appearing in $\tau$ and $p\in\mathbb P$ are needed, so this is a subset of a ground-model set. The [forcing definability lemma](../../../../../../forcing-definability-lemma.md) makes its defining predicate a formula of $M$. Ground-model [axiom schema of separation](../../../../../../axiom-schema-of-specification.md) therefore gives $\sigma\in M$.

If $(\eta,p)\in\sigma$ with $p\in G$, the accompanying $q\geq p$ belongs to $G$, so $\eta_G\in\tau_G$. The [forcing theorem](../../../../../../forcing-theorem.md) gives $\varphi(\eta_G,\tau_G,(\tau_1)_G,\ldots,(\tau_n)_G)$.

Conversely, if $u\in\tau_G$ satisfies this formula, choose $(\eta,q)\in\tau$ with $q\in G$ and $\eta_G=u$. The [forcing truth lemma](../../../../../../forcing-truth-lemma.md) supplies $r\in G$ forcing the formula for these names. Directedness gives $p\in G$ with $p\leq q,r$. Then $(\eta,p)\in\sigma$, and $u\in\sigma_G$. Thus

$$
\boxed{\sigma_G=\{u\in w:\varphi(u,w,v_1,\ldots,v_n)\}.}
$$

This proves the instance of the [axiom schema of separation](../../../../../../axiom-schema-of-specification.md) in the [generic extension](../../../../../../generic-extension.md), without assuming that instance there in order to construct the name.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 24](../../../paper-24-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
