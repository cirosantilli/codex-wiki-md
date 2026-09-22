<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Print a prefix while following the [linked list](../../../../../linked-list.md), counting how many closing parentheses remain. The final reciprocal can be printed without parentheses.
```
PROCEDURE printCF(f: fraction);
VAR p: fraction; opened: INTEGER;
BEGIN
  p := f; opened := 0;
  Out.Int(p.head, 0);
  p := p.tail;
  WHILE p # NIL DO
    IF p.tail = NIL THEN
      Out.String("+1/"); Out.Int(p.head, 0)
    ELSE
      Out.String("+1/("); Out.Int(p.head, 0);
      opened := opened + 1
    END;
    p := p.tail
  END;
  WHILE opened > 0 DO
    Out.String(")"); opened := opened - 1
  END
END printCF;
```
The first [loop invariant](../../../../../loop-invariant.md) says that `p` is the next unprinted [linked list node](../../../../../linked-list-node.md), the printed text is the correct expression prefix, and `opened` counts its unmatched opening parentheses. The final node contributes no opening parenthesis; the second [loop invariant](../../../../../loop-invariant.md) says that precisely `opened` closing parentheses remain. Thus `[1,2,3,4,5]` produces **`1+1/(2+1/(3+1/(4+1/5)))`**. A singleton prints just its head. If the first head is negative, its leading minus remains a valid prefix; subsequent heads are positive.

The precondition is a finite nonempty [continued fraction](../../../../../continued-fraction.md) list. Every dereference is made only for a nonnull pointer. The procedure uses $O(1)$ auxiliary space and time linear in the number of nodes, apart from printing their digits. The source's claimed strict upper bound $x_0+1$ has an exception under its stated definition: `[x0,1]` represents $x_0+1$. None of these algorithms relies on that incorrect strict bound.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [3](../../3.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2016](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
