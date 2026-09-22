<h1 id="6/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Put $h=x-1$ and $k=y-1$. At $(1,1)$, the value is $5+4\alpha$, the [gradient](../../../../../../gradient.md) is $(5+4\alpha,4+2\alpha)$, and the [Hessian matrix](../../../../../../hessian-matrix.md) is $\begin{pmatrix}8&2\alpha\\2\alpha&2\end{pmatrix}$. Thus the quadratic [Taylor expansion](../../../../../../taylor-expansion.md) is

$$
\boxed{f(1+h,1+k)
=5+4\alpha+(5+4\alpha)h+(4+2\alpha)k
+4h^2+2\alpha hk+k^2+O((|h|+|k|)^3).}
$$

The exact remainder is $h^3$, since the original [polynomial](../../../../../../polynomial-split.md) has only the cubic term $x^3$ beyond degree two.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [6](../../../6.md)
4. [Discrete mathematics, continuous mathematics and probability](../../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
5. [2014](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
