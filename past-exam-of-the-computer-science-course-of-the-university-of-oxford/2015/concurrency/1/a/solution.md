<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [unique fixed point principle](../../../../../unique-fixed-point-principle.md) says that a suitably [guarded recursion](../../../../../guarded-recursion.md) has a unique solution in the chosen [CSP semantic model](../../../../../csp-semantic-model.md). In particular, for a guarded process expression $F(X)$,

$$
\boxed{P=F(P),\quad Q=F(Q)\quad\Longrightarrow\quad P=Q.}
$$

The same principle applies to a mutually recursive system: two tuples satisfying the same guarded equations are componentwise equal. Thus an algebraic proof may show that a candidate satisfies the defining equations, instead of comparing arbitrarily long executions individually.

A [guarded recursion](../../../../../guarded-recursion.md) must make visible progress before re-entering its recursive dependency. For an equation built from [CSP prefixing](../../../../../csp-prefixing.md) and [CSP choice](../../../../../csp-choice.md), the usual sufficient condition is that every recursive occurrence lies behind a visible [CSP prefixing](../../../../../csp-prefixing.md) operation. For mutually recursive equations, every dependency cycle must pass such a guard. The guard must survive enclosing operators: an event subsequently removed by [CSP hiding](../../../../../csp-hiding.md) does not provide visible progress. Equivalently, in the usual semantic formulation the recursion functional must be contractive in observable depth. Merely seeing an arrow somewhere before the variable is insufficient.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Concurrency](../../../concurrency-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
