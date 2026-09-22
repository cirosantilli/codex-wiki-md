# Polynomial least-squares approximation

↑ **Parent:** [Polynomial approximation](polynomial-approximation.md)

For a positive-definite weighted [inner product](inner-product-split.md) on a compact interval, a [least-squares polynomial](polynomial-least-squares-approximation.md) is the [orthogonal projection](orthogonal-projection.md) of a function onto the finite-dimensional space $\Pi_n$ of [polynomials](polynomial-split.md) of degree at most $n$. In a [basis](basis.md) $\phi_0,\ldots,\phi_n$, its coefficients solve the [normal equations](normal-equation.md) $Gc=d$, where $G_{ij}=(\phi_i,\phi_j)$ and $d_i=(u,\phi_i)$. The [Gram matrix](gram-matrix.md) is positive definite: $z^TGz=\|\sum z_i\phi_i\|^2>0$ for $z\ne0$. Thus the coefficients exist and are unique. The residual is [orthogonal](orthogonal-vectors.md) to every candidate polynomial, giving $\|u-q\|^2=\|u-p_n\|^2+\|p_n-q\|^2$ and proving optimality. An orthogonal basis makes these equations diagonal, as in a [least-squares polynomial in an orthogonal-polynomial basis](least-squares-polynomial-in-an-orthogonal-polynomial-basis.md).

**Table of contents**

- [Weighted linear projection of a semicircle profile](weighted-linear-projection-of-a-semicircle-profile.md)
- [Parity preservation by polynomial least-squares projection](parity-preservation-by-polynomial-least-squares-projection.md)

## ↑ Ancestors (6)

1. [Polynomial approximation](polynomial-approximation.md)
2. [Uniform approximation](uniform-approximation-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Solution](past-exam-of-the-numerical-analysis-course-of-the-university-of-oxford/2014/2/a/solution.md)
- [Solution](past-exam-of-the-options-i-course-of-the-university-of-oxford/2012/p/p1/a/solution.md)
- [Solution](past-exam-of-the-options-ii-course-of-the-university-of-oxford/2011/p/p3/a/solution.md)
- [Solution](past-exam-of-the-options-ii-course-of-the-university-of-oxford/2011/p/p3/c/solution.md)
