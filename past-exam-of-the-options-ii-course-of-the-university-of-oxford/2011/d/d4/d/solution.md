<h1 id="d/d4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Expand $x^x=e^{x\log x}$. The absolute values of all terms have total [integral](../../../../../integral-split.md)

$$
\sum_{k=0}^\infty\frac1{k!}\int_0^1|x\log x|^k\,dx
=\sum_{j=1}^\infty j^{-j}<\infty.
$$

The [series](../../../../../series-mathematics.md) converges, for instance because $j^{-j}\leq2^{-j}$ for $j\geq2$. Part (b) applied to the absolute values, followed by subtraction of positive and negative parts, therefore justifies termwise integration. It gives the other [Sophomore's dream](../../../../../sophomore-s-dream.md) identity:

$$
\boxed{\int_0^1x^x\,dx=\sum_{j=1}^\infty\frac{(-1)^{j-1}}{j^j}.}
$$

Equivalently, the partial sums are dominated by $e^{|x\log x|}\leq e^{1/e}$, so the [dominated convergence theorem](../../../../../dominated-convergence-theorem.md) gives the same justification.

## ↑ Ancestors (13)

1. [D](../d.md)
2. [D4](../../d4.md)
3. [D](../../../d.md)
4. [2011](../../../../2011-split.md)
5. [Past exam of the options II course of the University of Oxford](../../../../split.md)
6. [Options II course of the University of Oxford](../../../../../options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
