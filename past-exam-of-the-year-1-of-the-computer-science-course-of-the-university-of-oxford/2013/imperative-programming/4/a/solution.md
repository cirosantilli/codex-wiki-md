<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Traverse the [trie](../../../../../trie.md) along the input [string](../../../../../string.md), stopping as soon as the required child is absent. All words and letter collections in this question are assumed to use only lowercase letters `a` through `z`; this is the alphabet represented by the given child [array](../../../../../array-data-structure.md). Put the following methods inside the supplied `Trie` class.
```
def contains(w: String): Boolean = {
  var t: Trie = this
  var i = 0
  while (i < w.length && t != null) {
    t = t.children(toIndex(w.charAt(i)))
    i += 1
  }
  t != null && t.complete
}
```
The [loop invariant](../../../../../loop-invariant.md) is that `t` is the [trie](../../../../../trie.md) node reached by the prefix `w.take(i)`, or null if that prefix has no path, with $0\leq i\leq w.length$. If `t` is null, no extension can be a stored word. Otherwise, following the next character preserves the [loop invariant](../../../../../loop-invariant.md). The [loop variant](../../../../../loop-variant.md) is $w.length-i$. At exit,

$$
\boxed{contains(w)\iff\text{the full path exists and its terminal flag is true}.}
$$

A prefix that exists but is not complete must return false. The empty [string](../../../../../string.md) is present exactly when the root's `complete` flag is true. The [time complexity](../../../../../time-complexity.md) is $O(1+|w|)$, with constant [auxiliary space](../../../../../auxiliary-space.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [4](../../4.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2013](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
