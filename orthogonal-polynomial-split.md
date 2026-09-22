# Orthogonal polynomial

↑ **Parent:** [Numerical analysis](numerical-analysis-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Orthogonal_polynomial)

An [orthogonal polynomial](orthogonal-polynomial-split.md) family chooses [polynomials](polynomial-split.md) that do not overlap under a specified [inner product](inner-product-split.md). For real [polynomials](polynomial-split.md) on an interval $(a,b)$, use the [weighted inner product](weighted-inner-product.md)

$$
\langle p,q\rangle_w=\int_a^b p(x)q(x)w(x)\,dx,\qquad \|p\|_w^2=\langle p,p\rangle_w.
$$

Assume $a<b$, the weight $w$ is measurable and positive [almost everywhere](almost-everywhere.md), and its absolute moments $\int_a^b |x|^k w(x)\,dx$ are finite for every [integer](integer-split.md) $k\geq0$. These conditions make the [integrals](integral-split.md) finite and give every nonzero [polynomial](polynomial-split.md) positive squared [norm](norm.md). A sequence $p_0,p_1,\ldots$ is an [orthogonal polynomial](orthogonal-polynomial-split.md) family when $p_n$ has real [coefficients](coefficient.md) and [polynomial degree](degree-of-a-polynomial.md) exactly $n$, and $\langle p_n,p_k\rangle_w=0$ for $n\ne k$.[NIST Digital Library of Mathematical Functions; Koornwinder, Wong, Koekoek, Swarttouw and Reinhardt, NIST DLMF Chapter 18, §18.2(i), equations 18.2.1 and 18.2.1\_5: interval orthogonality and finite absolute moments](nist-digital-library-of-mathematical-functions/18-orthogonal-polynomials.md)

Here $h_n=\|p_n\|_w^2>0$ and $\delta_{nk}$ is the [Kronecker delta](kronecker-delta.md). [Orthogonality](orthogonal-vectors.md) does not require $h_n=1$: an [orthonormal set](orthonormal-set.md) is obtained only after replacing $p_n$ by $p_n/\sqrt{h_n}$. Multiplying each member by any nonzero real constant preserves [orthogonality](orthogonal-vectors.md), but changes its [norm](norm.md) and the corresponding expansion [coefficient](coefficient.md). The [monic orthogonal polynomial](monic-orthogonal-polynomial.md) convention instead fixes each leading [coefficient](coefficient.md) to one.

The first four [Legendre polynomials](legendre-polynomial.md), named for [Adrien-Marie Legendre](adrien-marie-legendre.md), use $w=1$ on $[-1,1]$ and the normalization $P_n(1)=1$:

$$
P_0(x)=1,\qquad P_1(x)=x,\qquad P_2(x)=\frac{3x^2-1}{2},\qquad P_3(x)=\frac{5x^3-3x}{2}.
$$

Their [orthogonality](orthogonal-vectors.md) and squared [norms](norm.md) are

$$
\int_{-1}^1 P_n(x)P_k(x)\,dx=\frac{2}{2n+1}\delta_{nk}.
$$

Thus their [Gram matrix](gram-matrix.md) has a positive diagonal and zero entries elsewhere, although their [function graphs](graph-of-a-function.md) cross and overlap on the page. [Orthogonality](orthogonal-vectors.md) measures an [integral](integral-split.md) of products, rather than separation of [function graphs](graph-of-a-function.md).[NIST Digital Library of Mathematical Functions; Koornwinder and collaborators, NIST DLMF Chapter 18, Table 18.3.1, Legendre row: interval, unit weight, squared norm and normalization](nist-digital-library-of-mathematical-functions/18-orthogonal-polynomials.md)

<a id="image-the-first-four-legendre-polynomials-and-their-exact-integral-gram-matrix-orthogonal-with-unequal-squared-norms"></a>
![](legendre-polynomial-shapes-and-gram-matrix.png)

