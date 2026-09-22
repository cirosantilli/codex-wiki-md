<h1 id="5/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For the analogous positive off-diagonal entries in size $n$, take

$$
\boxed{d_1=1,\qquad d_i=\sqrt{\prod_{j=1}^{i-1}\frac{c_j}{b_j}}\quad(2\le i\le n),\qquad D=\operatorname{diag}(d_1,\ldots,d_n).}
$$

The same entrywise computation gives $(D^{-1}AD)_{ii}=a_i$ and $(D^{-1}AD)_{i,i+1}=(D^{-1}AD)_{i+1,i}=\sqrt{b_ic_i}$, with every other entry zero. Thus the result is a [symmetric matrix](../../../../../../symmetric-matrix.md) with a [tridiagonal](../../../../../../tridiagonal-matrix.md) pattern. Positivity of the diagonal entries $a_i$ is not needed for this [positive diagonal symmetrization of a tridiagonal matrix](../../../../../../positive-diagonal-symmetrization-of-a-tridiagonal-matrix.md); positivity of $b_i,c_i$ ensures the displayed positive, invertible $D$. In particular, the assertion is not an arbitrary-real-coefficient symmetrization claim when the off-diagonal signs differ.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [5](../../../5.md)
4. [Digital systems, linear algebra, introduction to formal proof](../../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
5. [2022](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
