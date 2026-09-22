<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

An [Oberon](../../../../../oberon-programming-language.md) [pointer](../../../../../pointer-computer-programming.md) refers to a record containing an [integer](../../../../../integer-split.md) label and two [subtree](../../../../../subtree.md) references:
```
TYPE
  Tree = POINTER TO Node;
  Node = RECORD
    left, right: Tree;
    label: INTEGER
  END;
```
Use `NIL` for the empty [binary tree](../../../../../binary-tree.md), including either absent child. The [representation invariant](../../../../../representation-invariant.md) requires a finite, acyclic [binary tree](../../../../../binary-tree.md) with disjoint left and right [subtrees](../../../../../subtree.md). In particular, shared nodes would represent a different structure and invalidate destructive traversal arguments.

$$
\boxed{\texttt{Leaf}\longleftrightarrow\texttt{NIL},\qquad\texttt{Fork}\longleftrightarrow\text{one allocated record}.}
$$

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [Imperative programming (resit)](../../../imperative-programming-resit-split.md)
4. [2015](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
