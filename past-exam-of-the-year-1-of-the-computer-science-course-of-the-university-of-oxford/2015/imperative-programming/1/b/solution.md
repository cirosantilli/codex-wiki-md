<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For parts (b)–(e), use [array indices](../../../../../array-index.md) as [tree](../../../../../tree-graph-theory-split.md) handles. This also makes the shared storage in part (d) type-correct: both pending handles and output markers occupy [integer](../../../../../integer-split.md) cells. Zero denotes a [leaf of a rooted tree](../../../../../leaf-of-a-rooted-tree.md); a positive handle $t$ denotes a fork whose children are in `nodes[t-1]`. Only finite acyclic structures are admitted. An allocated fork's children are themselves valid handles.
```
CONST MaxForks = 100000;
TYPE Tree = INTEGER;
     Node = RECORD left, right: Tree END;
     Arena = ARRAY MaxForks OF Node;
VAR nodes: Arena;
    used: INTEGER;

PROCEDURE NewFork(left, right: Tree): Tree;
BEGIN
  ASSERT(used < MaxForks);
  nodes[used].left := left; nodes[used].right := right;
  INC(used);
  RETURN used
END NewFork;

PROCEDURE Preorder(t: Tree; VAR out: ARRAY OF INTEGER;
                   VAR count: INTEGER);
  PROCEDURE Visit(p: Tree);
  BEGIN
    IF p = 0 THEN
      out[count] := 0; INC(count)
    ELSE
      out[count] := 1; INC(count);
      Visit(nodes[p-1].left); Visit(nodes[p-1].right)
    END
  END Visit;
BEGIN
  count := 0; Visit(t)
END Preorder;
```
Initialize `used := 0` before constructing any [trees](../../../../../tree-graph-theory-split.md); `NewFork` allocates within this arena. The fixed capacity is an implementation parameter and may be replaced by a dynamically allocated arena. The returned prefix `out[0..count)` encodes [Boolean](../../../../../boolean-data-type.md) values by $0=\mathrm{False}$ and $1=\mathrm{True}$. This encoding is part of the chosen representation, not a conversion of a [pointer](../../../../../pointer-computer-programming.md) into a [Boolean](../../../../../boolean-data-type.md) value.

The [recursion invariant](../../../../../recursion-invariant.md) is that `Visit(p)` appends exactly the [preorder traversal](../../../../../preorder-traversal.md) of the [subtree](../../../../../subtree.md) represented by `p`. If the [full binary tree](../../../../../full-binary-tree.md) has $I$ forks, it has $I+1$ [leaves](../../../../../leaf-of-a-rooted-tree.md); hence

$$
\boxed{\mathrm{count}=2I+1,\qquad \mathrm{out}[0..\mathrm{count})=P(t)\text{ encoded by }0,1.}
$$

Each occurrence is visited once, using linear [time complexity](../../../../../time-complexity.md) and a [call stack](../../../../../call-stack.md) bounded by the [height of a binary tree](../../../../../height-of-a-binary-tree.md). The arena is the input representation, not an extra copy made by the traversal.

## ↑ Ancestors (12)

1. [B](../b.md)
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
