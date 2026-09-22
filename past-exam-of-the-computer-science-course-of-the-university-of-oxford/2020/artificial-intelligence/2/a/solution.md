<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a finite [constraint satisfaction problem](../../../../../constraint-satisfaction-problem.md), remove values violating unary restrictions before starting. The following [backtracking](../../../../../backtracking.md) [algorithm](../../../../../algorithm-split.md) makes independent copies of [constraint domains](../../../../../constraint-domain.md) at each branch, so failed [forward checking](../../../../../forward-checking.md) cannot contaminate a sibling branch.

```
SOLVE(P):
    D := domains of P after unary filtering
    if some D[X] is empty: return failure
    return SEARCH({}, D)

SEARCH(assignment, D):
    if every variable is assigned: return assignment
    X := SELECT-UNASSIGNED-VARIABLE(assignment, D, P)
    for v in ORDER-DOMAIN-VALUES(X, assignment, D, P):
        if X=v is compatible with the current assignment:
            next_assignment := assignment extended by X=v
            next_domains := a deep copy of D
            next_domains[X] := {v}
            if INFERENCES(X, v, next_assignment, next_domains, P) succeeds:
                result := SEARCH(next_assignment, next_domains)
                if result is not failure: return result
    return failure
```

SELECT-UNASSIGNED-VARIABLE implements [minimum remaining values](../../../../../minimum-remaining-values.md): choose an unassigned [variable](../../../../../variable-mathematics.md) with the smallest current [constraint domain](../../../../../constraint-domain.md). Break ties by the [degree heuristic](../../../../../degree-heuristic.md), choosing the [variable](../../../../../variable-mathematics.md) constrained to the greatest number of other unassigned [variables](../../../../../variable-mathematics.md); a fixed final tie rule makes execution reproducible. ORDER-DOMAIN-VALUES may use any complete ordering; ascending values suffice here.

INFERENCES implements [forward checking](../../../../../forward-checking.md): for each unassigned neighbor $Y$ of $X$, remove every value incompatible with $X=v$, and fail if any [constraint domain](../../../../../constraint-domain.md) becomes empty. For higher-arity constraints, reject any completely instantiated violation and use a sound chosen filtering rule; the stated neighbor test is the usual binary case. [Forward checking](../../../../../forward-checking.md) never removes a value used by a possible extension of the current assignment. Exhausting every surviving value therefore makes this finite [backtracking](../../../../../backtracking.md) procedure both sound and complete.[§2.3, opening paragraphs: filtering neighbors after assignment](../../../../../cs-188-constraint-filtering-notes.md)[§2.4, Minimum Remaining Values](../../../../../cs-188-constraint-ordering-and-structure-notes.md)

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Artificial intelligence](../../../artificial-intelligence-split.md)
4. [2020](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
