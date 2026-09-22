# Argument principle

↑ **Parent:** [Complex analysis](complex-analysis-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Argument_principle)

The argument principle turns a boundary journey into an interior count: follow the values of a [meromorphic function](meromorphic-function.md) around a [contour](complex-integration-contour.md), and count their net turns around zero. Every enclosed [zero of a function](zero-of-a-function.md) contributes its [multiplicity of a zero](multiplicity-of-a-zero.md); every enclosed [pole](pole.md) subtracts its order. There is no need to find each [zero of a function](zero-of-a-function.md) separately.

Let $\gamma$ be a [piecewise smooth](piecewise-smooth-curve.md) [simple closed curve](simple-closed-curve.md) with [positive orientation of a contour](positive-orientation-of-a-contour.md). Suppose $f$ is a [meromorphic function](meromorphic-function.md) on an open [neighborhood](neighbourhood-mathematics.md) of the curve and its interior, with no [zeros of a function](zero-of-a-function.md) or [poles](pole.md) on $\gamma$. Then

$$
\boxed{N-P=\frac1{2\pi i}\oint_\gamma\frac{f'(z)}{f(z)}\,dz=\operatorname{wind}(f\circ\gamma,0)}.
$$

Here $N$ is the sum of the [zero multiplicities](multiplicity-of-a-zero.md) inside $\gamma$, and $P$ is the sum of the orders of its enclosed [poles](pole.md). The [image](image-of-a-function.md) [contour](complex-integration-contour.md) $f\circ\gamma$ may cross itself or revisit a point. Its signed [winding number](winding-number.md), rather than the number of visually bounded regions, is the quantity that counts.[§11.2, Theorems 11.1 and 11.4, pp. 1–3](topic-11-argument-principle-by-jeremy-orloff.md)

For the [polynomial](polynomial-split.md) $f(z)=z^3$ and the [unit circle](complex-unit-circle.md) $\gamma(t)=e^{it}$, $0\leq t\leq2\pi$, the [image](image-of-a-function.md) is $e^{3it}$. It goes around zero three times although its drawn outline is just one circle. The interior contains one distinct [zero of a function](zero-of-a-function.md), at zero, with [multiplicity of a zero](multiplicity-of-a-zero.md) three: **the count is three**. Reversing the [orientation of a contour](orientation-of-a-contour.md) reverses the [winding number](winding-number.md) and the sign of the [contour integral](contour-integral.md).

An [argument](argument-complex-analysis.md) must be followed continuously along the journey. Subtracting the principal [arguments](argument-complex-analysis.md) at the endpoints loses whole turns: a closed [image](image-of-a-function.md) [contour](complex-integration-contour.md) has the same endpoint value even when its [winding number](winding-number.md) is nonzero. Nor does [winding number](winding-number.md) zero prove that there are no [zeros of a function](zero-of-a-function.md): one enclosed simple [zero of a function](zero-of-a-function.md) and one enclosed simple [pole](pole.md) cancel in $N-P$. Known [poles](pole.md) must be added back to recover $N$.

The mechanism is short. Near a [zero of a function](zero-of-a-function.md) of order $m$, factor $f(z)=(z-a)^m g(z)$ with $g$ a nonvanishing [holomorphic function](holomorphic-function.md). Its [logarithmic derivative](logarithmic-derivative.md) is $f'/f=m/(z-a)+g'/g$, so its [residue](residue.md) is $m$. A [pole](pole.md) of order $m$ gives [residue](residue.md) $-m$. The [residue theorem](residue-theorem.md) adds those contributions. Changing variables to $w=f(z)$ identifies the resulting [contour integral](contour-integral.md) with the [winding number](winding-number.md). This is a local algebraic count joined to a global geometric count.[Topic 11: Argument Principle by Jeremy Orloff](topic-11-argument-principle-by-jeremy-orloff.md)

The usefulness goes beyond explicit [polynomials](polynomial-split.md). [Rouché's theorem](rouche-s-theorem.md) keeps a count unchanged when a boundary [perturbation](perturbation.md) cannot push the [image](image-of-a-function.md) [contour](complex-integration-contour.md) through zero. The [Nyquist stability criterion](nyquist-stability-criterion.md) applies the same counting idea to [poles](pole.md) governing a system under [feedback control](closed-loop-control.md).[§11.2.3 and §11.3.6](topic-11-argument-principle-by-jeremy-orloff.md)

**Table of contents**

- [Argument principle for a rational function](argument-principle-for-a-rational-function.md)
- [Weighted argument principle](weighted-argument-principle.md)
- [Boundary sampling can miss winding](boundary-sampling-can-miss-winding.md)
- [Radial crossing test for polynomial root counts](radial-crossing-test-for-polynomial-root-counts.md)
- [Quarter-sector winding test for a real quartic](quarter-sector-winding-test-for-a-real-quartic.md)
- [Rouché's theorem](rouche-s-theorem.md)
  - [Rouché localization of polynomial roots](rouche-localization-of-polynomial-roots.md)
  - [Hurwitz's theorem](hurwitz-s-theorem.md)
  - [Open mapping theorem (complex analysis)](open-mapping-theorem-complex-analysis.md)
    - [Maximum modulus principle from the complex open mapping theorem](maximum-modulus-principle-from-the-complex-open-mapping-theorem.md)
  - [Unit-disc image from a boundary modulus lower bound](unit-disc-image-from-a-boundary-modulus-lower-bound.md)
- [Integer residue of a logarithmic derivative](integer-residue-of-a-logarithmic-derivative.md)

## ↑ Ancestors (5)

1. [Complex analysis](complex-analysis-split.md)
2. [Analysis](analysis-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (38)

- [A univalent function has nonzero derivative](a-univalent-function-has-nonzero-derivative.md)
- [Elliptic collinearity determinant](elliptic-collinearity-determinant.md)
- [1 Algebraic and Analytic Methods](nist-digital-library-of-mathematical-functions/1-algebraic-and-analytic-methods.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-8/1/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-8/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-8/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ib/paper-3/13g/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-26/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-5/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-5/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/ib/paper-4/13e/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-24/4/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/ib/paper-4/14e/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/ib/paper-4/4e/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-26/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-26/3/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-86/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ib/paper-3/14h/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ib/paper-3/14h/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ib/paper-4/4h/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ii/paper-2/23f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ib/paper-3/14e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-33/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ii/paper-1/23g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-126/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-2/21f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-203/1/e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ib/paper-3/13f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ib/paper-3/13f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/ib/paper-3/13e/solution.md)
- [Power-product map to a slit half-plane](power-product-map-to-a-slit-half-plane.md)
- [Quarter-sector winding test for a real quartic](quarter-sector-winding-test-for-a-real-quartic.md)
- [Radial crossing test for polynomial root counts](radial-crossing-test-for-polynomial-root-counts.md)
- [Topic 11: Argument Principle by Jeremy Orloff](topic-11-argument-principle-by-jeremy-orloff.md)
- [Weighted argument principle](weighted-argument-principle.md)
- [Winding number](winding-number.md)
- [Zero-pole sum of an elliptic function](zero-pole-sum-of-an-elliptic-function.md)
- [Zeros of theta functions with characteristics](zeros-of-theta-functions-with-characteristics.md)
