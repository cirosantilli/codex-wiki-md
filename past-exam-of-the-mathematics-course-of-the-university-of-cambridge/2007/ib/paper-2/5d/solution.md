<h1 id="5d/solution">Solution</h1>

↑ **Parent:** [5D](../5d.md)

Use the [mixed Dirichlet-Neumann modes on an interval](../../../../../mixed-dirichlet-neumann-modes-on-an-interval.md). To justify their [Fourier series](../../../../../fourier-series-split.md), extend $y$ evenly across $x=1$ to $[0,2]$, then oddly across $x=0$, and repeat with period four. The condition $y(0)=0$ makes the odd extension [continuous](../../../../../continuous-function.md), and $y'(1)=0$ makes the even reflection continuously differentiable. The resulting periodic function has a convergent [Fourier sine series](../../../../../fourier-sine-series.md). Reflection about $x=1$ eliminates the even [sine](../../../../../sine.md) harmonics, leaving

$$
\boxed{\lambda_n=(n+1/2)\pi,\qquad n=0,1,2,\ldots.}
$$

Alternatively these values follow directly from $\sin\lambda_n0=0$ and $\lambda_n\cos\lambda_n=0$. [Fourier orthogonality](../../../../../fourier-orthogonality.md) gives

$$
\int_0^1\sin\lambda_nx\sin\lambda_mx\,dx=\frac12\delta_{nm},\qquad
\boxed{a_n=2\int_0^1y(x)\sin\lambda_nx\,dx.}
$$

The extension argument also supplies completeness, not merely orthogonality, of this [Fourier sine basis](../../../../../fourier-sine-basis.md).

Expand the forcing as $x\cos\pi x=\sum b_n\sin\lambda_nx$. Product-to-sum and [integration by parts](../../../../../integration-by-parts.md) give

$$
\begin{aligned}
b_n&=2\int_0^1x\cos\pi x\sin\lambda_nx\,dx\\
&=\int_0^1x[\sin((\lambda_n+\pi)x)+\sin((\lambda_n-\pi)x)]\,dx\\
&=-(-1)^n\left[\frac1{(\lambda_n+\pi)^2}+\frac1{(\lambda_n-\pi)^2}\right].
\end{aligned}
$$

Each mode of the differential operator has [eigenvalue](../../../../../eigenvalue.md) $-(\lambda_n^2+\alpha^2)$. Hence, for real $\alpha$, the solution is

$$
\boxed{y(x)=\sum_{n=0}^\infty
\frac{(-1)^n}{\lambda_n^2+\alpha^2}
\left[\frac1{(\lambda_n+\pi)^2}+\frac1{(\lambda_n-\pi)^2}\right]
\sin\lambda_nx.}
$$

The coefficients are $O(n^{-4})$, so the series and its first two differentiated series converge uniformly. Therefore it solves the equation and the [boundary conditions](../../../../../boundary-condition.md) term by term. Uniqueness follows by multiplying the homogeneous equation by its real solution and integrating: the boundary terms vanish and $\int_0^1[(y')^2+\alpha^2y^2],dx=0$, forcing $y=0$.

## ↑ Ancestors (10)

1. [5D](../5d.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
