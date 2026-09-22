<h1 id="8/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For each requested `x`, enumerate its middle relatives and then each middle value's relatives in the second relation:

```
def compose2[X, Y, Z](r: Rel2[X, Y], s: Rel2[Y, Z]): Rel2[X, Z] =
  new Rel2[X, Z] {
    def relatives(x: X): List[Z] =
      r.relatives(x).flatMap(y => s.relatives(y)).distinct
  }
```

A returned `z` is present exactly when some enumerated `y` witnesses the two relation memberships. Conversely, every such witness appears in `r.relatives(x)`, and its `z` appears in `s.relatives(y)`, so no composed relative is omitted. `.distinct` removes repeated endpoints, including repetitions produced through different witnesses. **This is the same [composition of relations](../../../../../composition-of-relations.md) as part (b), represented one queried row at a time.** Neither the entire first carrier nor the entire result must be enumerated in advance. The relation operations must remain consistent while the returned view is used; changing their underlying state would make this a live view rather than a snapshot.

## ↑ Ancestors (12)

1. [C](../c.md)
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
