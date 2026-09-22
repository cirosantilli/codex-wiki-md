<h1 id="a/1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [Hilbert-Bernays-Löb derivability conditions](../../../../../hilbert-bernays-lob-derivability-conditions.md) are: if $S\vdash A$ then $S\vdash\Box A$; $S\vdash\Box(A\to B)\to(\Box A\to\Box B)$; and $S\vdash\Box A\to\Box\Box A$. The first is an external rule about provability; the latter two are internal theorems. Standard numerical correctness and the stipulated $\Sigma_1$ form accompany the predicate in this question. These conditions do not include [reflection](../../../../../full-local-reflection-in-a-one-sentence-extension-is-inconsistent.md) $\Box A\to A$.

Choose a fixed refutable sentence $\bot$ and identify $\operatorname{Con}_S$ with $\neg\Box\bot$. Different fixed refutable choices have provably equivalent [consistency](../../../../../consistent-first-order-theory.md) sentences, because $S$ proves their equivalence to a [contradiction](../../../../../contradiction.md). From $\bot\to G$, [necessitation](../../../../../necessitation-rule.md) and [distribution](../../../../../normal-modal-distribution-axiom.md) give $\Box\bot\to\Box G$. Since $G\to\neg\Box G$, this yields $G\to\operatorname{Con}_S$.

For the converse, necessitate $G\to\neg\Box G$ and distribute to get $\Box G\to\Box\neg\Box G$. [Positive introspection](../../../../../positive-introspection.md) also gives $\Box G\to\Box\Box G$. The two boxed contradictories imply $\Box\bot$ by formalized [propositional reasoning](../../../../../classical-propositional-logic.md). Thus $\Box G\to\Box\bot$, and contraposition gives $\operatorname{Con}_S\to\neg\Box G\to G$. Consequently

$$
\boxed{S\vdash G\leftrightarrow\operatorname{Con}_S.}
$$

Finally the [deduction theorem](../../../../../deduction-theorem-for-first-order-logic.md) says that $S+G$ is [inconsistent](../../../../../consistent-first-order-theory.md) exactly when $S\vdash\neg G$. The internal equivalence identifies $S+G$ and $S+\operatorname{Con}_S$ in their deductive consequences. Hence **$S\nvdash\neg G$ exactly when $S+\operatorname{Con}_S$ is [consistent](../../../../../consistent-first-order-theory.md)**. [Consistency](../../../../../consistent-first-order-theory.md) of $S$ alone need not ensure this stronger [consistency](../../../../../consistent-first-order-theory.md) condition.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [1](../../1.md)
3. [A](../../../a.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the model theory and Gödel's incompleteness theorems course of the University of Oxford](../../../../split.md)
6. [Model theory and Gödel's incompleteness theorems course of the University of Oxford](../../../../../model-theory-and-godel-s-incompleteness-theorems-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
