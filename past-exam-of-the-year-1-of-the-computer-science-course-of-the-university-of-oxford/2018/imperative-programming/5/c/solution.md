<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Return the new root of the affected [subtree](../../../../../subtree.md), assigning that result back to the parent's child reference:
```
def addToTree(word: String, t: Tree): Tree = {
  require(word != null)
  if (t == null) new Tree(word, 1)
  else {
    val c = word.compareTo(t.word)
    if (c < 0) t.left = addToTree(word, t.left)
    else if (c > 0) t.right = addToTree(word, t.right)
    else {
      require(t.count < Int.MaxValue)
      t.count += 1
    }
    t
  }
}
// Updating the whole structure uses: root = addToTree(word, root)
```
Assume the input [binary search tree](../../../../../binary-search-tree.md) satisfies part (b)'s [representation invariant](../../../../../representation-invariant.md) and, if the key already occurs, its count can be incremented. [Structural induction](../../../../../structural-induction.md) proves the [postcondition](../../../../../postcondition.md). For an empty [subtree](../../../../../subtree.md), the fresh entry represents one occurrence. Otherwise the word comparison identifies the only possible child [subtree](../../../../../subtree.md) containing the word. The [recursive call](../../../../../recursive-call.md) adds exactly one occurrence there, preserving the inherited strict bounds; in the equal case only the count changes. The number of entries in the current [subtree](../../../../../subtree.md) strictly decreases in each [recursive call](../../../../../recursive-call.md), proving [algorithm termination](../../../../../algorithm-termination.md). **The returned [binary search tree](../../../../../binary-search-tree.md) represents the old [multiset](../../../../../multiset.md) plus one occurrence of `word`.** With height $h$, at most $h+1$ comparisons are made; without balancing this can be linear in the number of words. Actual comparison work also depends on the compared [string data type](../../../../../string-data-type.md) lengths.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [5](../../5.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2018](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
