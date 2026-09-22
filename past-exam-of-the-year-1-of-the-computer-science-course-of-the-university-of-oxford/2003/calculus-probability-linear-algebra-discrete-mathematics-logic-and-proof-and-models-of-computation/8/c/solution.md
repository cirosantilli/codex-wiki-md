<h1 id="8/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

In the language of [first-order logic](../../../../../first-order-logic.md), define

$$
\boxed{\operatorname{Bottom}(b)\;\equiv\;\forall y\;R(b,y),\qquad\operatorname{Minimal}(b)\;\equiv\;\forall y\;(R(y,b)\Rightarrow y=b).}
$$

Thus a [least element](../../../../../least-element.md) lies below every element, whereas a [minimal element](../../../../../minimal-element-of-a-partially-ordered-set.md) merely has no distinct element below it. The latter definition allows multiple incomparable [minimal elements](../../../../../minimal-element-of-a-partially-ordered-set.md).

Here is a formal [natural deduction](../../../../../natural-deduction.md) proof, with the antisymmetry axiom available as a premise. Assume $\operatorname{Bottom}(b)$ and take a fresh arbitrary variable $t$. Assume $R(t,b)$. By [universal elimination](../../../../../universal-quantifier-elimination-rule.md) applied to $\operatorname{Bottom}(b)$, obtain $R(b,t)$. By [conjunction introduction](../../../../../conjunction-introduction-rule.md), obtain $R(t,b)\land R(b,t)$. Instantiate antisymmetry at $t,b$, and use [modus ponens rule](../../../../../implication-elimination-rule.md) to obtain $t=b$. Discharge the assumption $R(t,b)$ by [implication introduction](../../../../../implication-introduction-rule.md), obtaining $R(t,b)\Rightarrow t=b$. Since $t$ was arbitrary and is free in no undischarged assumption, [universal introduction](../../../../../universal-quantifier-introduction-rule.md) gives $\operatorname{Minimal}(b)$. Discharge the initial assumption and universally quantify $b$ to conclude

$$
\boxed{\forall b\;\bigl(\operatorname{Bottom}(b)\Rightarrow\operatorname{Minimal}(b)\bigr).}
$$

Only antisymmetry was needed for this implication; reflexivity and transitivity are part of the ambient [partial order](../../../../../partially-ordered-set.md) axioms.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [8](../../8.md)
3. [Calculus, probability, linear algebra, discrete mathematics, logic and proof, and models of computation](../../../calculus-probability-linear-algebra-discrete-mathematics-logic-and-proof-and-models-of-computation-split.md)
4. [2003](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
