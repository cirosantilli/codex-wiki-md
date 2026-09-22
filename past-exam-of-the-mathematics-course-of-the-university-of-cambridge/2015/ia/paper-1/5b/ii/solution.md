<h1 id="5b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Subtract the two constraints to obtain $x\cdot(a-b)=A-B$. The [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) gives $|A-B|\leq\|x\|\,\|a-b\|$. Since $a\ne b$, division and squaring give the [distance bound from two hyperplane constraints](../../../../../../distance-bound-from-two-hyperplane-constraints.md)

$$
\boxed{\|x\|^2\geq\frac{(A-B)^2}{\|a-b\|^2}.}
$$

If $a=b$ and $A\ne B$, **the intersection is empty**. If $a=b\ne0$ and $A=B$, the constraints describe the same hyperplane. Its points satisfy $\|x\|^2\geq A^2/\|a\|^2$, with equality at $x=Aa/\|a\|^2$. The fraction involving $a-b$ is undefined in this case and cannot be used.

If $a=b=0$, both equations are satisfied by every $x$ when $A=B=0$, and otherwise there is no solution. These degenerate cases distinguish an inconsistent constraint from a repeated one.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [5B](../../5b.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
