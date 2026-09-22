<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Assume $\nvdash_{IPC}\varphi$. By Kripke completeness there is a rooted countermodel. Unravel it into a tree and retain only the subformulas $\Phi$ of $\varphi$. Whenever a retained node fails an implication $\alpha\to\beta\in\Phi$, retain one successor witnessing $\alpha$ and the failure of $\beta$. Along a branch, passing to a genuinely new witness strictly enlarges the finite theory of subformulas, so at most $n$ witness levels are needed. Identifying repeated equal theories and retaining at most one witness for each failed implication leaves at most $n$ representatives for each of the at most $2^n$ theories. The resulting pruned filtration has at most $n2^n$ worlds and still refutes $\varphi$ by the truth lemma.

**Thus every underivable formula with $n$ subformulas has a countermodel of size at most $n2^n$. The contrapositive proves the claim and is the quantitative [Finite model property of intuitionistic propositional logic](../../../../../../finite-model-property-of-intuitionistic-propositional-logic.md).**

## ↑ Ancestors (11)

1. [E](../e.md)
2. [1](../../1.md)
3. [Paper 120](../../../paper-120-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
