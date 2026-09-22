# Weighted inner product

↑ **Parent:** [Inner product](inner-product-split.md)

For a positive weight $w$, the weighted inner product of [functions](function-split.md) is $\langle f,g\rangle_w=\int\overline f g w$. It is the usual [inner product](inner-product-split.md) in the [L2 space](l2-space-is-a-hilbert-space.md) for the measure $w(x)dx$. A [Sturm-Liouville eigenfunction expansion](sturm-liouville-eigenfunction-expansion.md) uses this weight to make its [eigenfunctions](eigenfunction.md) [orthogonal](orthogonal-vectors.md).

The weight specifies how different locations contribute to a squared error: $\|f-g\|_w^2=\int|f-g|^2w$. More weight makes an error in that region more costly. The [weighted Euclidean inner product](weighted-euclidean-inner-product.md) makes the same choice for a finite list of coordinates.

For an explicit real-function example on $[0,1]$, let $w(x)=1+x$ and approximate $f(x)=x$ by a [constant function](constant-function.md). The [orthogonal projection onto a finite-dimensional subspace](orthogonal-projection-onto-a-finite-dimensional-subspace.md) spanned by the function $1$ gives

$$
c=\frac{\langle x,1\rangle_w}{\langle1,1\rangle_w}
=\frac{\int_0^1x(1+x)\,dx}{\int_0^1(1+x)\,dx}
=\frac{5/6}{3/2}=\frac59.
$$

The best unweighted constant is $1/2$. Giving greater weight to larger $x$ moves the best constant upward, so a weighting choice changes the approximation even though the allowed family of [functions](function-split.md) is unchanged.

**Table of contents**

- [Weighted norm](weighted-norm.md)
- [Weighted Euclidean inner product](weighted-euclidean-inner-product.md)

## ↑ Ancestors (6)

1. [Inner product](inner-product-split.md)
2. [Linear algebra](linear-algebra-split.md)
3. [Algebra](algebra-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (57)

- [Adjoint in weighted coordinates](adjoint-in-weighted-coordinates.md)
- [Cubic-coordinate reduction of a singular Sturm-Liouville operator](cubic-coordinate-reduction-of-a-singular-sturm-liouville-operator.md)
- [Decoupled coefficients of orthogonal polynomial projections](decoupled-coefficients-of-orthogonal-polynomial-projections.md)
- [Dirichlet eigenfunctions of the Chebyshev differential operator](dirichlet-eigenfunctions-of-the-chebyshev-differential-operator.md)
- [Dirichlet spectrum with inverse-square weight](dirichlet-spectrum-with-inverse-square-weight.md)
- [Legendre least-squares projections of a cubic](legendre-least-squares-projections-of-a-cubic.md)
- [Logarithmic change of variable in a Sturm-Liouville problem](logarithmic-change-of-variable-in-a-sturm-liouville-problem.md)
- [Neumann eigenfunctions of the Chebyshev differential operator](neumann-eigenfunctions-of-the-chebyshev-differential-operator.md)
- [Normalization of the ordinary Laguerre polynomials](normalization-of-the-ordinary-laguerre-polynomials.md)
- [Normalized Sturm-Liouville spectral Green kernel](normalized-sturm-liouville-spectral-green-kernel.md)
- [Orthogonal polynomial](orthogonal-polynomial-split.md)
- [Orthogonal vectors](orthogonal-vectors.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-328/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-328/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2011/paper-2/20/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2002/paper-1/9/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2004/paper-1/7/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2004/paper-1/7/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2005/paper-1/7/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2007/paper-1/7/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2008/paper-2/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2010/paper-1/10/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2010/paper-2/1/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2010/paper-2/1/iv/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2010/paper-2/7/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2011/paper-2/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2012/paper-1/10/i/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2012/paper-2/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2013/paper-1/10/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2013/paper-1/10/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2013/paper-2/1/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2014/paper-2/1/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2014/paper-2/1/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2015/paper-2/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2015/paper-2/1/b/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2015/paper-2/1/b/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2016/paper-2/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2017/paper-2/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2017/paper-2/1/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2017/paper-2/7/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2018/paper-1/10/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2018/paper-2/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2019/paper-2/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2021/paper-2/1/a/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2022/paper-1/10/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2023/paper-1/10/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2023/paper-2/1/b/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2024/paper-1/10/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2024/paper-2/1/d/solution.md)
- [Radial vibrations of a circular membrane](radial-vibrations-of-a-circular-membrane.md)
- [Regular solution of a forced Chebyshev equation](regular-solution-of-a-forced-chebyshev-equation.md)
- [String with an endpoint mass](string-with-an-endpoint-mass.md)
- [Symmetric positive-definite preconditioning](symmetric-positive-definite-preconditioning.md)
- [Vector normalization](vector-normalization.md)
- [Weighted Euclidean inner product](weighted-euclidean-inner-product.md)
- [Weighted Neumann heat kernel with constant drift](weighted-neumann-heat-kernel-with-constant-drift.md)
- [Weighted norm](weighted-norm.md)
