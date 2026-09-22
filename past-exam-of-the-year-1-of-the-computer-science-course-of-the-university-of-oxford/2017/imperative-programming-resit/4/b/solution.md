<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Remove zero nodes while retaining every nonzero node and its order:

```
PROCEDURE normalise(VAR r: poly);
VAR p,prev: poly;
BEGIN
  p := r; prev := NIL;
  WHILE p # NIL DO
    IF p.coeff = 0 THEN
      IF prev = NIL THEN r := p.next
      ELSE prev.next := p.next END
    ELSE
      prev := p
    END;
    p := p.next
  END
END normalise;
```

At each step, the processed prefix contains precisely the nonzero nodes already examined, and `prev` is its final node or `NIL`. Thus removal at the head, consecutive removals and removal of every node are handled. This [linked-list deletion](../../../../../linked-list-deletion.md) pass takes linear time in the original node count. It does not by itself combine duplicate powers.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [4](../../4.md)
3. [Imperative programming (resit)](../../../imperative-programming-resit-split.md)
4. [2017](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
