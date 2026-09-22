# Hidden-variable encoding

↑ **Parent:** [Constraint satisfaction problem](constraint-satisfaction-problem.md)

Replace a finite many-variable relation $R(X_1,\ldots,X_k)$ by one auxiliary [variable](variable-mathematics.md) $Y$ whose domain is the allowed tuples of $R$, together with [binary constraints](binary-constraint.md) equating each tuple coordinate to its corresponding $X_i$. Any original satisfying assignment extends to exactly its allowed tuple, and any satisfying encoded assignment projects to a solution of $R$. The tuple domain can be large; the transformation changes arity, not necessarily representation size efficiently when $R$ is succinct.

## ↑ Ancestors (7)

1. [Constraint satisfaction problem](constraint-satisfaction-problem.md)
2. [Search problem](search-problem.md)
3. [Computational problem](computational-problem.md)
4. [Computational complexity theory](computational-complexity-theory.md)
5. [Theoretical computer science](theoretical-computer-science-split.md)
6. [Computer science](computer-science-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2021/artificial-intelligence/2/g/solution.md)
