<h1 id="6/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Substitution gives $R^TRx=R^TQ^Tb$. Since $R^T$ is invertible, cancel it on the left to obtain the nonsingular triangular system

$$
\boxed{Rx=Q^Tb.}
$$

This is the [reduced QR least-squares solution](../../../../../../reduced-qr-least-squares-solution.md). Its geometric justification is the orthogonal decomposition

$$
\|Ax-b\|_2^2=\|Rx-Q^Tb\|_2^2+\|(I-QQ^T)b\|_2^2.
$$

The second term is independent of $x$, while invertibility of $R$ lets the first term be zero at exactly one point. Although $Q^TQ=I_M$, one must not replace $QQ^T$ by $I_N$: $Q$ is tall and its product $QQ^T$ is the [orthogonal projection](../../../../../../orthogonal-projection.md) onto its column space.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [6](../../../6.md)
4. [Digital systems, linear algebra, introduction to formal proof resit](../../../../digital-systems-linear-algebra-introduction-to-formal-proof-resit-split.md)
5. [2019](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
