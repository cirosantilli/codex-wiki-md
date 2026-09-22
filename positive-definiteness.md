# Positive definiteness

↑ **Parent:** [Positive-definite bilinear form](positive-definite-bilinear-form.md)

The strict positivity of a [quadratic form](quadratic-form-split.md) on every nonzero [vector](vector.md). A real symmetric [matrix](matrix.md) has positive definiteness exactly when its associated [quadratic form](quadratic-form-split.md) does, making it a [positive-definite matrix](positive-definite-matrix.md). A [Hermitian form](hermitian-form.md) is positive definite when its value on $(v,v)$ is real and strictly positive for every nonzero vector.

Think of a [positive-definite quadratic form](positive-definite-quadratic-form.md) as an energy cost for a displacement: every direction costs something, and zero cost identifies the origin. For example, the real [symmetric matrix](symmetric-matrix.md)

$$
A=\begin{pmatrix}3&1\\1&3\end{pmatrix},\qquad q(x,y)=3x^2+2xy+3y^2=3\left(x+\frac y3\right)^2+\frac83y^2
$$

is a [positive-definite matrix](positive-definite-matrix.md) because the two squares can vanish together only at $(0,0)$. The mixed term couples the [coordinates](coordinate-linear-algebra.md), but cannot overwhelm their positive contributions: $q(1,1)=8$ and $q(1,-1)=4$. The graph is a bowl, and its positive [level sets](level-set.md) are [ellipses](ellipse.md) with axes along the [eigenvectors](eigenvector.md), rather than along the original [coordinates](coordinate-linear-algebra.md).

<a id="image-positive-quadratic-energy-bowl-and-elliptical-level-curves"></a>
![](positive-quadratic-energy-elliptical-levels.png)