**[Figure 1](#image-the-first-four-legendre-polynomials-and-their-exact-integral-gram-matrix-orthogonal-with-unequal-squared-norms). The first four Legendre polynomials and their exact integral Gram matrix: orthogonal, with unequal squared norms**.

For these four [polynomials](polynomial-split.md), a short verification expands each product and uses $\int_{-1}^1x^{2j+1}\,dx=0$ and $\int_{-1}^1x^{2j}\,dx=2/(2j+1)$. For example, $\langle P_0,P_2\rangle=(3(2/3)-2)/2=0$ and $\langle P_1,P_3\rangle=(5(2/5)-3(2/3))/2=0$. The same calculation gives the diagonal entries $2,2/3,2/5,2/7$. More generally, apply the [Gram-Schmidt process](gram-schmidt-process.md) to the [monomial basis](monomial-basis.md) $1,x,x^2,\ldots$: at step $n$, subtract projections onto the earlier [polynomials](polynomial-split.md). The result retains its leading term, has degree $n$, and has positive [norm](norm.md), proving existence without a differential equation. Different degrees also give [linear independence](linear-independence.md), so $p_0,\ldots,p_m$ form a [basis](basis.md) of the [polynomials](polynomial-split.md) of degree at most $m$.

This [basis](basis.md) turns [least-squares solutions](least-squares-solution-of-a-linear-inverse-problem.md) for [functions](function-split.md) into independent scalar calculations, as the [decoupled coefficients of orthogonal polynomial projections](decoupled-coefficients-of-orthogonal-polynomial-projections.md) show. In a [spectral method](spectral-method.md), increasing the degree enlarges the approximation space while keeping earlier projection [coefficients](coefficient.md) fixed. Weighted [integrals](integral-split.md) also connect the same [orthogonal polynomials](orthogonal-polynomial-split.md) to [Gaussian quadrature](gaussian-quadrature.md): its nodes are [polynomial roots](root-of-a-polynomial.md) of a member of the family. The projection problem minimizes an integrated squared error; [Gaussian quadrature](gaussian-quadrature.md) uses the family to choose evaluation points for an [integral](integral-split.md).

**Table of contents**

- [Rodrigues' formula](rodrigues-formula.md)
- [Decoupled coefficients of orthogonal polynomial projections](decoupled-coefficients-of-orthogonal-polynomial-projections.md)
  - [Legendre least-squares projections of a cubic](legendre-least-squares-projections-of-a-cubic.md)
- [Kravchuk polynomials](kravchuk-polynomials.md)
- [Orthogonality forces many interior zeros](orthogonality-forces-many-interior-zeros.md)
- [Zernike polynomials](zernike-polynomials.md)
  - [Zernike spherical mode](zernike-spherical-mode.md)
- [Monic orthogonal polynomial](monic-orthogonal-polynomial.md)
  - [Three-term recurrence for monic orthogonal polynomials](three-term-recurrence-for-monic-orthogonal-polynomials.md)
- [Hermite polynomial](hermite-polynomial.md)
  - [Hermite polynomial derivative recurrence](hermite-polynomial-derivative-recurrence.md)
  - [Hermite function](hermite-function.md)
    - [Hermite functions are Fourier eigenfunctions](hermite-functions-are-fourier-eigenfunctions.md)
    - [Mehler formula for Hermite functions](mehler-formula-for-hermite-functions.md)
  - [Probabilists' Hermite polynomial](probabilists-hermite-polynomial.md)
    - [Space-time Hermite polynomial](space-time-hermite-polynomial.md)
- [Zeros of orthogonal polynomials](zeros-of-orthogonal-polynomials.md)
- [Jacobi matrix](jacobi-matrix.md)

## ↑ Ancestors (5)

1. [Numerical analysis](numerical-analysis-split.md)
2. [Analysis](analysis-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (32)

- [Basis](basis.md)
- [Chebyshev polynomial](chebyshev-polynomial.md)
- [Decoupled coefficients of orthogonal polynomial projections](decoupled-coefficients-of-orthogonal-polynomial-projections.md)
- [Legendre least-squares projections of a cubic](legendre-least-squares-projections-of-a-cubic.md)
- [Normalization of the ordinary Laguerre polynomials](normalization-of-the-ordinary-laguerre-polynomials.md)
- [Orthogonal polynomial](orthogonal-polynomial-split.md)
- [Orthogonal polynomial contrast](orthogonal-polynomial-contrast.md)
- [Orthogonal projection onto a finite-dimensional subspace](orthogonal-projection-onto-a-finite-dimensional-subspace.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ib/paper-3/6b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/ib/paper-2/9a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ib/paper-4/8f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ii/paper-3/2f/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ib/paper-3/19f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ib/paper-4/8d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ib/paper-4/8c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/ib/paper-4/1g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/ib/paper-4/8c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ib/paper-1/6d/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ib/paper-2/16d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ib/paper-3/19c/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ib/paper-1/18c/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-2/2h/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ib/paper-4/6b/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/ib/paper-3/17b/a/solution.md)
- [Recurrence relation](recurrence-relation.md)
- [René F. Swarttouw](rene-f-swarttouw.md)
- [Rodrigues' formula](rodrigues-formula.md)
- [Roelof Koekoek](roelof-koekoek.md)
- [Tom H. Koornwinder](tom-h-koornwinder.md)
- [Two-node Gaussian quadrature with sine weight](two-node-gaussian-quadrature-with-sine-weight.md)
- [Vandermonde determinant invariance under monic basis change](vandermonde-determinant-invariance-under-monic-basis-change.md)
- [Zernike polynomials](zernike-polynomials.md)
