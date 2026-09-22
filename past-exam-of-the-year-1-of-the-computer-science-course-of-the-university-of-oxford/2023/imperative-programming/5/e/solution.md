<h1 id="5/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Insert a singleton mapping, retrieve a stored representative, or relabel every occurrence of the second block's old representative:

```
def makeSet(x: Int): Unit = {
  require(isInMap(x) == -1, "element already present")
  require(used < capacity, "capacity exhausted")
  elements(used) = x
  representatives(used) = x
  used += 1
}

def find(x: Int): Int = {
  val i = isInMap(x)
  require(i >= 0, "unknown element")
  representatives(i)
}

def union(x: Int, y: Int): Unit = {
  val keep = find(x)
  val replace = find(y)
  if (keep != replace) {
    var i = 0
    while (i < used) {
      if (representatives(i) == replace) representatives(i) = keep
      i += 1
    }
  }
}
```

For `makeSet`, the new key is absent, its representative is itself, and old mappings are unchanged. `find` is a read-only [linear search](../../../../../linear-search.md). In `union`, **snapshot both representatives before changing any cell**: recomputing the representative of `y` during the scan could change the criterion halfway through. The [loop invariant](../../../../../loop-invariant.md) says that every processed index already has its specified final representative and every unprocessed index still has its old representative. The cached labels make this assertion stable.

At exit the abstract [postcondition](../../../../../postcondition.md) in part (a) holds. The surviving representative was already a fixed point and belongs to its old block; every member of the replaced block, including its old representative key, now maps to it. Thus idempotence and key uniqueness are preserved. Duplicate insertions, absent-element operations and capacity overflow fail before changing the map. Each operation is $O(used)$ in the worst case, except that a same-block union can skip the relabel scan after its lookups. Storage is $O(capacity)$. These bounds follow from the chosen parallel-array [quick-find](../../../../../quick-find.md) representation; no parent-pointer optimization is being assumed.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [5](../../5.md)
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
