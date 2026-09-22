<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For the [linear least-squares problem](../../../../linear-least-squares-problem.md) [objective function](../../../../objective-function.md), direct expansion with $d=y-x$ gives

$$
f(y)=\frac12\|Ax-b+Ad\|^2
=f(x)+(Ax-b)^TAd+\frac12\|Ad\|^2.
$$

Its [gradient](../../../../gradient.md) is $\nabla f(x)=A^T(Ax-b)$, so the middle term equals $\nabla f(x)^Td$.

Use the supplied thin [singular value decomposition](../../../../singular-value-decomposition.md) $A=USV^T$. Since $U^TU=I_n$, the [linear map](../../../../linear-map.md) $w\mapsto Uw$ preserves the [Euclidean norm](../../../../euclidean-norm.md). The square [matrix](../../../../matrix.md) $V$ is an [orthogonal matrix](../../../../orthogonal-matrix.md), so $\|V^Td\|=\|d\|$. Consequently

$$
\|Ad\|^2=\|SV^Td\|^2
=\sum_{i=1}^n s_{i,i}^2(V^Td)_i^2
\geq s_{\min}^2\sum_{i=1}^n(V^Td)_i^2
=s_{\min}^2\|d\|^2.
$$

Substitution into the expansion proves

$$
\boxed{f(y)\geq f(x)+\nabla f(x)^T(y-x)+\frac{s_{\min}^2}{2}\|y-x\|^2.}
$$

Thus $f$ is a [strongly convex function](../../../../strongly-convex-function.md) with modulus $\gamma=s_{\min}^2>0$. This modulus is sharp: choose $d=Ve_i$ for an index attaining the smallest [singular value](../../../../singular-value.md). The [Hessian matrix](../../../../hessian-matrix.md) is $A^TA=VS^2V^T$, so the same conclusion says that its smallest [eigenvalue](../../../../eigenvalue.md) is $s_{\min}^2$.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the optimisation for data science course of the University of Oxford](../../../split.md)
5. [Optimisation for data science course of the University of Oxford](../../../../optimisation-for-data-science-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
