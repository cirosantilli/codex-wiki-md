<h1 id="1/c/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The standard relational [guarded fragment](../../../../../../guarded-fragment.md) contains $\boxed{\text{(i) and (ii)}}$. In (i), $\mathit{Student}(x)$ guards the only quantified variable:

$$
\forall x\bigl(\mathit{Student}(x)\to(\mathit{Takes}(x,\mathit{KRR},2015)\to((\mathit{Undergrad}(x)\lor\mathit{Masters}(x))\land\neg(\mathit{Undergrad}(x)\land\mathit{Masters}(x))))\bigr).
$$

The constants in the course-taking relation do not introduce additional free variables that need guarding.

For (ii), use the two implications from part (c)(i). Each outer [universal quantification](../../../../../../universal-quantification.md) is guarded by its unary category predicate. The inner [existential quantification](../../../../../../existential-quantification.md) can be written

$$
\exists y\,(\mathit{SupervisedBy}(x,y)\land\top),
$$

whose guard contains both $x$ and $y$. Sentence (iii) uses a nonconstant function and so is outside the standard relational [guarded fragment](../../../../../../guarded-fragment.md). This conclusion uses the original vocabulary; it does not silently replace the counting term by a fresh relation.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [C](../../c.md)
3. [1](../../../1.md)
4. [Knowledge representation and reasoning](../../../../knowledge-representation-and-reasoning-split.md)
5. [2015](../../../../split.md)
6. [Past exam of the computer science course of the University of Oxford](../../../../../split.md)
7. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
