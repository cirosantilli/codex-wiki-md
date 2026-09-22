<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Perform a [depth-first traversal](../../../../../depth-first-search.md), retaining the path's letters in a buffer. A terminal node must be printed before its children, so a word precedes its proper extensions in [lexicographic order](../../../../../lexicographic-order.md).
```
VAR word: ARRAY N OF CHAR;

PROCEDURE Visit(t: Trie; depth: INTEGER);
VAR j, c: INTEGER;
BEGIN
  IF t # NIL THEN
    IF t.terminal THEN
      j := 0;
      WHILE j < depth DO
        Out.Char(word[j]); j := j+1
      END;
      Out.Ln
    END;
    c := 0;
    WHILE c < 26 DO
      IF t.child[c] # NIL THEN
        word[depth] := CHR(ORD("a")+c);
        Visit(t.child[c], depth+1)
      END;
      c := c+1
    END
  END
END Visit;

PROCEDURE PrintTrie(t: Trie);
BEGIN
  Visit(t, 0)
END PrintTrie;
```
The [recursion invariant](../../../../../recursion-invariant.md) is that `word[0..depth)` spells the path to `t`. The child loop's [loop invariant](../../../../../loop-invariant.md) says children with indices below `c` have been completely printed. Each edge appends its lowercase label; each terminal flag prints exactly one represented [string](../../../../../string.md). All words therefore appear once, in lowercase. The output loop prints precisely the prefix of length `depth`; no terminating zero needs storing in this buffer.

**An `N`-character buffer suffices for words of length at most `N`.** At depth `N` there can be no child, so `word[N]` is never accessed. A terminal root prints an empty line; a `NIL` root prints nothing. The [running time](../../../../../running-time.md) is linear in allocated nodes plus the number of printed characters, since the alphabet size is fixed at 26.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
3. [Imperative programming (resit)](../../../imperative-programming-resit-split.md)
4. [2016](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
