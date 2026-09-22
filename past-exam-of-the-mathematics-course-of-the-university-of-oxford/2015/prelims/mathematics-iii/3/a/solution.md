<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [gradient](../../../../../../gradient.md) of the given [polynomial](../../../../../../polynomial-split.md) is

$$
\nabla f=(2x+y^2+1,\ 2y(1+x)).
$$

Its second component vanishes when $y=0$ or $x=-1$. The first component then gives exactly three [critical points](../../../../../../critical-point.md):

$$
(-\tfrac12,0),\qquad (-1,1),\qquad (-1,-1).
$$

The [Hessian matrix](../../../../../../hessian-matrix.md) and its [determinant](../../../../../../determinant.md) are

$$
H_f=\begin{pmatrix}2&2y\\2y&2+2x\end{pmatrix},\qquad \det H_f=4(1+x-y^2).
$$

At $(-1/2,0)$ the [Hessian matrix](../../../../../../hessian-matrix.md) is $\operatorname{diag}(2,1)$, whose [positive definiteness](../../../../../../positive-definiteness.md) proves a strict [local minimum](../../../../../../local-minimum.md) by the [second-derivative test](../../../../../../second-derivative-test.md). At $(-1,\pm1)$ its [determinant](../../../../../../determinant.md) is $-4$, so both points are [saddle points of a scalar function](../../../../../../saddle-point-of-a-scalar-function.md). Their values and classifications are

$$
\boxed{\begin{aligned}
f(-\tfrac12,0)&=-\tfrac14&&\text{strict local minimum},\\
f(-1,\pm1)&=0&&\text{saddle points}.
\end{aligned}}
$$

There are **no [local maxima](../../../../../../local-maximum.md)**.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [3](../../3.md)
3. [Mathematics III](../../../mathematics-iii-split.md)
4. [Prelims](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
