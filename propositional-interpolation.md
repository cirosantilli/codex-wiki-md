# Propositional interpolation

↑ **Parent:** [Propositional variable elimination](propositional-variable-elimination.md)

If $A\vdash B$, eliminate the letters private to $A$ by

$$
C=\bigvee_{\varepsilon:\operatorname{Var}(A)\setminus\operatorname{Var}(B)\to\{0,1\}}A[\varepsilon].
$$

Every assignment satisfying $A$ satisfies one disjunct of $C$. If an assignment satisfies $C$, change only the eliminated letters to its witnessing assignment. The modified assignment satisfies $A$ and hence $B$, whose letters were unchanged. Thus $A\models C\models B$, and the [propositional completeness theorem](completeness-theorem-for-propositional-logic.md) gives the two derivations. The interpolant uses only common letters; an empty common vocabulary is handled by logical truth constants.

## ↑ Ancestors (8)

1. [Propositional variable elimination](propositional-variable-elimination.md)
2. [Propositional formula](propositional-formula.md)
3. [Propositional logic](propositional-logic.md)
4. [Mathematical logic](mathematical-logic-split.md)
5. [Foundations of mathematics](foundations-of-mathematics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ii/paper-2/16g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-20/4/b/solution.md)
