<h1 id="e/3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

A subset is [compact](../../../../compact-space.md) if every cover of it by open sets of the ambient space has a [finite subcover](../../../../finite-subcover.md); equivalently use open sets of its [subspace topology](../../../../subspace-topology.md). A cover of $A\cup B$ separately covers $A$ and $B$. [Compactness](../../../../compact-space.md) of each supplies two finite collections, whose union is finite and covers $A\cup B$. If $A$ is closed in a [compact](../../../../compact-space.md) space, add the open complement of $A$ to any [open cover](../../../../open-cover.md) of $A$. [Compactness](../../../../compact-space.md) supplies a [finite subcover](../../../../finite-subcover.md) of the whole space, and discarding the complement leaves a finite cover of $A$.

For the enlarged space, every old open set is open in $C$ and has the same trace on $X$. The trace on $X$ of a new open set $V\cup\{\infty\}$ is $V$, which is open in $X$ because its complement is closed. Thus the induced topology on $X$ is exactly the original one.

Given an [open cover](../../../../open-cover.md) of $C$, choose a member containing infinity. It has the form $V\cup\{\infty\}$ with $K=X\setminus V$ [compact](../../../../compact-space.md). The remaining cover restricted to $K$ has a [finite subcover](../../../../finite-subcover.md). Together with the chosen infinity-neighborhood, these finitely many sets cover $C$. Hence **$C$ is [compact](../../../../compact-space.md)**, with no [Hausdorff](../../../../hausdorff-space.md) assumption needed.

Finally put $a=f(\infty)$. [Continuity](../../../../continuous-function.md) makes $U=f^{-1}((a-\epsilon,a+\epsilon))$ open and containing infinity. Therefore $U=V\cup\{\infty\}$ with $W=X\setminus V$ [compact](../../../../compact-space.md) and closed in $X$. For every $x\in X\setminus W=V$ we have

$$
\boxed{|f(x)-a|<\epsilon.}
$$

This expresses convergence to the value at infinity outside [compact](../../../../compact-space.md) closed subsets.

## ↑ Ancestors (12)

1. [3](../3.md)
2. [E](../../e.md)
3. [2006](../../../2006-split.md)
4. [Past exam of the options II course of the University of Oxford](../../../split.md)
5. [Options II course of the University of Oxford](../../../../options-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
