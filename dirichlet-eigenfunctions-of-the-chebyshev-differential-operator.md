# Dirichlet eigenfunctions of the Chebyshev differential operator

↑ **Parent:** [Chebyshev differential equation](chebyshev-differential-equation.md)

The [Chebyshev differential equation](chebyshev-differential-equation.md) $-(1-x^2)y''+xy'=\lambda y$ on $-1<x<1$, with zero endpoint values, has the [Sturm-Liouville form](sturm-liouville-form.md)

$$
-\frac d{dx}\left[\sqrt{1-x^2}\,y'\right]=\lambda\frac{y}{\sqrt{1-x^2}}.
$$

Thus $p=\sqrt{1-x^2}$ and the weight defining the [weighted inner product](weighted-inner-product.md) is $w=(1-x^2)^{-1/2}$. The substitution $x=\cos\theta$ maps the problem to $-Y''=\lambda Y$ on $0<\theta<\pi$ with homogeneous [Dirichlet boundary conditions](dirichlet-boundary-condition.md). It also transforms $w(x)\,dx$ into $-d\theta$. Consequently the normalized [eigenfunctions](eigenfunction.md) are

$$
\boxed{y_n(x)=\sqrt{\frac2\pi}\sin(n\arccos x),\qquad\lambda_n=n^2,\quad n=1,2,\ldots.}
$$

Their [weighted inner product](weighted-inner-product.md) is the ordinary sine [inner product](inner-product-split.md) on $[0,\pi]$. Equivalently, $y_n=\sqrt{2/\pi}\sqrt{1-x^2}\,U_{n-1}(x)$, where $U_{n-1}$ is a [Chebyshev polynomial of the second kind](chebyshev-polynomial-of-the-second-kind.md). These are not the cosine solutions $T_n$, which have different endpoint values. The original endpoints are singular because $p$ vanishes and $w$ diverges there, but the transformed Dirichlet problem specifies the self-adjoint realization. The eigenfunctions vanish at both endpoints and their quasi-derivatives $py_n'$ have finite limits, so the boundary form vanishes.

## ↑ Ancestors (7)

1. [Chebyshev differential equation](chebyshev-differential-equation.md)
2. [Chebyshev polynomial](chebyshev-polynomial.md)
3. [Numerical analysis](numerical-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Neumann eigenfunctions of the Chebyshev differential operator](neumann-eigenfunctions-of-the-chebyshev-differential-operator.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2001/paper-1/7/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2015/paper-2/1/b/i/solution.md)
