<h1 id="8/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Join on equal middle components, produce the outer pair, and eliminate duplicate outputs. Using the variant declarations from part (a):

```
def compose1[X, Y, Z](r: Rel1[X, Y], s: Rel1[Y, Z]): Rel1[X, Z] = {
  val joined = (for {
    (x, y) <- r.pairs
    (middle, z) <- s.pairs
    if y == middle
  } yield (x, z)).distinct
  new Rel1[X, Z] {
    val pairs: List[(X, Z)] = joined
  }
}
```

Every produced pair has a witness `y` with both required input pairs, proving soundness. Conversely, any witness for a composed pair occurs in the two input lists, so the nested traversal produces that pair; `.distinct` retains one occurrence, proving completeness. Thus **the result represents $S\circ R$**, with each pair listed once, even if either input lists duplicates or several witnesses yield the same outer pair. Equality of middle values is assumed to implement the relation's intended key equality. The nested join examines $|r.pairs|\,|s.pairs|$ candidate pairs before duplicate elimination.

## ↑ Ancestors (12)

1. [B](../b.md)
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
