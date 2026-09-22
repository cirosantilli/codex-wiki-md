<h1 id="1/g/solution">Solution</h1>

↑ **Parent:** [G](../g.md)

Let $s(T)$ be the number of nodes and let the [left-size potential of a binary tree](../../../../../left-size-potential-of-a-binary-tree.md) be

$$
L(\varnothing)=0,\qquad L(T)=s(T.left)+L(T.right).
$$

Equivalently $L(T)$ counts nodes outside the right spine, so $0\leq L(T)\leq s(T)$; for a nonempty [binary tree](../../../../../binary-tree.md) of $n$ nodes, $L(T)\leq n-1$.

For the [right tree rotation](../../../../../right-tree-rotation.md) in part (f), write the old shape as $((A,x,B),y,C)$. Before and after,

$$
L_{\rm before}=s(A)+1+s(B)+L(C),\qquad
L_{\rm after}=s(A)+s(B)+L(C).
$$

Thus each inner iteration decreases $L$ by exactly one, making $L$ an inner [loop variant](../../../../../loop-variant.md). Removing a root with empty left [subtree](../../../../../subtree.md) leaves $L$ unchanged and decreases $s$ by one. Therefore $s+L$ decreases on every rotation or visit, while $s$ decreases on every completed outer iteration. These are bounds used for proof; the program never computes them.

There are exactly $n$ visits and exactly $L(T_0)$ rotations, since the final empty [binary tree](../../../../../binary-tree.md) has potential zero. Counting constant-cost `p`,

$$
\boxed{\text{rotations}+\text{visits}=n+L(T_0)\leq2n-1\quad(n>0),\qquad T(n)=\Theta(n+1).}
$$

The nested loops therefore have linear total [running time](../../../../../running-time.md), despite one outer iteration potentially making many rotations.

## ↑ Ancestors (12)

1. [G](../g.md)
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
