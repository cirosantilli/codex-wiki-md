<h1 id="a/3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

[GL](../../../../../godel-lob-logic.md) has all classical propositional [tautologies](../../../../../tautology.md), the normal [distribution](../../../../../normal-modal-distribution-axiom.md) [axiom](../../../../../axiom.md) $\Box(A\to B)\to(\Box A\to\Box B)$ and the Löb [axiom](../../../../../axiom.md) $\Box(\Box A\to A)\to\Box A$, closed under uniform substitution, modus ponens and [necessitation](../../../../../necessitation-rule.md) of theorems. We use its derived positive-introspection theorem $\Box A\to\Box\Box A$, normal boxed reasoning, and the boxed replacement principle supplied in the question.

For completeness, [positive introspection](../../../../../positive-introspection.md) follows from these [axioms](../../../../../axiom.md). Put $C=A\land\Box A$. [Distribution](../../../../../hilbert-bernays-lob-derivability-conditions.md) gives $\Box C\to\Box A$, so [propositional logic](../../../../../classical-propositional-logic.md) proves $A\to(\Box C\to C)$. Necessitate and distribute to get $\Box A\to\Box(\Box C\to C)$; Löb's [axiom](../../../../../axiom.md) gives $\Box A\to\Box C$, and boxing $C\to\Box A$ finishes $\Box A\to\Box\Box A$.

For a [GL fixed point by truth substitution](../../../../../gl-fixed-point-by-truth-substitution.md), [set](../../../../../set-split.md) $\top=(\bot\to\bot)$, $U=\Box Y(\top)$ and $V=\Box Y(U)$. From the [tautology](../../../../../tautology.md) $U\to(\top\leftrightarrow U)$, boxed reasoning gives $\Box U\to\Box(\top\leftrightarrow U)$. The supplied replacement principle and [distribution](../../../../../normal-modal-distribution-axiom.md) then give

$$
\mathrm{GL}\vdash\Box U\to(U\leftrightarrow V).
$$

Since $U$ is itself boxed, [positive introspection](../../../../../positive-introspection.md) gives $U\to\Box U$, and hence $U\to V$.

For the reverse direction, the displayed implication entails the theorem $V\to(\Box U\to U)$. Necessitate it and distribute to obtain $\Box V\to\Box(\Box U\to U)$. Since $V$ is boxed, $V\to\Box V$ holds. The Löb [axiom](../../../../../axiom.md) therefore yields $V\to\Box U$, and the same displayed implication then yields $V\to U$. Consequently

$$
\boxed{\mathrm{GL}\vdash U\leftrightarrow\Box Y(U),\qquad U=\Box Y(\top).}
$$

All occurrences of the unknown letter have been removed from $U$ by substitution of truth; any other parameter letters remain available. The proof does not assume the invalid [reflection](../../../../../full-local-reflection-in-a-one-sentence-extension-is-inconsistent.md) principle $\Box U\to U$ as an unconditional [axiom](../../../../../axiom.md).

## ↑ Ancestors (13)

1. [C](../c.md)
2. [3](../../3.md)
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
