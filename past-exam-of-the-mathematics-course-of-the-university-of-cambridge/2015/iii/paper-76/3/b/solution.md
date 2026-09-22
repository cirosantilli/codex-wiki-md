<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Choose a fixed positive [Landweber relaxation parameter](../../../../../../landweber-relaxation-parameter.md) $\tau$ and rearrange the [normal equation for a linear inverse problem](../../../../../../normal-equation-for-a-linear-inverse-problem.md) as the [fixed point](../../../../../../fixed-point.md) equation

$$
 x=(I-\tau A^*A)x+\tau A^*y.
$$

Successive substitution gives [Landweber iteration](../../../../../../landweber-iteration.md)

$$
\boxed{x_{n+1}=x_n+\tau A^*(y-Ax_n),\qquad x_0=0.}
$$

Set $B=A^*A$ and $P=I-\tau B$. Induction yields the closed polynomial-operator expression

$$
\boxed{x_n=\tau\sum_{j=0}^{n-1}P^jA^*y
 =h_n(B)A^*y,\qquad
 h_n(t)=\begin{cases}\dfrac{1-(1-\tau t)^n}{t},&t\ne0,\\n\tau,&t=0.\end{cases}}
$$

For $n=0$ the sum is empty, giving zero. The expression is well defined without an inverse of $A^*A$, which can have a [kernel of a linear map](../../../../../../kernel-of-a-linear-map.md) and an unbounded inverse on its range. Each iterate lies in the closure of $\operatorname{Ran}A^*$, so initialization at zero eliminates the arbitrary null-space component of a solution. The unrelaxed choice $\tau=1$ gives $x_{n+1}=(I-A^*A)x_n+A^*y$ and the corresponding sum with $\tau=1$; it needs the convergence restriction in part (d).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 76](../../../paper-76-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
