<h1 id="5/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Interpret the norms as [Euclidean norms](../../../../../../euclidean-norm.md) and set $B=A^{\mathsf T}A$. This is a [real symmetric matrix](../../../../../../real-symmetric-matrix.md) with $\mathbf x^{\mathsf T}B\mathbf x=\|A\mathbf x\|^2\ge0$, hence a [positive semidefinite matrix](../../../../../../positive-semidefinite-matrix.md). Squaring the nonnegative objective does not change its [argmin](../../../../../../argmin.md). Let $\lambda_{\min}$ be the smallest [eigenvalue](../../../../../../eigenvalue.md) of $B$ and $E_{\min}$ its [eigenspace](../../../../../../eigenspace.md).

First minimize on the [unit sphere](../../../../../../unit-sphere.md). The [Lagrange multiplier](../../../../../../lagrange-multiplier.md) function $L(\mathbf x,\lambda)=\mathbf x^{\mathsf T}B\mathbf x-\lambda(\mathbf x^{\mathsf T}\mathbf x-1)$ has stationarity condition $B\mathbf x=\lambda\mathbf x$. Multiplication by $\mathbf x^{\mathsf T}$ shows that the squared objective at such a point is $\lambda$. The [spectral theorem for real symmetric matrices](../../../../../../spectral-theorem-for-real-symmetric-matrices.md) also gives, for every unit [vector](../../../../../../vector.md), $\mathbf x^{\mathsf T}B\mathbf x\ge\lambda_{\min}$, with equality exactly in $E_{\min}$. This proves global minimality, rather than merely finding stationary candidates.

If $\lambda_{\min}>0$, every point with $\|\mathbf x\|>1$ has a strictly smaller objective after rescaling to unit length. Therefore

$$
\boxed{\operatorname*{arg\,min}_{\|\mathbf x\|\ge1}\|A\mathbf x\|=\{\mathbf x\in E_{\min}:\|\mathbf x\|=1\},\quad\min=\sqrt{\lambda_{\min}}.}
$$

If $\lambda_{\min}=0$, the [kernel of a linear map](../../../../../../kernel-of-a-linear-map-split.md) satisfies $\ker B=\ker A$, since $B\mathbf x=0$ implies $\|A\mathbf x\|^2=0$, and the converse is immediate. The [minimum](../../../../../../minimum-of-a-subset-of-a-total-order.md) is then zero, attained precisely at

$$
\boxed{\{\mathbf x\in\ker A:\|\mathbf x\|\ge1\}.}
$$

In this case minimizers need not have unit length. This distinction is essential for a rank-deficient $A$, including any real $m\times n$ [matrix](../../../../../../matrix.md) with $m<n$. The result is the [minimum image norm outside a Euclidean unit ball](../../../../../../minimum-image-norm-outside-a-euclidean-unit-ball.md), governed by the least [singular value](../../../../../../singular-value.md).

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [5](../../../5.md)
4. [Discrete mathematics, probability and continuous mathematics](../../../../discrete-mathematics-probability-and-continuous-mathematics-split.md)
5. [2023](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
