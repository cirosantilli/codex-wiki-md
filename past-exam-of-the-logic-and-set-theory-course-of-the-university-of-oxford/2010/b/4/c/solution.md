<h1 id="b/4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

**True in ZF.** Let $i:A\hookrightarrow A'$ and $j:B\hookrightarrow B'$ witness the two cardinal inequalities. Because $A$ is nonempty, fix one element $a_0\in A$. Send $f:B\to A$ to $\widehat f:B'\to A'$ defined by

$$
\boxed{\widehat f(b')=\begin{cases}
i(f(b)),&b'=j(b)\text{ for }b\in B,\\
i(a_0),&b'\notin j[B].
\end{cases}}
$$

The first case is well defined by injectivity of $j$. If $f\ne g$, choose a point where their values differ; the images differ at its $j$-image because $i$ is [injective](../../../../../injective-function.md). Thus $f\mapsto\widehat f$ is [injective](../../../../../injective-function.md), proving the desired inequality of function-space cardinalities.

Fixing one element of a single known nonempty set does not invoke the [axiom of choice](../../../../../axiom-of-choice.md). The nonzero-base hypothesis is what permits this constant extension outside the smaller domain.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [4](../../4.md)
3. [B](../../../b.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the logic and set theory course of the University of Oxford](../../../../split.md)
6. [Logic and set theory course of the University of Oxford](../../../../../logic-and-set-theory-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
