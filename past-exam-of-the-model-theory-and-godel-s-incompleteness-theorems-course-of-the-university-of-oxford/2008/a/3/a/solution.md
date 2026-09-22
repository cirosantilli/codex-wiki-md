<h1 id="a/3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the [Hilbert-Bernays-Löb derivability conditions](../../../../../hilbert-bernays-lob-derivability-conditions.md) for an [arithmetical provability predicate](../../../../../arithmetical-provability-predicate.md). Abbreviate $P_S(\ulcorner A\urcorner)$ by $P A$. The conditions needed below are

$$
S\vdash A\Longrightarrow S\vdash P A,\qquad
S\vdash P(A\to B)\to(P A\to P B),\qquad
S\vdash P A\to P P A.
$$

These are the usual theoremhood, distribution and positive-introspection conditions intended by a standard [arithmetical provability predicate](../../../../../arithmetical-provability-predicate.md); arbitrary [predicate symbols](../../../../../predicate-symbol.md) merely agreeing with provability externally need not satisfy them.

Since $S\vdash\neg Y$, it proves $Y\to G$. The first two conditions give $S\vdash P Y\to P G$. For the converse, the fixed-point equivalence gives $S\vdash G\to(P G\to Y)$. Applying theoremhood and distribution gives

$$
S\vdash P G\to P(P G\to Y).
$$

[Positive introspection](../../../../../positive-introspection.md) also gives $P G\to P P G$, and distribution combines these to yield $S\vdash P G\to P Y$. Thus $S\vdash P G\leftrightarrow P Y$. Combining with $G\leftrightarrow\neg P G$ proves

$$
\boxed{S\vdash G\leftrightarrow\neg P Y.}
$$

If $S$ proved $\neg P Y$, it would prove $G$. The theoremhood condition would then give $P G$, while the fixed-point equivalence gives $\neg P G$. Therefore [first-order consistency](../../../../../first-order-consistency.md) implies

$$
\boxed{S\nvdash\neg P Y.}
$$

## ↑ Ancestors (13)

1. [A](../a.md)
2. [3](../../3.md)
3. [A](../../../a.md)
4. [2008](../../../../2008-split.md)
5. [Past exam of the model theory and Gödel's incompleteness theorems course of the University of Oxford](../../../../split.md)
6. [Model theory and Gödel's incompleteness theorems course of the University of Oxford](../../../../../model-theory-and-godel-s-incompleteness-theorems-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
