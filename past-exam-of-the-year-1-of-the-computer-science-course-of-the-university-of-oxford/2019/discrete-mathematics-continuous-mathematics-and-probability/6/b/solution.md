<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

If $\mathbf b=0$, the objective is zero at every feasible point, so **every point of the ellipsoid is a minimizer**. Suppose now $\mathbf b\ne0$. A minimum cannot be interior: a sufficiently small step in direction $-\mathbf b$ would remain feasible and decrease the objective. The boundary is active.

For

$$
\mathcal L(\mathbf x,\lambda)=\mathbf b^{\mathsf T}\mathbf x+
\lambda(\mathbf x^{\mathsf T}A\mathbf x-1),
$$

stationarity gives $\mathbf b+2\lambda A\mathbf x=0$. A [positive-definite symmetric matrix](../../../../../symmetric-positive-definite-matrix.md) is invertible, and the minimizing sign has $\lambda>0$. Enforcing the boundary gives

$$
\lambda=\frac12\sqrt{\mathbf b^{\mathsf T}A^{-1}\mathbf b},\qquad
\boxed{\mathbf x_*=
-\frac{A^{-1}\mathbf b}{\sqrt{\mathbf b^{\mathsf T}A^{-1}\mathbf b}}.}
$$

For global optimality, use the [inner product](../../../../../inner-product-split.md) $\langle u,v\rangle_A=u^{\mathsf T}Av$. The [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) gives

$$
|\mathbf b^{\mathsf T}\mathbf x|
=|\langle A^{-1}\mathbf b,\mathbf x\rangle_A|
\le\sqrt{\mathbf b^{\mathsf T}A^{-1}\mathbf b}
\sqrt{\mathbf x^{\mathsf T}A\mathbf x}
\le\sqrt{\mathbf b^{\mathsf T}A^{-1}\mathbf b}.
$$

The proposed point attains the negative of this bound. Thus **the minimum is $-\sqrt{\mathbf b^{\mathsf T}A^{-1}\mathbf b}$**, and equality in the [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md), together with the sign and boundary conditions, makes this minimizer unique when $\mathbf b\ne0$.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [6](../../6.md)
3. [Discrete mathematics, continuous mathematics, and probability](../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
4. [2019](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
