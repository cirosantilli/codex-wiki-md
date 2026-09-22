<h1 id="3/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

`AddTail` in part (d) is already [tail-recursive](../../../../../tail-recursion.md): the recursive call is the final action of its branch. The following loop follows a separate cursor so that the caller's root pointer is preserved:
```
PROCEDURE AddIter(VAR t: Trie; s: ARRAY OF CHAR);
VAR u: Trie; i, c: INTEGER;
BEGIN
  IF t = NIL THEN Make(t) END;
  u := t; i := 0;
  WHILE s[i] # 0X DO
    c := Index(s[i]);
    IF u.child[c] = NIL THEN Make(u.child[c]) END;
    u := u.child[c]; i := i+1
  END;
  u.terminal := TRUE
END AddIter;
```
The [loop invariant](../../../../../loop-invariant.md) is that `u` points to the node reached by the first `i` letters, all necessary nodes along that path exist, and no previously terminal node has lost its flag. Each iteration advances one character. At the terminator, marking `u` inserts exactly the desired [string](../../../../../string.md). Using `t := t.child[c]` as the cursor update would instead overwrite the caller's root through the `VAR` parameter. **This version has $O(1+\ell)$ [running time](../../../../../running-time.md) and constant auxiliary space**, apart from newly allocated nodes in the result.

## ↑ Ancestors (12)

1. [F](../f.md)
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
