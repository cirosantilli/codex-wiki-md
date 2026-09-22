<h1 id="a/3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Abbreviate the [arithmetical provability predicate](../../../../../arithmetical-provability-predicate.md) by $\Box$, with the [Hilbert-Bernays-Löb derivability conditions](../../../../../hilbert-bernays-lob-derivability-conditions.md) understood. [Löb's theorem](../../../../../lob-s-theorem.md) says

$$
\boxed{S\vdash\Box A\to A\quad\Longrightarrow\quad S\vdash A.}
$$

Choose a diagonal sentence $D$ with $S\vdash D\leftrightarrow(\Box D\to A)$. Internalizing its forward implication gives $S\vdash\Box D\to\Box(\Box D\to A)$. Internal [modus ponens rule](../../../../../implication-elimination-rule.md) gives $\Box(\Box D\to A)\to(\Box\Box D\to\Box A)$, while [positive introspection](../../../../../positive-introspection.md) gives $\Box D\to\Box\Box D$. Combining these yields $S\vdash\Box D\to\Box A$.

Now use the assumed theorem $\Box A\to A$. It follows that $S\vdash\Box D\to A$, and the reverse direction of the diagonal equivalence gives $S\vdash D$. External [necessitation rule](../../../../../necessitation-rule.md) gives $S\vdash\Box D$, and the previously derived implication gives $S\vdash A$. This proves the theorem from the supplied fixed-point property and the derivability conditions.

The [Gödel second incompleteness theorem](../../../../../godel-second-incompleteness-theorem.md) states that a consistent [arithmetic](../../../../../arithmetic-split.md) theory in this setting cannot prove its own consistency sentence $\operatorname{Con}_S=\neg\Box\bot$. If it could, it would prove $\Box\bot\to\bot$; applying Löb's theorem with $A=\bot$ would make it inconsistent. Therefore $\boxed{S\nvdash\operatorname{Con}_S}$ when $S$ is consistent.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [3](../../3.md)
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
