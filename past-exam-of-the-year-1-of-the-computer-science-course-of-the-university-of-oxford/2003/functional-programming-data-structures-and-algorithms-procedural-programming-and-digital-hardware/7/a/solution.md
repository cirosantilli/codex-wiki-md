<h1 id="7/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The representation invariant for the [array](../../../../../array-data-structure.md) [stack](../../../../../stack-data-structure.md) is $0\leq s.n\leq N$, with live entries at positions $0,\ldots,s.n-1$ and the top at `s.n-1` when nonempty. The following [Oberon](../../../../../oberon-programming-language.md) procedures use the given [data types](../../../../../data-type.md):

```
PROCEDURE makeEmpty(VAR s : stack);
BEGIN
  s.n := 0
END makeEmpty;

PROCEDURE isEmpty(s : stack) : BOOLEAN;
BEGIN
  RETURN s.n = 0
END isEmpty;

PROCEDURE push(VAR s : stack; t : node);
BEGIN
  s.a[s.n] := t;
  s.n := s.n+1
END push;

PROCEDURE pop(VAR s : stack) : node;
VAR t : node;
BEGIN
  s.n := s.n-1;
  t := s.a[s.n];
  s.a[s.n] := NIL;
  RETURN t
END pop;
```

For `push`, the supplied [precondition](../../../../../precondition.md) `s.n < N` makes the old `s.n` a valid free index. For `pop`, the [precondition](../../../../../precondition.md) `s.n > 0` makes the decremented index the old top. Setting the vacated entry to `NIL` avoids retaining a reference to the removed [binary tree](../../../../../binary-tree.md); it does not deallocate that [binary tree](../../../../../binary-tree.md). `makeEmpty` need not clear inactive entries for the abstract [stack](../../../../../stack-data-structure.md) behavior. None of these procedures has a loop. Each changes or inspects a constant number of fields, so its logical work is [constant time](../../../../../constant-time.md); an implementation of the specified by-value `isEmpty` parameter may additionally copy the fixed-capacity record. The essential update rule is

$$
\boxed{\text{push writes then increments; pop decrements then reads}.}
$$

## ↑ Ancestors (12)

1. [A](../a.md)
2. [7](../../7.md)
3. [Functional programming, data structures and algorithms, procedural programming, and digital hardware](../../../functional-programming-data-structures-and-algorithms-procedural-programming-and-digital-hardware-split.md)
4. [2003](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
