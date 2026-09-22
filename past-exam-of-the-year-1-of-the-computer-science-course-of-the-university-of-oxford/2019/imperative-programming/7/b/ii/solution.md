<h1 id="7/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Make defensive copies on both entry and exit, while keeping the supplied `Dimension` class unchanged:
```
class Frame(d: Dimension) {
  require(d != null)
  private val saved = new Dimension(d.width, d.height)
  private val savedArea = saved.width * saved.height

  def area: Int = savedArea
  def dimension: Dimension = new Dimension(saved.width, saved.height)
  def isPortrait: Boolean = saved.height >= saved.width
}
```
The private stored dimensions have no aliases exposed to the caller and are never changed. Mutating the constructor argument affects only the caller's object; mutating a returned `Dimension` affects only a fresh copy. Consequently **the stored area is calculated once and stays equal to the stored dimensions' product**. This [defensive copying](../../../../../../defensive-copying.md) is sufficient because `Dimension` contains only primitive fields; a more deeply nested mutable structure could require a [deep copy](../../../../../../deep-copy.md) or an immutable representation.

The multiplication above deliberately retains the supplied class's `Int` arithmetic and accessor type. If an exact mathematical area outside that range is required, compute once with `saved.width.toLong * saved.height.toLong` and expose `Long` instead; avoiding aliases and avoiding [integer overflow](../../../../../../integer-overflow.md) are separate concerns.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [7](../../../7.md)
4. [Imperative programming](../../../../imperative-programming-split.md)
5. [2019](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
