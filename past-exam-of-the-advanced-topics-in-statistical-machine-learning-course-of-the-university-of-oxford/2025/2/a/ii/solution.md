<h1 id="2/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For every $m\geq1$, every choice $x_1,\ldots,x_m\in\mathcal X$, and every coefficient [vector](../../../../../vector.md) $\alpha\in\mathbb R^m$, the required condition is

$$
\boxed{\sum_{i,j=1}^m\alpha_i\alpha_j k(x_i,x_j)\geq0}.
$$

Thus $\alpha^TK\alpha\geq0$ for the [kernel matrix](../../../../../kernel-matrix.md) $K$. For a [feature map](../../../../../feature-map.md), this follows from

$$
\sum_{i,j}\alpha_i\alpha_j\langle\varphi(x_i),\varphi(x_j)\rangle=\left\|\sum_i\alpha_i\varphi(x_i)\right\|_{\mathcal H}^2\geq0.
$$

In [kernel methods](../../../../../kernel-method.md), the term [positive-definite kernel](../../../../../positive-semidefinite-kernel-split.md) commonly uses this non-strict inequality. Strict positive definiteness is the stronger requirement that the expression be positive for distinct inputs and every nonzero $\alpha$; it is not required here.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [2](../../../2.md)
4. [2025](../../../../2025-split.md)
5. [Past exam of the advanced topics in statistical machine learning course of the University of Oxford](../../../../split.md)
6. [Advanced topics in statistical machine learning course of the University of Oxford](../../../../../advanced-topics-in-statistical-machine-learning-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics and statistics course of the University of Oxford](../../../../../year-4-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Mathematics and statistics course of the University of Oxford](../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
