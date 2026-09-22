<h1 id="n2/e/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For $|s|\leq1$, all the generating-function expectations are absolutely bounded. Conditional on $X=k$, independence gives

$$
\mathbb E[s^T\mid X=k]=s\prod_{i=1}^k\mathbb E[s^{T_i}]=sG_T(s)^k.
$$

At $k=0$ the product is one, consistent with the empty-family case. The [law of total expectation](../../../../../law-of-total-expectation.md) now yields

$$
\boxed{G_T(s)=s\sum_{k=0}^{\infty}p_kG_T(s)^k
=sG_X(G_T(s))=s\exp\{\lambda(G_T(s)-1)\}.}
$$

This is the [total progeny generating function of a branching process](../../../../../total-progeny-generating-function-of-a-branching-process.md). The given almost-sure finiteness of $T$ ensures $G_T(1)=1$. The conditional-expectation proof avoids assuming a finite expected total before it has been established.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [E](../../e.md)
3. [N2](../../../n2.md)
4. [2013](../../../../2013-split.md)
5. [Past exam of the options II for mathematics and philosophy course of the University of Oxford](../../../../split.md)
6. [Options II for mathematics and philosophy course of the University of Oxford](../../../../../options-ii-for-mathematics-and-philosophy-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics and philosophy course of the University of Oxford](../../../../../year-2-of-the-mathematics-and-philosophy-course-of-the-university-of-oxford.md)
8. [Mathematics and philosophy course of the University of Oxford](../../../../../mathematics-and-philosophy-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
