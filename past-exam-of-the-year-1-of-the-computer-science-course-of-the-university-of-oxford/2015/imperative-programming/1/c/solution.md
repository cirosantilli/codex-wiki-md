<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use an explicit [stack](../../../../../stack-data-structure.md) of handles. Push the right [subtree](../../../../../subtree.md) first, so that the left [subtree](../../../../../subtree.md) is removed first by the [LIFO stack](../../../../../stack-data-structure.md).
```
PROCEDURE PreorderIter(t: Tree; VAR out: ARRAY OF INTEGER;
                       VAR count: INTEGER;
                       VAR stack: ARRAY OF Tree);
VAR top: INTEGER; p: Tree;
BEGIN
  count := 0; top := 1; stack[0] := t;
  WHILE top > 0 DO
    DEC(top); p := stack[top];
    IF p = 0 THEN
      out[count] := 0; INC(count)
    ELSE
      out[count] := 1; INC(count);
      stack[top] := nodes[p-1].right; INC(top);
      stack[top] := nodes[p-1].left; INC(top)
    END
  END
END PreorderIter;
```
The [loop invariant](../../../../../loop-invariant.md) says that the already written prefix, followed by the [preorder traversals](../../../../../preorder-traversal.md) of the pending [subtrees](../../../../../subtree.md) in top-to-bottom [stack](../../../../../stack-data-structure.md) order, equals the entire required output. Popping a [leaf of a rooted tree](../../../../../leaf-of-a-rooted-tree.md) transfers one marker to the prefix. Popping a fork transfers its marker and replaces its remaining work by left then right [subtree](../../../../../subtree.md) work. Both preserve the [loop invariant](../../../../../loop-invariant.md). The number of as-yet-unwritten [vertices](../../../../../vertex-graph-theory.md) decreases by one per iteration, proving termination.

$$
\boxed{\text{Push right, push left; pop and emit until the stack is empty.}}
$$

The [time complexity](../../../../../time-complexity.md) is linear in the output length. The maximum [stack](../../../../../stack-data-structure.md) size is at most one plus the [height of a binary tree](../../../../../height-of-a-binary-tree.md).

## ↑ Ancestors (12)

1. [C](../c.md)
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
