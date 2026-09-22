<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Use the preceding fixed point with $q=\bot$. If the chosen arithmetic interpretation sends $\bot$ to a PA-refutable sentence $Z$, it gives the arithmetic sentence

$$
C=(BZ\to Z),\qquad\operatorname{PA}\vdash C\leftrightarrow(BC\to Z).
$$

This follows from [Arithmetical soundness of GL](../../../../arithmetical-soundness-of-gl.md). Since [Peano arithmetic](../../../../peano-arithmetic.md) proves $\neg Z$, the two implications are equivalent to negated provability:

$$
\operatorname{PA}\vdash C\leftrightarrow\neg BZ,\qquad\operatorname{PA}\vdash C\leftrightarrow\neg BC.
$$

Thus $C$ expresses the [formal consistency statement](../../../../formal-consistency-statement.md) for [Peano arithmetic](../../../../peano-arithmetic.md) and is also a negative provability fixed point, like its [Gödel sentence](../../../../godel-sentence.md) $G$.

Apply the supplied modal uniqueness formula to the context with a [modalized occurrence](../../../../modalized-occurrence.md) $X(p)=(\Box p\to\bot)$, with two fresh variables interpreted as $G$ and $C$. A [modalized occurrence](../../../../modalized-occurrence.md) means that each indicated variable occurrence lies inside a box. [Peano arithmetic](../../../../peano-arithmetic.md) proves both arithmetic fixed-point equations. The first derivability condition boxes those equations, so the translated uniqueness formula gives

$$
\operatorname{PA}\vdash B(G\leftrightarrow C).
$$

One must not infer $G\leftrightarrow C$ by reflection. Instead, distribution and the provability of the two propositional projections give $\operatorname{PA}\vdash BG\leftrightarrow BC$. Negating and using the two fixed-point equations now yields

$$
\boxed{\operatorname{PA}\vdash G\leftrightarrow C\leftrightarrow\neg BZ=\operatorname{Con}(\operatorname{PA}).}
$$

This proves the [Equivalence of a Gödel sentence and a consistency statement](../../../../equivalence-of-a-godel-sentence-and-a-consistency-statement.md) using the required modal soundness, fixed point and uniqueness results.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [3](../../3.md)
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
