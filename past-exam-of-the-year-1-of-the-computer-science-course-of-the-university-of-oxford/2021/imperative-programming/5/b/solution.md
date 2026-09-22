<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Assume the supplied [hash function](../../../../../hash-function.md) is stable and produces valid table indices. The [representation invariant](../../../../../representation-invariant.md) places each name in its hashed bucket, permits at most one entry per name, and requires finite acyclic, disjoint bucket chains.

```
def store(name: String, number: String): Unit = {
  val bucket = hash(name)
  val entry = find(name, table(bucket))
  if (entry == null) {
    table(bucket) = new Entry(name, number, table(bucket))
  } else {
    entry.number = number
  }
}
```

If the key exists, updating its associated number implements map override without creating a duplicate entry. Otherwise a new entry is prepended to the correct bucket and leaves every existing mapping unchanged. Its immutable name preserves bucket membership. Thus **the mapping afterwards is the old mapping overridden at precisely the supplied key**. [Hash collisions](../../../../../hash-collision.md) between different names do not imply key equality and are handled by [separate chaining](../../../../../separate-chaining.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [5](../../5.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2021](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
