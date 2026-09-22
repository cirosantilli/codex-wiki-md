# Vanishing moment

↑ **Parent:** [Wavelet](wavelet.md)

A [vanishing moment](vanishing-moment.md) is a cancellation condition: positive and negative parts of an analyzing [function](function-split.md) balance when weighted by a [monomial](monomial.md). Having $q$ [vanishing moments](vanishing-moment.md) means that the first $q$ such balances hold, starting with the unweighted [integral](integral-split.md):

$$
\int_{\mathbb R}x^r\psi(x)\,dx=0,\qquad r=0,\ldots,q-1,\qquad q\geq1.
$$

Consequently a [wavelet](wavelet.md) ignores local [polynomial](polynomial-split.md) trends of [degree of a polynomial](degree-of-a-polynomial.md) less than $q$. A [smooth](smooth-function.md) feature is close to its [Taylor polynomial](taylor-polynomial.md), so only the small [Taylor remainder](taylor-remainder.md) contributes to its detail coefficient. A [jump discontinuity](jump-discontinuity.md) cannot be approximated this way across its edge; its [jump response of a localized analyzing function](jump-response-of-a-localized-analyzing-function.md) can remain large relative to details from a [smooth](smooth-function.md) region.[Wavelet Bases, §7.2.1, printed p. 206, equation (7.69) and the paragraph explaining cancellation of Taylor polynomials](a-wavelet-tour-of-signal-processing-by-stephane-mallat/wavelet-bases.md)

These are ordinary absolutely convergent [integrals](integral-split.md), not a prescription for assigning values to divergent expressions. A sufficient assumption is

$$
\int_{\mathbb R}(1+|x|^{q-1})|\psi(x)|\,dx<\infty.
$$

It makes $ψ$ and all $x^r\psi$ for $r<q$ [integrable functions](lebesgue-integrable-function.md). Being [square-integrable](square-integrable-function.md) alone does not ensure these weighted [integrals](integral-split.md) exist. For a [square-integrable function](square-integrable-function.md) with [compact support](compact-support.md), the [Cauchy-Schwarz inequality](cauchy-schwarz-inequality.md) guarantees every such weighted [integral](integral-split.md) is finite. Saying **exactly $q$** [vanishing moments](vanishing-moment.md) additionally requires an existing, nonzero next [integral](integral-split.md) $\int x^q\psi(x)\,dx$; the usual phrase “has $q$” allows more cancellation.

**Table of contents**

- [Wavelet polynomial annihilation](wavelet-polynomial-annihilation.md)
- [Second-difference analyzing function](second-difference-analyzing-function.md)
- [Jump response of a localized analyzing function](jump-response-of-a-localized-analyzing-function.md)
- [Vanishing moments and Fourier zeros](vanishing-moments-and-fourier-zeros.md)
- [Smooth-mask vanishing-moment criterion](smooth-mask-vanishing-moment-criterion.md)
  - [Integer-frequency zeros of a scaling function](integer-frequency-zeros-of-a-scaling-function.md)

## ↑ Ancestors (6)

1. [Wavelet](wavelet.md)
2. [Fourier analysis](fourier-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (22)

- [Best N-term wavelet approximation of piecewise Hölder functions](best-n-term-wavelet-approximation-of-piecewise-holder-functions.md)
- [Boundary wavelet](boundary-wavelet.md)
- [Daubechies wavelet](daubechies-wavelet.md)
- [Haar wavelet](haar-wavelet.md)
- [Interval-adapted wavelet basis](interval-adapted-wavelet-basis.md)
- [Jump response of a localized analyzing function](jump-response-of-a-localized-analyzing-function.md)
- [Lacunary scaling-phase regularity counterexample](lacunary-scaling-phase-regularity-counterexample.md)
- [Moment differentiation of the Fourier transform](moment-differentiation-of-the-fourier-transform.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-340/1/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-340/2/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-340/1/e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-340/2/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-340/3/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-340/3/e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-340/6/solution.md)
- [Piecewise polynomial function](piecewise-polynomial-function.md)
- [Second-difference analyzing function](second-difference-analyzing-function.md)
- [Smooth-mask vanishing-moment criterion](smooth-mask-vanishing-moment-criterion.md)
- [Vanishing moment](vanishing-moment.md)
- [Vanishing moments and Fourier zeros](vanishing-moments-and-fourier-zeros.md)
- [Wavelet coefficient decay for Hölder functions](wavelet-coefficient-decay-for-holder-functions.md)
- [Wavelet polynomial annihilation](wavelet-polynomial-annihilation.md)
