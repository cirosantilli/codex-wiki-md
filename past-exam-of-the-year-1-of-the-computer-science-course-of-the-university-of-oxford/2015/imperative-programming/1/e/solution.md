<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Maintain a cursor to the first unread marker. A fork consumes its own marker and then two complete encodings, in left-to-right order.
```
PROCEDURE Decode(VAR code: ARRAY OF INTEGER;
                 VAR pos: INTEGER): Tree;
VAR marker: INTEGER; left, right: Tree;
BEGIN
  marker := code[pos]; INC(pos);
  IF marker = 0 THEN RETURN 0 END;
  ASSERT(marker = 1);
  left := Decode(code, pos);
  right := Decode(code, pos);
  RETURN NewFork(left, right)
END Decode;
```
Start with `pos := 0; t := Decode(code, pos)`, with sufficient unused arena space. The valid-input [precondition](../../../../../precondition.md) ensures that every read exists and every fork has two encoded [subtrees](../../../../../subtree.md). Evaluating the two recursive calls in separate statements fixes their order.

[Structural induction](../../../../../structural-induction.md) shows that decoding $P(t)$ reconstructs the same [binary tree](../../../../../binary-tree.md) shape and leaves the cursor just after its encoding. The [tree](../../../../../tree-graph-theory-split.md) handles need not coincide with the original handles: the abstract [tree](../../../../../tree-graph-theory-split.md) does. The result is

$$
\boxed{\operatorname{Decode}(P(t))\cong t,\quad\mathrm{pos}=|P(t)|.}
$$

The [time complexity](../../../../../time-complexity.md) is linear in the encoding length, with [call stack](../../../../../call-stack.md) space bounded by the [height of a binary tree](../../../../../height-of-a-binary-tree.md).

## ↑ Ancestors (12)

1. [E](../e.md)
2. [1](../../1.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2015](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
