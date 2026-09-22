<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Create only the missing nodes along the required [trie](../../../../../trie.md) path, and mark its last node complete.
```
def add(w: String): Unit = {
  var t: Trie = this
  var i = 0
  while (i < w.length) {
    val k = toIndex(w.charAt(i))
    if (t.children(k) == null) t.children(k) = new Trie
    t = t.children(k)
    i += 1
  }
  t.complete = true
}
```
The [loop invariant](../../../../../loop-invariant.md) is that the path for `w.take(i)` exists and ends at `t`, while the [set](../../../../../set-split.md) of complete words remains unchanged from entry. A fresh node has all children null and `complete == false`, so creating an unfinished path introduces no stored word. The [loop variant](../../../../../loop-variant.md) is $w.length-i$. At termination the full path exists; setting its final flag gives

$$
\boxed{D_{\mathrm{after}}=D_{\mathrm{before}}\cup\{w\}.}
$$

Existing paths and terminal flags are untouched, so adding an existing word is idempotent. Adding the empty [string](../../../../../string.md) marks the root. The [time complexity](../../../../../time-complexity.md) is $O(1+|w|)$ because the alphabet size is fixed; at most $|w|$ new [trie](../../../../../trie.md) nodes are allocated.

## ↑ Ancestors (12)

1. [B](../b.md)
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
