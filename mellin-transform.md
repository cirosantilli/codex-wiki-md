# Mellin transform

↑ **Parent:** [Integral transform](integral-transform.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Mellin_transform)

The [Mellin transform](mellin-transform.md) is an [integral transform](integral-transform.md) suited to changes of scale: replacing $f(x)$ by $f(ax)$ multiplies its transform by $a^{-s}$ for $a>0$. For a [locally integrable function](locally-integrable-function.md) $f:(0,\infty)\to\mathbb C$, define

$$
\mathcal Mf(s)=\int_0^\infty x^{s-1}f(x)\,dx,\qquad s=\sigma+i\tau,
$$

where the [improper integral](improper-integral.md) converges. The [complex number](complex-number.md) $x^{s-1}=\exp((s-1)\log x)$ uses the real [natural logarithm](natural-logarithm.md) because $x>0$. Its [absolute value](absolute-value.md) is $x^{\sigma-1}$, so [absolute convergence](absolute-convergence.md) depends on the [real part](real-part.md) $\sigma$ rather than the [imaginary part](imaginary-part.md) $\tau$. The [Mellin fundamental strip](fundamental-strip-of-a-mellin-transform.md) records the open range of such [real parts](real-part.md).[Chapter 2, §2.5(i), equation 2.5.1 and the following strip-of-analyticity paragraph](nist-digital-library-of-mathematical-functions.md)

A familiar example is the [exponential function](exponential-function.md) $f(x)=e^{-x}$:

$$
\mathcal M\{e^{-x}\}(s)=\Gamma(s),\qquad \operatorname{Re}s>0.
$$

This is exactly the [Gamma integral](gamma-integral.md). Near zero $e^{-x}$ tends to one, so [absolute convergence](absolute-convergence.md) requires $\sigma>0$; at infinity $x^r e^{-x}\to0$ for every real $r$, so there is no upper boundary. The [Gamma function](gamma-function.md) has a [meromorphic continuation](meromorphic-continuation.md) with [simple poles](simple-pole.md) at $0,-1,-2,\ldots$, but a finite continued value elsewhere in $\sigma\leq0$ does not make the defining [improper integral](improper-integral.md) converge.[Chapter 5, §5.2(i), equation 5.2.1, its Re z \> 0 condition, and the following analytic-continuation paragraph](nist-digital-library-of-mathematical-functions.md)

The [Mellin transform of an interval indicator](mellin-transform-of-an-interval-indicator.md) gives an elementary example with [absolute convergence](absolute-convergence.md) for every [complex number](complex-number.md) $s$. The [Mellin transform in logarithmic coordinates](mellin-transform-in-logarithmic-coordinates.md) explains why changes of scale become [translations](translation-geometry.md), connecting the [scaling property of the Mellin transform](scaling-property-of-the-mellin-transform.md) to the [Fourier transform](fourier-transform.md).

**Table of contents**

- [Mellin transform of an interval indicator](mellin-transform-of-an-interval-indicator.md)
- [Fundamental strip of a Mellin transform](fundamental-strip-of-a-mellin-transform.md)
- [Scaling property of the Mellin transform](scaling-property-of-the-mellin-transform.md)
- [Mellin transform in logarithmic coordinates](mellin-transform-in-logarithmic-coordinates.md)
- [Imaginary-part regularization at a zero Mellin exponent](imaginary-part-regularization-at-a-zero-mellin-exponent.md)
- [Mellin transform of call prices](mellin-transform-of-call-prices.md)
- [Meromorphic continuation of a Mellin transform from an asymptotic expansion](meromorphic-continuation-of-a-mellin-transform-from-an-asymptotic-expansion.md)
  - [Accumulating asymptotic exponents obstruct Mellin continuation](accumulating-asymptotic-exponents-obstruct-mellin-continuation.md)
- [Mellin inversion theorem](mellin-inversion-theorem.md)

## ↑ Ancestors (5)

1. [Integral transform](integral-transform.md)
2. [Analysis](analysis-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (40)

- [Accumulating asymptotic exponents obstruct Mellin continuation](accumulating-asymptotic-exponents-obstruct-mellin-continuation.md)
- [Additive twist of a cusp-form L-function](additive-twist-of-a-cusp-form-l-function.md)
- [Epstein zeta function](epstein-zeta-function.md)
- [Functional equation of an additive cusp-form twist](functional-equation-of-an-additive-cusp-form-twist.md)
- [Fundamental strip of a Mellin transform](fundamental-strip-of-a-mellin-transform.md)
- [L-function of a cusp form](l-function-of-a-cusp-form.md)
- [Mellin continuation of a noncuspidal modular form](mellin-continuation-of-a-noncuspidal-modular-form.md)
- [Mellin transform](mellin-transform.md)
- [Mellin transform in logarithmic coordinates](mellin-transform-in-logarithmic-coordinates.md)
- [Mellin transform of an interval indicator](mellin-transform-of-an-interval-indicator.md)
- [Meromorphic continuation of a Mellin transform from an asymptotic expansion](meromorphic-continuation-of-a-mellin-transform-from-an-asymptotic-expansion.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-26/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-26/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-24/3/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-24/3/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-24/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-28/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-88/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-88/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-30/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-33/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-33/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-55/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ii/paper-1/6b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ii/paper-2/11b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-126/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-137/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-137/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-137/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-211/2/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-137/2/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-117/2/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-137/1/c/solution.md)
- [Phase-normalized Fricke functional equation](phase-normalized-fricke-functional-equation.md)
- [Pole-subtracted theta integral for an Epstein zeta function](pole-subtracted-theta-integral-for-an-epstein-zeta-function.md)
- [Pole-subtracted theta integral for the completed zeta function](pole-subtracted-theta-integral-for-the-completed-zeta-function.md)
- [Rational-cusp inversion of a level-one cusp form](rational-cusp-inversion-of-a-level-one-cusp-form.md)
- [Scaling property of the Mellin transform](scaling-property-of-the-mellin-transform.md)
- [Smoothed prime number theorem from a zero-free region](smoothed-prime-number-theorem-from-a-zero-free-region.md)
- [Zero-mode correction to the spectral zeta value](zero-mode-correction-to-the-spectral-zeta-value.md)