**[Figure 3](#image-positive-quadratic-energy-bowl-and-elliptical-level-curves). Positive quadratic energy bowl and elliptical level curves**.

The real and complex settings require different symmetry assumptions. For a real [symmetric matrix](symmetric-matrix.md) use $q(x)=x^TAx$ with $x\in\mathbb R^n$; for a complex [Hermitian matrix](hermitian-operator.md) use $q(z)=z^*Az$ with $z\in\mathbb C^n$, where $z^*$ is the [conjugate transpose](conjugate-transpose.md). The latter expression is real, so strict positivity is meaningful. A complex [quadratic form](quadratic-form-split.md) such as $z_1^2+z_2^2$ has no such positivity: it vanishes at $(1,i)$ and takes negative real values at $(i,0)$. A [Hermitian form](hermitian-form.md) uses [complex conjugation](complex-conjugation.md), which changes this example to $|z_1|^2+|z_2|^2$.

For a real [matrix](matrix.md) $M$ without a symmetry hypothesis, its [quadratic form](quadratic-form-split.md) depends only on its [symmetric part of a matrix](symmetric-part-of-a-matrix.md):

$$
x^TMx=x^T\frac{M+M^T}{2}x.
$$

Positive [eigenvalues](eigenvalue.md) of $M$ alone do not establish [positive definiteness](positive-definiteness.md) of this [quadratic form](quadratic-form-split.md). For example, $M=\begin{pmatrix}1&4\\0&1\end{pmatrix}$ has both [eigenvalues](eigenvalue.md) equal to $1$, yet $q(1,-1)=1-4+1=-2$. The relevant test is positivity of the [symmetric part of a matrix](symmetric-part-of-a-matrix.md), not the [spectrum](spectrum-functional-analysis.md) of an arbitrary [matrix](matrix.md).[Theorem 1.7, equation (1.3), p. 3: symmetric and alternating parts](bilinear-forms-by-keith-conrad.md)

**Table of contents**

- [Two-by-two positive-definiteness test](two-by-two-positive-definiteness-test.md)
- [Positive-definiteness threshold in a two-by-two family](positive-definiteness-threshold-in-a-two-by-two-family.md)
- [Ellipsoid level sets of a positive-definite quadratic form](ellipsoid-level-sets-of-a-positive-definite-quadratic-form.md)
- [Unique minimizer of a positive-definite quadratic function](unique-minimizer-of-a-positive-definite-quadratic-function.md)

## ↑ Ancestors (8)

1. [Positive-definite bilinear form](positive-definite-bilinear-form.md)
2. [Symmetric bilinear form](symmetric-bilinear-form.md)
3. [Bilinear form](bilinear-form-split.md)
4. [Linear algebra](linear-algebra-split.md)
5. [Algebra](algebra-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (41)

- [Cholesky decomposition as a sum of squares](cholesky-decomposition-as-a-sum-of-squares.md)
- [Coercive bilinear form](coercive-bilinear-form.md)
- [Determinant pairing is not an inner product](determinant-pairing-is-not-an-inner-product.md)
- [Discrete sampling inner product on polynomial spaces](discrete-sampling-inner-product-on-polynomial-spaces.md)
- [Hermitian form](hermitian-form.md)
- [Hermitian inner product](hermitian-inner-product.md)
- [Hessian matrix](hessian-matrix.md)
- [Matrix decomposition](matrix-decomposition.md)
- [Miscibility criterion for a two-component condensate](miscibility-criterion-for-a-two-component-condensate.md)
- [Nondegenerate bilinear form](nondegenerate-bilinear-form.md)
- [Orthogonal polynomials for the absolute-value weight](orthogonal-polynomials-for-the-absolute-value-weight.md)
- [Solution](past-exam-of-the-algebra-1-and-differential-equations-1-course-of-the-university-of-oxford/2014/3/b/ii/solution.md)
- [Solution](past-exam-of-the-algebra-1-and-differential-equations-1-course-of-the-university-of-oxford/2015/3/a/iii/solution.md)
- [Solution](past-exam-of-the-algebra-1-and-differential-equations-1-course-of-the-university-of-oxford/2015/3/b/i/solution.md)
- [Solution](past-exam-of-the-algebra-analysis-and-differential-equations-1-course-of-the-university-of-oxford/2010/2/c/solution.md)
- [Solution](past-exam-of-the-algebra-analysis-and-differential-equations-1-course-of-the-university-of-oxford/2011/2/b/solution.md)
- [Solution](past-exam-of-the-algebra-analysis-and-differential-equations-1-course-of-the-university-of-oxford/2013/algebra/2/a/solution.md)
- [Solution](past-exam-of-the-algebra-analysis-and-differential-equations-2-course-of-the-university-of-oxford/2007/2/solution.md)
- [Solution](past-exam-of-the-algebra-and-analysis-i-for-mathematics-and-philosophy-course-of-the-university-of-oxford/2013/algebra/2/a/solution.md)
- [Solution](past-exam-of-the-calculus-of-variations-course-of-the-university-of-oxford/2009/2/a/solution.md)
- [Solution](past-exam-of-the-elasticity-and-plasticity-course-of-the-university-of-oxford/2008/1/b/solution.md)
- [Solution](past-exam-of-the-elasticity-and-plasticity-course-of-the-university-of-oxford/2008/1/d/solution.md)
- [Solution](past-exam-of-the-linear-algebra-course-of-the-university-of-oxford/2023/3/a/ii/solution.md)
- [Solution](past-exam-of-the-linear-algebra-course-of-the-university-of-oxford/2023/3/b/ii/solution.md)
- [Solution](past-exam-of-the-mathematical-methods-i-course-of-the-university-of-oxford/2014-resit/11/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-32/2/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/ib/paper-2/12e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-21/4/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-46/1/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-83/4/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-oxford/2015/prelims/mathematics-i/4/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-oxford/2015/prelims/mathematics-iii/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-oxford/2021/prelims/mathematics-i/4/a/i/solution.md)
- [Solution](past-exam-of-the-numerical-linear-algebra-course-of-the-university-of-oxford/2011/2/a/solution.md)
- [Solution](past-exam-of-the-numerical-linear-algebra-course-of-the-university-of-oxford/2011/2/c/solution.md)
- [Solution](past-exam-of-the-numerical-linear-algebra-course-of-the-university-of-oxford/2011/3/a/solution.md)
- [Solution](past-exam-of-the-numerical-linear-algebra-course-of-the-university-of-oxford/2011/3/c/solution.md)
- [Solution](past-exam-of-the-options-ii-course-of-the-university-of-oxford/2004/f/f2/b/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2022/discrete-mathematics-continuous-mathematics-and-probability-resit/5/a/ii/solution.md)
- [Positive definiteness](positive-definiteness.md)
- [Sylvester's criterion](sylvester-s-criterion.md)
