<h1 id="8/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

A `Rel3` provides only a membership test for a supplied pair. It gives no way to enumerate the finite middle carrier `Y`, enumerate one element's relatives, or even obtain a first value of type `Y`. Finiteness alone supplies no generic enumeration operation. To answer the existential query for the composed relation, **supply a complete finite enumeration of the middle carrier explicitly**:

```
def compose3[X, Y, Z](r: Rel3[X, Y], s: Rel3[Y, Z],
                      middleValues: List[Y]): Rel3[X, Z] = {
  val witnesses = middleValues.distinct
  new Rel3[X, Z] {
    def related(x: X, z: Z): Boolean =
      witnesses.exists(y => r.related(x, y) && s.related(y, z))
  }
}
```

The [precondition](../../../../../precondition.md) is that `middleValues` contains every admissible middle value, or at least every possible witness. Extra irrelevant values do not change the answer if the two membership tests are defined for them. The [postcondition](../../../../../postcondition.md) is precisely $\exists y\in Y:\ R(x,y)\land S(y,z)$. `.exists` and `&&` use [short-circuit evaluation](../../../../../short-circuit-evaluation.md); with an empty middle carrier, the answer is false. Each query uses at most $|Y|$ pairs of membership tests, apart from the one-time duplicate elimination.

An alternative interface can expose `def rightDomain: List[Y]` together with the first predicate, with an explicit completeness contract. Such an output position is incompatible with retaining a contravariant `Y` in that extended trait, so its variance must be reconsidered. Passing the enumeration separately leaves the safe base `Rel3[-X,-Y]` unchanged.

The information gap is substantive. A black-box algorithm making finitely many membership queries cannot rule out a witness at an unexamined middle value: two relations can agree on every inspected pair while differing only by a fresh witness that makes the composition true. A finite but unenumerated carrier can be enlarged to include that witness. A complete explicit enumeration, a known traversable carrier, or an equivalent relatives-enumeration interface removes this obstruction. This is [finite-domain composition from relation predicates](../../../../../finite-domain-composition-from-relation-predicates.md), rather than a problem solvable merely by nesting the two Boolean-valued methods.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [8](../../8.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2023](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
