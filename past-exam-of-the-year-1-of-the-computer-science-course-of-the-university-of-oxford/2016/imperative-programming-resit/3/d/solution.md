<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Allocate nodes only as required, explicitly initializing every field:
```
PROCEDURE Make(VAR t: Trie);
VAR c: INTEGER;
BEGIN
  NEW(t); t.terminal := FALSE; c := 0;
  WHILE c < 26 DO t.child[c] := NIL; c := c+1 END
END Make;

PROCEDURE AddTail(VAR t: Trie; s: ARRAY OF CHAR; i: INTEGER);
BEGIN
  IF t = NIL THEN Make(t) END;
  IF s[i] = 0X THEN
    t.terminal := TRUE
  ELSE
    AddTail(t.child[Index(s[i])], s, i+1)
  END
END AddTail;

PROCEDURE Add(VAR t: Trie; s: ARRAY OF CHAR);
BEGIN
  AddTail(t, s, 0)
END Add;
```
Here `0X` is the zero character, and `s` must contain its terminator within its [array](../../../../../array-data-structure.md) bounds. `Make` establishes that the first `c` child fields are `NIL` as its [loop invariant](../../../../../loop-invariant.md). Passing `t` by reference lets the base allocation replace a missing root or child pointer.

For correctness, use [induction](../../../../../mathematical-induction.md) on the number of characters before the terminator. At length zero, setting `terminal` adds exactly the empty suffix. Otherwise the chosen child stores exactly words with the required next letter, and the [induction hypothesis](../../../../../induction-hypothesis.md) adds the remaining suffix while preserving all other words. Thus **the resulting [set](../../../../../set-split.md) is the old [set](../../../../../set-split.md) union the supplied word, ignoring case**. Repeated insertion changes no word membership. A newly allocated path reaches the newly terminal node, preserving the canonical [representation invariant](../../../../../representation-invariant.md) after the procedure finishes. The [running time](../../../../../running-time.md) is $O(1+\ell)$ for a word of length $\ell$, using $O(1+\ell)$ [call stack](../../../../../call-stack.md) space without optimization.

## ↑ Ancestors (12)

1. [D](../d.md)
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
