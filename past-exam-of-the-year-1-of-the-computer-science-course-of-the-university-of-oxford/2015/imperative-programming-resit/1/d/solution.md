<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Split the half-open [array](../../../../../array-data-structure.md) segment at its midpoint, using one entry for the root:
```
PROCEDURE MakeTree(VAR u: ARRAY OF INTEGER;
                   a, b: INTEGER): Tree;
VAR m: INTEGER; t: Tree;
BEGIN
  IF a = b THEN RETURN NIL END;
  m := a + (b-a) DIV 2;
  NEW(t);
  t.label := u[m];
  t.left := MakeTree(u, a, m);
  t.right := MakeTree(u, m+1, b);
  RETURN t
END MakeTree;
```
The [precondition](../../../../../precondition.md) is $0\leq a\leq b\leq\operatorname{LEN}(u)$. Set $n=b-a$. For $n>0$ the child sizes are $\lfloor n/2\rfloor$ and $n-1-\lfloor n/2\rfloor$, differing by at most one. The same construction in both [subtrees](../../../../../subtree.md) proves [subtree-size balance](../../../../../subtree-size-balance.md) at every node. [Structural induction](../../../../../structural-induction.md) also gives the [inorder traversal](../../../../../inorder-traversal.md) $u[a..m)$, followed by $u[m]$, followed by $u[m+1..b)$, hence precisely $u[a..b)$; no [sortedness](../../../../../sortedness.md) assumption is needed.

Exactly $n$ records are allocated. Each nonempty [recursive call](../../../../../recursive-call.md) makes two child calls, so there are $2n+1$ calls including empty segments. Under constant-cost allocation and [reference parameter](../../../../../reference-parameter.md) passing,

$$
\boxed{T(n)=\Theta(n+1),\quad\operatorname{inorder}(t)=u[a..b),\quad t\text{ is nearly balanced}.}
$$

For positive $n$ this is proportional to $b-a$; the empty case takes constant time. The [call stack](../../../../../call-stack.md) has $O(1+\log(n+1))$ depth.

## ↑ Ancestors (12)

1. [D](../d.md)
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
