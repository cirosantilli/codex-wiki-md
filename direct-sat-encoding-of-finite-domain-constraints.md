# Direct SAT encoding of finite-domain constraints

↑ **Parent:** [Constraint satisfaction problem](constraint-satisfaction-problem.md)

Represent each original value choice $X_i=v$ by a [Boolean variable](boolean-variable.md) $p_{i,v}$ and impose an [exactly-one constraint](exactly-one-constraint.md) for each original [variable](variable-mathematics.md). For every forbidden tuple $(v_i)_{i\in S}$ of a constraint with scope $S$, add the [Boolean clause](clause-of-a-boolean-formula.md) $\bigvee_{i\in S}\neg p_{i,v_i}$. A complete original assignment satisfies every constraint exactly when its one-hot indicators satisfy all these [Boolean clauses](clause-of-a-boolean-formula.md): each forbidden-tuple [Boolean clause](clause-of-a-boolean-formula.md) excludes precisely that joint choice. A [satisfying assignment](satisfying-assignment.md) decodes by reading the unique true indicator for each original [variable](variable-mathematics.md).

For [constraint domain](constraint-domain.md) sizes $q_i$, pairwise uniqueness requires $\sum_i\binom{q_i}{2}$ [Boolean clauses](clause-of-a-boolean-formula.md). If a constraint has $f_C$ forbidden tuples and arity $r_C$, its contribution is $f_C$ [Boolean clauses](clause-of-a-boolean-formula.md) and $r_Cf_C$ [literal](boolean-literal.md) occurrences. Thus bounded arity gives a polynomial-size encoding in explicitly listed domains, whereas enumerating a succinct high-arity relation can be exponential in its description length. [Unit propagation](unit-propagation.md) on this encoding can be weaker than [arc consistency](arc-consistency.md) on the original [binary constraints](binary-constraint.md).

## ↑ Ancestors (7)

1. [Constraint satisfaction problem](constraint-satisfaction-problem.md)
2. [Search problem](search-problem.md)
3. [Computational problem](computational-problem.md)
4. [Computational complexity theory](computational-complexity-theory.md)
5. [Theoretical computer science](theoretical-computer-science-split.md)
6. [Computer science](computer-science-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2020/artificial-intelligence/2/e/solution.md)
