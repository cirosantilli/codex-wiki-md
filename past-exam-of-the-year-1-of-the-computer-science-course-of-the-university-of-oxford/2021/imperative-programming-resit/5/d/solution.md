<h1 id="5/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For a remaining tree $T$, define the potential

$$
L(\varnothing)=0,\qquad L(T)=|T.left|+L(T.right).
$$

This counts the nodes not on the right spine, so $0\leq L(T)\leq |T|$. Consider a [right rotation](../../../../../right-tree-rotation.md) with old root $y$, left child $x$, and three untouched [subtrees](../../../../../subtree.md) $A,B,C$. Before the rotation the potential is

$$
1+|A|+|B|+L(C).
$$

After the rotation it is $|A|+|B|+L(C)$, so **each rotation decreases $L$ by exactly one** while preserving the number of remaining nodes. This supplies a nonnegative decreasing bound for the inner loop.

When the root has no left child, printing it and advancing to its right child leaves $L$ unchanged and decreases the remaining node count by one. Thus $|T|+L(T)$ decreases on every rotation and every removal, proving termination of the whole procedure. Over the entire execution there are exactly $N$ printed nodes and exactly $L(T_0)$ rotations, since the final potential is zero. Both quantities are at most $N$, so **the running time is $\Theta(N)$ for a nonempty tree**, with constant [auxiliary space](../../../../../auxiliary-space.md). The nested syntax does not imply quadratic time: it is the total potential decrease across all iterations that bounds the inner work. The potential is a proof device and is not computed by the running program.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [5](../../5.md)
3. [Imperative programming (resit)](../../../imperative-programming-resit-split.md)
4. [2021](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
