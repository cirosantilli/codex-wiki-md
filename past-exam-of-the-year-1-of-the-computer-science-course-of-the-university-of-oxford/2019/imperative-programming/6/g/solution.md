<h1 id="6/g/solution">Solution</h1>

↑ **Parent:** [G](../g.md)

Make two separate character [iterators](../../../../../iterator.md) so that scanning uppercase letters does not consume the lowercase pass:
```
def upperLower(s: String): Iterator[Char] = {
  val upper = new FilterIterator[Char]((c: Char) => c.isUpper, s.iterator)
  val lower = new FilterIterator[Char]((c: Char) => c.isLower, s.iterator)
  new ConcatIterator[Char](upper, lower)
}
```
Each filtering [iterator](../../../../../iterator.md) preserves the original order of its selected characters. Concatenation therefore yields **all uppercase letters in source order, then all lowercase letters in source order**, omitting other characters. The two `s.iterator` calls are essential: reusing a single consuming [iterator](../../../../../iterator.md) would let the first pass discard lowercase characters before the second pass could return them. Construction remains lazy; an empty [string](../../../../../string.md) yields an exhausted [iterator](../../../../../iterator.md) without a special case.

## ↑ Ancestors (12)

1. [G](../g.md)
2. [6](../../6.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2019](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
