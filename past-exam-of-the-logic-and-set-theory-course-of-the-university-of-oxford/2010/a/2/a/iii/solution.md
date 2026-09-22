<h1 id="a/2/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The old system does derive the replacement axiom. Here is a syntactic proof using only its axioms, [modus ponens rule](../../../../../../implication-elimination-rule.md), and the permitted [deduction theorem for propositional logic](../../../../../../deduction-theorem-for-propositional-logic.md).

First derive explosion. From $U$ and $\neg U$, the first axiom gives $\neg V\to\neg U$. The old third axiom then gives $U\to V$, and [modus ponens rule](../../../../../../implication-elimination-rule.md) with $U$ gives any desired $V$.

Next derive the classical reductio rule. Suppose $\Gamma,\neg B$ derives both $C$ and $\neg C$. Let $T$ be the theorem $B\to B$, obtainable by applying the [deduction theorem for propositional logic](../../../../../../deduction-theorem-for-propositional-logic.md) to the identity derivation from assumption $B$. Explosion under $\Gamma,\neg B$ gives $\neg T$, so the [deduction theorem for propositional logic](../../../../../../deduction-theorem-for-propositional-logic.md) gives $\Gamma\vdash\neg B\to\neg T$. The old third axiom with $\alpha=T$, $\beta=B$ yields $\Gamma\vdash T\to B$. Since $T$ is a theorem, $\Gamma\vdash B$. Thus a contradiction under $\neg B$ permits deriving $B$ with that temporary assumption discharged.

Now assume $h=\neg\beta\to\alpha$ and $\neg\alpha$, and temporarily also assume $\neg\beta$. [Modus ponens rule](../../../../../../implication-elimination-rule.md) gives $\alpha$, contradicting $\neg\alpha$. The just-proved reductio rule discharges $\neg\beta$ and gives $\beta$. Finally discharge $\neg\alpha$ and $h$ by the [deduction theorem for propositional logic](../../../../../../deduction-theorem-for-propositional-logic.md):

$$
\boxed{(\neg\beta\to\alpha)\to(\neg\alpha\to\beta).}
$$

No propositional completeness theorem is needed in this derivation.

## ↑ Ancestors (14)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [2](../../../2.md)
4. [A](../../../../a.md)
5. [2010](../../../../../2010-split.md)
6. [Past exam of the logic and set theory course of the University of Oxford](../../../../../split.md)
7. [Logic and set theory course of the University of Oxford](../../../../../../logic-and-set-theory-course-of-the-university-of-oxford.md)
8. [Year 3 of the mathematics course of the University of Oxford](../../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
