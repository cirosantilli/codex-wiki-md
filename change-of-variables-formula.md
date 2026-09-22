# Change of variables formula

↑ **Parent:** [Multivariable calculus](multivariable-calculus.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Change_of_variables_formula)

The [change of variables formula](change-of-variables-formula.md) expresses an [integral](integral.md) in coordinates that make its [integrand](integrand.md) or its region simpler. Three ingredients change together: the region, the [function](function-split.md) being integrated, and the element of [area](surface-area.md) or volume. The last change is measured by the absolute [Jacobian determinant](jacobian-determinant.md); forgetting it amounts to counting transformed cells as though their sizes had stayed the same.

In one dimension, substitution is the integrated [chain rule](chain-rule.md). If $g$ is [continuously differentiable](continuously-differentiable-function.md) on $[a,b]$ and $f$ is [continuous](continuous-function.md) on its image, then

$$
\int_a^b f(g(x))g'(x)\,dx=\int_{g(a)}^{g(b)}f(u)\,du.
$$

These are directed [definite integrals](definite-integral.md): if $g$ decreases, the transformed endpoints reverse. This identity does not require $g$ to be [injective](injective-function.md), because an [antiderivative](antiderivative.md) composed with $g$ already accounts for any backtracking.[OpenStax, Calculus Volume 1, Section 5.5: Substitution](https://openstax.org/books/calculus-volume-1/pages/5-5-substitution)

For a concrete computation, set $u=1+x^2$, so $du=2x\,dx$. The endpoints $x=0,1$ become $u=1,2$:

$$
\int_0^1\frac{2x}{1+x^2}\,dx=\int_1^2\frac{du}{u}=[\ln u]_1^2=\ln 2\approx0.693147.
$$

The numerator is precisely the [derivative](derivative.md) of the expression in the denominator. Substitution reveals the familiar [natural logarithm](natural-logarithm.md) hidden inside this [rational function](rational-function.md). Keeping the original endpoints after changing the [integrand](integrand.md) would describe a different [integral](integral.md).

For the elementary two-dimensional theorem, let $T:U\to V$ be a $C^1$ [diffeomorphism](diffeomorphism.md) between [open sets](open-set.md) in the plane, let $S\subset U$ be a bounded region with piecewise smooth boundary, and let $f$ be [continuous](continuous-function.md) on $T(S)$, with the displayed [integrals](integral.md) finite. Then

$$
\iint_{T(S)}f(x,y)\,dx\,dy=\iint_S f(T(u,v))|\det DT(u,v)|\,du\,dv.
$$

Here $DT$ is the [Jacobian matrix](jacobian-matrix.md). The [diffeomorphism](diffeomorphism.md) assumption means a [bijection](bijection.md) with a [continuously differentiable](continuously-differentiable-function.md) inverse, and ensures a nonzero [Jacobian determinant](jacobian-determinant.md). This excludes overlapping sheets; the more general [area formula](area-formula-geometric-measure-theory.md) handles multiplicity.[MIT 18.022: The change of variables theorem](https://math.mit.edu/~larsh/teaching/F2007/handouts/changeofvariables.pdf)

Take $S=[0,1]^2$ and the [linear map](linear-map.md)

$$
T(u,v)=(2u+v,v),\qquad DT=\begin{pmatrix}2&1\\0&1\end{pmatrix},\qquad \det DT=2.
$$

Its inverse is $(u,v)=((x-y)/2,y)$. The square becomes a [parallelogram](parallelogram.md) with vertices $(0,0),(2,0),(3,1),(1,1)$: base two, height one, [area](surface-area.md) two. Consequently $\iint_{T(S)}1\,dx\,dy=\iint_S2\,du\,dv=2$. A nonconstant [integrand](integrand.md) changes too: $\iint_{T(S)}x\,dx\,dy=\int_0^1\int_0^1(2u+v)2\,du\,dv=3$.

The direction of the map matters when selecting the factor. Here $T$ goes from the new coordinates to the original coordinates, so the factor is two. Its inverse has [Jacobian determinant](jacobian-determinant.md) $1/2$, appropriate for converting [area](surface-area.md) in the opposite direction. Writing down the map before computing its [Jacobian matrix](jacobian-matrix.md) prevents a reciprocal-factor error.

<a id="image-a-unit-square-becomes-a-parallelogram-of-area-two-reflection-changes-the-determinant-sign-but-preserves-area"></a>
![](change-of-variables-area.png)

**[Figure 33](#image-a-unit-square-becomes-a-parallelogram-of-area-two-reflection-changes-the-determinant-sign-but-preserves-area). A unit square becomes a parallelogram of area two; reflection changes the determinant sign but preserves area**.

Now reflect the image vertically: $\widetilde T(u,v)=(2u+v,-v)$ has [Jacobian determinant](jacobian-determinant.md) $-2$, but still produces [area](surface-area.md) two. The sign records reversal of the [orientation of a vector space](orientation-of-a-vector-space.md); ordinary [area](surface-area.md) uses its absolute value. For oriented [differential forms](differential-form-split.md), the [pullback of a differential form](pullback-of-a-differential-form.md) instead retains the signed [determinant](determinant.md).[MIT 18.952 notes: Integration of forms, Chapter 3](https://math.mit.edu/classes/18.952/spring2013/docs/book.pdf)

The geometric beauty is that a nonlinear [differentiable map](differentiable-map.md) has a [local linear approximation](local-linear-approximation.md): tiny [rectangles](rectangle.md) behave approximately like these [parallelograms](parallelogram.md). Summing their scaled contributions gives the [change of variables formula](change-of-variables-formula.md). In [polar coordinates](polar-coordinates.md) this factor is $r$, explaining $dx\,dy=r\,dr\,d\theta$; equal angular steps cover more [area](surface-area.md) farther from the origin. Choosing suitable coordinates can simplify both the boundary and the [integrand](integrand.md).[OpenStax, Calculus Volume 3, Section 5.7: Change of variables in multiple integrals](https://openstax.org/books/calculus-volume-3/pages/5-7-change-of-variables-in-multiple-integrals)

**Table of contents**

- [Ordered-cone substitution by products and ratios](ordered-cone-substitution-by-products-and-ratios.md)
- [Ratio-product coordinates](ratio-product-coordinates.md)
- [Squared-radius difference substitution](squared-radius-difference-substitution.md)
- [Weighted inverse multiplicity](weighted-inverse-multiplicity.md)
- [Rational square diffeomorphism](rational-square-diffeomorphism.md)
- [Hyperbolic substitution](hyperbolic-substitution.md)
- [Monotone substitution inequality](monotone-substitution-inequality.md)
- [Area formula (geometric measure theory)](area-formula-geometric-measure-theory.md)
- [Polar coordinates](polar-coordinates.md)
  - [Cylindrical coordinate system](cylindrical-coordinate-system.md)
    - [Azimuthal derivative of a cylindrical vector Fourier mode](azimuthal-derivative-of-a-cylindrical-vector-fourier-mode.md)
    - [Cylindrical radius](cylindrical-radius.md)
  - [Cardioid](cardioid.md)
- [Orthogonal coordinates](orthogonal-coordinates.md)
  - [Del in cylindrical and spherical coordinates](del-in-cylindrical-and-spherical-coordinates.md)
  - [Hyperspherical coordinates](hyperspherical-coordinates.md)
    - [Spherical coordinate system](spherical-coordinate-system.md)
      - [Radial unit vector in spherical coordinates](radial-unit-vector-in-spherical-coordinates.md)
      - [Scale factors of orthogonal coordinates](scale-factors-of-orthogonal-coordinates.md)
      - [Curl in spherical coordinates](curl-in-spherical-coordinates.md)
    - [Volume of an n-ball](volume-of-an-n-ball.md)
    - [Surface area of an n-sphere](surface-area-of-an-n-sphere.md)

## ↑ Ancestors (7)

1. [Multivariable calculus](multivariable-calculus.md)
2. [Calculus](calculus-split.md)
3. [Real analysis](real-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (64)

- [Area formula (geometric measure theory)](area-formula-geometric-measure-theory.md)
- [Benford law from logarithmic uniformity](benford-law-from-logarithmic-uniformity.md)
- [Beta-prime distribution](beta-prime-distribution.md)
- [Change of variables formula](change-of-variables-formula.md)
- [Change-of-variables formula for a probability density](change-of-variables-formula-for-a-probability-density.md)
- [Cofactor matrix](cofactor-matrix.md)
- [Conformal invariance of the planar Dirichlet inner product](conformal-invariance-of-the-planar-dirichlet-inner-product.md)
- [Determinant](determinant.md)
- [Differential entropy under affine rescaling](differential-entropy-under-affine-rescaling.md)
- [Differential entropy under an increasing transformation](differential-entropy-under-an-increasing-transformation.md)
- [Double integral](double-integral.md)
- [Frequency and wavelength spectral radiance conversion](frequency-and-wavelength-spectral-radiance-conversion.md)
- [Jacobian determinant](jacobian-determinant.md)
- [Multiple integral](multiple-integral.md)
- [Odd-integrand cancellation by reflection](odd-integrand-cancellation-by-reflection.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/ia/paper-3/10a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-55/1/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-71/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ia/paper-3/10a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/ia/paper-3/10a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/ia/paper-2/11f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ia/paper-3/12a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-46/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-32/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ia/paper-2/11f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ia/paper-3/12c/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ia/paper-3/10c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/ia/paper-3/10c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-55/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-7/1/f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-7/2/g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/ia/paper-3/9c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-64/2/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-7/1/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-7/4/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ia/paper-2/9f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ia/paper-3/10c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-304/3/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-308/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ia/paper-3/3b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-4/2f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-132/3/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-203/2/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ia/paper-3/9c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-105/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ia/paper-3/9b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-1/7a/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-348/2/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ia/paper-1/3e/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ia/paper-1/3e/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-219/1/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-327/3/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-327/3/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ia/paper-3/3a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-327/1/b/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-327/1/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-3/35a/b/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-225/3/a/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-225/3/a/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-209/3/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-327/1/b/ii/solution.md)
- [Rational square diffeomorphism](rational-square-diffeomorphism.md)
- [Spectral radiant flux](spectral-radiant-flux.md)
- [Total variation under opposite smooth flows](total-variation-under-opposite-smooth-flows.md)
