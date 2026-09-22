<h1 id="7/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Here equivalence means equivalence on all finite structures of the chosen signature, and an [existential sentence](../../../../../../existential-sentence.md) means an existential second-order sentence. Suppose, towards a contradiction, that [P](../../../../../../p-complexity.md) equals [NP](../../../../../../np-complexity.md). We use that P is closed under complementation, that fixed first-order model checking is polynomial-time, and that guessing a polynomial-length string followed by a polynomial-time test is in NP.

Under this equality, evaluating any fixed [second-order logic](../../../../../../second-order-logic.md) sentence is in P. Prove this by induction through its quantifiers and Boolean operations. The first-order part is already polynomial-time. If an inner formula can be evaluated in P, existentially quantifying a relation of fixed arity guesses at most $n^k$ bits and then performs the inner polynomial-time test. This gives an NP procedure and hence, under the assumption, a P procedure. A universal relation quantifier is handled by complementing the corresponding existential test. Boolean combinations remain polynomial-time as well. A fixed formula has only finitely many such steps and fixed arities, so the resulting time bound is polynomial.

Consequently every second-order definable class lies in P, hence in NP. By [Fagin's theorem](../../../../../../fagin-s-theorem.md) it has an equivalent existential second-order sentence. This contradicts the posited second-order sentence with no such equivalent. Therefore

$$
\boxed{P\ne NP.}
$$

The proof uses the equality assumption to collapse quantifier alternation; it does not assume an unproved strictness statement about the polynomial hierarchy.

## ↑ Ancestors (11)

1. [B](../b.md)
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
