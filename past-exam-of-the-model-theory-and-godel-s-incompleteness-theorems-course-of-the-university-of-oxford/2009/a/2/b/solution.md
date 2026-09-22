<h1 id="a/2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For [Rosser separation by a bounded stage comparison](../../../../../rosser-separation-by-a-bounded-stage-comparison.md), use the [numeralwise enumeration in arithmetic](../../../../../numeralwise-enumeration-in-arithmetic.md) properties meant by enumeration in $S$: membership supplies some standard stage with a provable positive instance, while nonmembership makes every standard-stage instance refutable. These are stronger than merely attaching a $\Sigma_1$ syntactic label to an arbitrary formula. The finite-initial-segment [axiom](../../../../../axiom.md) lets us combine finitely many numeralwise refutations into a bounded universal assertion.

If $n$ is provable, choose a standard stage $p$ with $S\vdash P(\overline n,\overline p)$. [Consistency](../../../../../consistent-first-order-theory.md) means $n$ is not refutable. Therefore $S\vdash\neg R(\overline n,\overline j)$ for each $j\le p$. Using the displayed finite-segment [axiom](../../../../../axiom.md) and equality substitution, combine these proofs to get $S\vdash\forall z\le\overline p\,\neg R(\overline n,z)$. [Existential introduction](../../../../../existential-quantifier-introduction-rule.md) with stage $p$ proves the separator at $n$.

If $n$ is refutable, choose a standard stage $q$ with $S\vdash R(\overline n,\overline q)$. [Consistency](../../../../../consistent-first-order-theory.md) implies that $n$ is not provable, so all standard instances of $P(\overline n,\cdot)$ are refutable. In particular their finitely many instances through $q$ give $S\vdash\forall z\le\overline q\,\neg P(\overline n,z)$. For an arbitrary proposed witness $z$, the total-comparison [axiom](../../../../../axiom.md) gives $z\le\overline q$ or $\overline q\le z$. In the first case its $P$ conjunct fails; in the second case the known $R$ instance at $q$ contradicts its bounded no-refutation conjunct. [Generalize](../../../../../universal-generalization-rule.md) on $z$ to refute the existential separator. Hence **the proposed first-proof-before-refutation formula separates the two [sets](../../../../../set-split.md)**.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [2](../../2.md)
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
