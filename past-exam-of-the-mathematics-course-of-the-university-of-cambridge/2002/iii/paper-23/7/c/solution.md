<h1 id="7/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Every fixed [second-order logic](../../../../../../second-order-logic.md) sentence is evaluable in [PSPACE](../../../../../../pspace.md). On a universe of size $n$, a relation of arity $k$ is stored using $n^k$ bits. Enumerate its possible interpretations with a counter of the same polynomial length, recursively evaluate the inner formula and reuse the storage. Universal quantifiers require checking all interpretations; existential ones stop at the first success. The fixed quantifier depth and fixed arities bound total space by a polynomial, even though time can be exponential. First-order quantifiers and Boolean operations require no larger bound.

If $NP=PSPACE$, this places the class defined by the assumed second-order sentence in NP. [Fagin's theorem](../../../../../../fagin-s-theorem.md) would give an equivalent existential second-order sentence, again contradicting the hypothesis. Hence

$$
\boxed{NP\ne PSPACE.}
$$

For completeness, $NP\subseteq PSPACE$: a polynomial-time nondeterministic computation can be searched deterministically depth first, retaining a polynomial-length computation branch and reusing space. Thus the inequality is a strict containment under the stated hypothesis.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [7](../../7.md)
3. [Paper 23](../../../paper-23-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
