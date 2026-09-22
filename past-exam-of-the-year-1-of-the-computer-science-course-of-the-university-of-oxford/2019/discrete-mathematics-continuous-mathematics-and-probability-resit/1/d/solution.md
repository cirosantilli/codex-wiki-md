<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Put $B=T\cap S$. By [distributivity](../../../../../distributive-property.md), $g(A)=B\cup(T\cap A)$ and $B\subseteq T$. Consequently,

$$
\begin{aligned}
g(g(A))&=B\cup\bigl(T\cap(B\cup(T\cap A))\bigr)\\
&=B\cup(T\cap B)\cup(T\cap A)\\
&=B\cup(T\cap A)=g(A).
\end{aligned}
$$

Here we used [associativity](../../../../../associative-property.md), [distributivity](../../../../../distributive-property.md), and [idempotence](../../../../../idempotence.md) of [set intersection](../../../../../set-intersection.md) and [set union](../../../../../set-union.md). The equality holds for every $A\in\mathcal P(U)$, so **$g\circ g=g$**: $g$ is an [idempotent function](../../../../../idempotent-function.md).

## ↑ Ancestors (12)

1. [D](../d.md)
2. [1](../../1.md)
3. [Discrete mathematics, continuous mathematics, and probability resit](../../../discrete-mathematics-continuous-mathematics-and-probability-resit-split.md)
4. [2019](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
