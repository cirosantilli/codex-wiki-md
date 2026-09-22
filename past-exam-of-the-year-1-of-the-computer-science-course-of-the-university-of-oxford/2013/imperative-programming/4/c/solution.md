<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use [trie search with a letter multiset](../../../../../trie-search-with-a-letter-multiset.md). Counts avoid generating the same result repeatedly when the input contains equal letters. The [backtracking](../../../../../backtracking.md) explores a letter value once, irrespective of how many indistinguishable copies remain.
```
def allWords(ls: String): List[String] = {
  val left = new Array[Int](26)
  var i = 0
  while (i < ls.length) {
    left(toIndex(ls.charAt(i))) += 1
    i += 1
  }
  var out = List.empty[String]

  def visit(t: Trie, prefix: String): Unit = {
    if (t.complete) out = prefix :: out
    var k = 0
    while (k < 26) {
      val child = t.children(k)
      if (left(k) > 0 && child != null) {
        left(k) -= 1
        visit(child, prefix + toChar(k))
        left(k) += 1
      }
      k += 1
    }
  }

  visit(this, "")
  out.reverse
}
```
At entry to `visit`, `t` is reached by `prefix`, and `left(k)` is the input multiplicity of letter $k$ minus its multiplicity in `prefix`. All these counts are nonnegative. Each recursive call consumes one available letter, and restoration makes sibling calls see the same counts as before that child. The [recursion](../../../../../recursion-computer-science.md) therefore terminates at depth at most $|ls|$, even when the dictionary contains longer words.

A completed prefix is emitted once, and the traversal continues so that longer words with the same prefix are also found. Every emitted word is in the dictionary and uses at most the available multiplicities. Conversely, every dictionary word meeting those bounds has an existing [trie](../../../../../trie.md) path whose next letter has positive remaining count at every step; the traversal reaches its terminal node. A [trie](../../../../../trie.md) has a unique root path for each word, and each child is visited at most once per reached node. Therefore

$$
\boxed{out=\{w\in D:\forall c,\ \operatorname{count}_w(c)\leq\operatorname{count}_{ls}(c)\},\quad\text{without repetitions}.}
$$

The boxed expression specifies the [set](../../../../../set-split.md) of entries in the returned [list](../../../../../list-abstract-data-type.md), rather than its ordering. If the dictionary includes the empty [string](../../../../../string.md), the method includes it once. Counting costs $O(|ls|+26)$; visiting $R$ reachable nodes costs $O(26R)$ apart from [string](../../../../../string.md) copying and output construction. The presented immutable-prefix construction additionally costs the sum of the prefix lengths it constructs. The recursion depth is at most $|ls|$, and the letter-count [array](../../../../../array-data-structure.md) has fixed size.

## ↑ Ancestors (12)

1. [C](../c.md)
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
