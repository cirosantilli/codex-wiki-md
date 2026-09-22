<h1 id="6/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The [heat equation](../../../../../../heat-equation.md) and its homogeneous [Dirichlet boundary conditions](../../../../../../dirichlet-boundary-condition.md) are [linear](../../../../../../linearity.md), so [superposition](../../../../../../superposition-principle.md) of the separated modes gives

$$
\boxed{u(x,t)=\sum_{n=1}^{\infty}\alpha_n\sin\frac{n\pi x}{L}
\exp\left(-\frac{Dn^2\pi^2t}{L^2}\right).}
$$

The [Fourier sine basis](../../../../../../fourier-sine-basis.md) represents the initial profile on the interior of the interval. At $t=0$ its [Fourier sine series](../../../../../../fourier-sine-series.md) must equal $x(1-x)$. Multiplying by $\sin(m\pi x/L)$, integrating from $0$ to $L$, and using [orthogonality](../../../../../../orthogonal-vectors.md) gives

$$
\int_0^L\sin\frac{n\pi x}{L}\sin\frac{m\pi x}{L}\,dx
=\begin{cases}L/2,&n=m,\\0,&n\ne m.\end{cases}
$$

Therefore the required [Fourier sine coefficients](../../../../../../fourier-sine-coefficient.md) are

$$
\boxed{\alpha_n=\frac2L\int_0^L x(1-x)\sin\frac{n\pi x}{L}\,dx,
\qquad n=1,2,\ldots.}
$$

For every $t>0$, the exponential factors ensure convergence of the differentiated series, and every term satisfies the [partial differential equation](../../../../../../partial-differential-equation-split.md) and the [boundary conditions](../../../../../../boundary-condition.md). The [Fourier sine series](../../../../../../fourier-sine-series.md) recovers the smooth initial profile at every $0<x<L$ as $t\downarrow0$.

The scan explicitly prints $x(1-x)$ on $(0,L)$; it must not silently become $x(L-x)$. For $L\ne1$, the interior profile tends to $L(1-L)\ne0$ at the right endpoint, whereas the prescribed [boundary condition](../../../../../../boundary-condition.md) is zero for $t>0$. The solution is therefore not continuous at the corner $(L,0)$, although it satisfies every condition on the printed open ranges. A solution continuous on the closed space-time domain with these data would require $L=1$.[Printed page 7, Question 6(b), initial profile and ranges](../../../../../../discrete-mathematics-continuous-mathematics-and-probability-examination-2015-by-university-of-oxford.md)

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [6](../../../6.md)
4. [Discrete mathematics, continuous mathematics, and probability](../../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
5. [2015](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
