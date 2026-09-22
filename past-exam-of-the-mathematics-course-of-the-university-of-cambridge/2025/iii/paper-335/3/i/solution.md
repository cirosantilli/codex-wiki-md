<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

A [regularization of an inverse problem](../../../../../../regularization-of-an-inverse-problem.md) consists of bounded operators $R_\alpha:Y\to X$ and a parameter rule $\alpha=\alpha(\delta,y^\delta)$ such that, whenever $\|y^\delta-y\|\leq\delta$ and $y$ lies in the domain of $A^\dagger$,

$$
\alpha(\delta,y^\delta)\to0,
\qquad
R_{\alpha(\delta,y^\delta)}y^\delta\to A^\dagger y
$$

as $\delta\to0$. It is needed because a compact operator on an infinite-dimensional space has singular values tending to zero, so direct inversion divides noisy data by arbitrarily small numbers and is generally discontinuous.

[Tikhonov regularization](../../../../../../tikhonov-regularization.md) defines

$$
x_\alpha^\delta
=\underset{x\in X}{\operatorname{argmin}}
\left(\|Ax-y^\delta\|^2+\alpha\|x\|^2\right),
$$

and its normal equation gives

$$
\boxed{x_\alpha^\delta
=(A^*A+\alpha I)^{-1}A^*y^\delta.}
$$

For every fixed $\alpha>0$, $A^*A+\alpha I$ is bounded below by $\alpha I$, and the data-to-solution operator is bounded. Small changes in $y^\delta$ therefore produce small changes in $x_\alpha^\delta$.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 335](../../../paper-335-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
