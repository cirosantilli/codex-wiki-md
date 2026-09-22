<h1 id="8d/solution">Solution</h1>

↑ **Parent:** [8D](../8d.md)

With $x=\cos\theta$, the weighted [inner product](../../../../../inner-product.md) for the [Chebyshev polynomials](../../../../../chebyshev-polynomial.md) becomes

$$
\int_{-1}^1\frac{T_n(x)T_m(x)}{\sqrt{1-x^2}}\,dx=\int_0^\pi\cos(n\theta)\cos(m\theta)\,d\theta.
$$

The identity $2\cos(n\theta)\cos(m\theta)=\cos((n-m)\theta)+\cos((n+m)\theta)$ and the vanishing of $\int_0^\pi\cos(k\theta)\,d\theta$ for positive integers $k$ give zero when $n\neq m$, $\pi/2$ when $n=m>0$, and $\pi$ when $n=m=0$. Thus

$$
\boxed{\int_{-1}^1\frac{T_nT_m}{\sqrt{1-x^2}}\,dx=\frac\pi2\delta_{nm}(1+\delta_{n0}).}
$$

For [Gaussian quadrature](../../../../../gaussian-quadrature.md), choose the $n$ distinct nodes as the zeros of the degree-$n$ [orthogonal polynomial](../../../../../orthogonal-polynomial.md) for the weight, here $T_n$, and choose the weights as the weighted integrals of their [Lagrange interpolation](../../../../../lagrange-polynomial.md) basis functions. If a [polynomial](../../../../../polynomial-split.md) $p$ has degree at most $2n-1$, divide it as $p=qT_n+r$, where both $q$ and $r$ have degree at most $n-1$. Orthogonality makes the integral of $qT_n$ zero, while its quadrature sum also vanishes; interpolation integrates $r$ exactly. This proves degree $2n-1$ exactness. It is optimal because the squared nodal [polynomial](../../../../../polynomial-split.md), of degree $2n$, has zero quadrature sum and strictly positive integral.

For $n=3$, $T_3(x)=4x^3-3x$, so the nodes are $-\sqrt3/2,0,\sqrt3/2$. Their interpolation basis functions are

$$
\ell_-(x)=\frac23x\left(x-\frac{\sqrt3}{2}\right),\quad \ell_0(x)=1-\frac43x^2,\quad \ell_+(x)=\frac23x\left(x+\frac{\sqrt3}{2}\right).
$$

The weighted zeroth and second moments are $\pi$ and $\pi/2$, and the first moment is zero. Integrating these three basis functions gives equal weights $\pi/3$, hence the [Chebyshev–Gauss quadrature](../../../../../chebyshev-gauss-quadrature.md) rule

$$
\boxed{\int_{-1}^1\frac{f(x)}{\sqrt{1-x^2}}\,dx\approx\frac\pi3\left[f\!\left(-\frac{\sqrt3}{2}\right)+f(0)+f\!\left(\frac{\sqrt3}{2}\right)\right],}
$$

which is exact for every [polynomial](../../../../../polynomial-split.md) of degree at most $5$.

## ↑ Ancestors (10)

1. [8D](../8d.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
