<h1 id="a/1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Again abbreviate provability by $\Box$. The [Gödel sentence](../../../../../godel-sentence.md) equivalence gives $S\vdash G\to\neg\Box G$. Internalizing this implication using the first two [Hilbert-Bernays-Löb derivability conditions](../../../../../hilbert-bernays-lob-derivability-conditions.md) gives

$$
S\vdash\Box G\to\Box\neg\Box G.
$$

[Positive introspection](../../../../../positive-introspection.md) also gives $S\vdash\Box G\to\Box\Box G$. Internal [modus ponens rule](../../../../../implication-elimination-rule.md) combines proofs of a sentence and its [negation](../../../../../negation.md) into a proof of a contradiction; a contradiction implies any sentence. Consequently

$$
S\vdash\Box G\to\Box\neg G.
$$

These are syntactic manipulations of provability, not an appeal to [soundness](../../../../../soundness.md). If $S\vdash\neg\Box\neg G$, taking the contrapositive of the last implication gives $S\vdash\neg\Box G$, and the diagonal equivalence gives $S\vdash G$. Part (a) rules that out for a consistent theory. Hence

$$
\boxed{S\nvdash\neg\Box\neg G\quad\text{when }S\text{ is consistent}.}
$$

## ↑ Ancestors (13)

1. [B](../b.md)
2. [1](../../1.md)
3. [A](../../../a.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the model theory and Gödel's incompleteness theorems course of the University of Oxford](../../../../split.md)
6. [Model theory and Gödel's incompleteness theorems course of the University of Oxford](../../../../../model-theory-and-godel-s-incompleteness-theorems-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
