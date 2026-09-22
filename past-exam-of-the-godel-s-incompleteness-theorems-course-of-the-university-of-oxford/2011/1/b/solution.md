<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $BA=\exists y\,\operatorname{Prov}(\ulcorner A\urcorner,y)$ and fix a refutable [first-order sentence](../../../../first-order-sentence.md) $\bot$, so $S\vdash\neg\bot$ and $\operatorname{Con}_S=\neg B\bot$. First prove the internal equivalence

$$
\boxed{S\vdash G\leftrightarrow\operatorname{Con}_S.}
$$

Because $\bot\to G$ is provable, the [derivability conditions](../../../../hilbert-bernays-lob-derivability-conditions.md) give $B\bot\to BG$. The fixed-point equivalence $G\leftrightarrow\neg BG$ therefore yields $G\to\neg B\bot$.

For the reverse implication, necessitating $G\to\neg BG$ and applying distribution gives $BG\to B(\neg BG)$. [positive introspection](../../../../positive-introspection.md) gives $BG\to B(BG)$. Finally the provable implication $BG\to(\neg BG\to\bot)$, necessitated and distributed, gives

$$
B(BG)\to\bigl(B(\neg BG)\to B\bot\bigr).
$$

Consequently $S\vdash BG\to B\bot$, so $\neg B\bot\to\neg BG\to G$. The same argument works with any chosen refutable [first-order sentence](../../../../first-order-sentence.md) in place of $\bot$; their formal consistency statements are provably equivalent.

By the classical [deduction theorem for propositional logic](../../../../deduction-theorem-for-propositional-logic.md) applied to adjoining a [first-order sentence](../../../../first-order-sentence.md), $S+\{G\}$ is consistent exactly when $S\nvdash\neg G$. The displayed equivalence makes $S+\{G\}$ and $S+\{\operatorname{Con}_S\}$ deductively equivalent. Therefore

$$
\boxed{S\nvdash\neg G\iff S+\{\operatorname{Con}_S\}\text{ is consistent}.}
$$

No soundness assumption on that extension is being substituted for consistency.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the Gödel's incompleteness theorems course of the University of Oxford](../../../split.md)
5. [Gödel's incompleteness theorems course of the University of Oxford](../../../../godel-s-incompleteness-theorems-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
