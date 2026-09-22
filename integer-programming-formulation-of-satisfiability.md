# Integer programming formulation of satisfiability

↑ **Parent:** [Boolean satisfiability problem](boolean-satisfiability-problem.md)

Encode each truth value by $t_k\in\{0,1\}$. A positive [Boolean literal](boolean-literal.md) has value $t_k$ and its negation has value $1-t_k$. The sum of literal values in a clause is at least one exactly when that clause is true. Thus the displayed inequalities, with objective zero, express [Boolean satisfiability](boolean-satisfiability-problem.md) as a binary [integer programming](integer-programming.md) feasibility problem. For [maximum satisfiability](maximum-satisfiability.md), introduce $q_i\in\{0,1\}$ with $q_i\leq\sum_{\ell\in C_i}L_\ell(t)$ and maximize $\sum_iq_i$. False clauses force zero indicators; true clauses permit indicators one, and maximization selects all of them. Hence the optimal objective equals the maximum number of true clauses.

## ↑ Ancestors (9)

1. [Boolean satisfiability problem](boolean-satisfiability-problem.md)
2. [NP-completeness](np-completeness.md)
3. [NP-hardness](np-hardness.md)
4. [Polynomial-time many-one reduction](polynomial-time-many-one-reduction.md)
5. [Polynomial-time reduction](polynomial-time-reduction.md)
6. [Computational complexity theory](computational-complexity-theory.md)
7. [Theoretical computer science](theoretical-computer-science.md)
8. [Computer science](computer-science-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-35/4/solution.md)
