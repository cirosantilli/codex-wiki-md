# Matched asymptotic expansion

↑ **Parent:** [Singular perturbation](singular-perturbation-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Matched_asymptotic_expansion)

A [matched asymptotic expansion](matched-asymptotic-expansion.md) constructs approximations in regions with different [distinguished limits](distinguished-limit.md) and fixes their free constants by requiring agreement in an [overlap region](overlap-region.md). The [inner expansion](inner-expansion.md) resolves rapid variation; the [outer expansion](outer-expansion.md) describes the surrounding region. Matching compares their common limiting behavior, rather than imposing distant [boundary conditions](boundary-condition.md) directly on a local approximation.[§§4.3.3–4.3.4, pp. 57–58: inner expansion and matching](asymptotic-analysis-and-singular-perturbation-theory-by-john-k-hunter.md)

For the [singular perturbation](singular-perturbation-split.md) problem $\epsilon y''+y'=0$, $y(0)=0$, $y(1)=1$, the leading [outer solution](outer-expansion.md) is $y_0=1$. The [inner variable](inner-variable.md) $X=x/\epsilon$ gives $Y_0''+Y_0'=0$ and $Y_0(0)=0$, hence $Y_0=A(1-e^{-X})$. In the [overlap region](overlap-region.md) $\epsilon\ll x\ll1$, the [inner variable](inner-variable.md) tends to infinity while the outer coordinate tends to zero. The [asymptotic matching condition](asymptotic-matching-condition.md) is

$$
\lim_{X\to\infty}Y_0(X)=\lim_{x\to0^+}y_0(x)=1,
$$

so $A=1$. One concrete path through the [overlap region](overlap-region.md) is $x=\sqrt\epsilon$: then $x\to0$ and $X=\epsilon^{-1/2}\to\infty$. Matching selects the free constant that the left [boundary condition](boundary-condition.md) alone could not determine.

Why choose the right [boundary condition](boundary-condition.md) for the [outer solution](outer-expansion.md)? If instead one selects $y_0=0$ from the left, a proposed right [boundary layer](boundary-layer.md) with $Z=(1-x)/\epsilon$ satisfies $U_0''-U_0'=0$. Its [general solution](general-solution.md) is $A+B e^Z$. Matching to zero as $Z\to\infty$ forces $A=B=0$, contradicting $U_0(0)=1$. The direction in which the [exponential function](exponential-function.md) decays determines which endpoint can carry the [boundary layer](boundary-layer.md); endpoint selection is part of the calculation.

**Table of contents**

- [Endpoint derivative in a negative-drift boundary layer](endpoint-derivative-in-a-negative-drift-boundary-layer.md)
- [Logistic crossover in a weakly nonlinear Euler equation](logistic-crossover-in-a-weakly-nonlinear-euler-equation.md)
  - [Nonlinear crossover delayed by a small unstable-mode coefficient](nonlinear-crossover-delayed-by-a-small-unstable-mode-coefficient.md)
- [Nonlinear endpoint layer with a quadratic reaction](nonlinear-endpoint-layer-with-a-quadratic-reaction.md)
  - [One-third-power scaling at a nonlinear turning endpoint](one-third-power-scaling-at-a-nonlinear-turning-endpoint.md)
- [Asymptotic matching condition](asymptotic-matching-condition.md)
- [Square-root reaction problem with nested boundary layers](square-root-reaction-problem-with-nested-boundary-layers.md)
  - [First integral of a square-root reaction layer](first-integral-of-a-square-root-reaction-layer.md)
- [Nested layers at an essential singular endpoint](nested-layers-at-an-essential-singular-endpoint.md)
- [Matched expansion with square-root and logarithmic corrections](matched-expansion-with-square-root-and-logarithmic-corrections.md)
- [Logarithmic matching in a small-exponent boundary layer](logarithmic-matching-in-a-small-exponent-boundary-layer.md)
- [Gaussian interior layer of a conservative drift equation](gaussian-interior-layer-of-a-conservative-drift-equation.md)
- [Oscillatory endpoint with a quadratically vanishing drift](oscillatory-endpoint-with-a-quadratically-vanishing-drift.md)
- [First-order composite expansion for a positive drift](first-order-composite-expansion-for-a-positive-drift.md)
- [Logarithmically enhanced nonlinear boundary layer](logarithmically-enhanced-nonlinear-boundary-layer.md)
- [Boundary layer around a moving endpoint](boundary-layer-around-a-moving-endpoint.md)
- [Square-root boundary layer at a vanishing drift](square-root-boundary-layer-at-a-vanishing-drift.md)
  - [Error-function logarithmic switchback](error-function-logarithmic-switchback.md)
- [Overlap region](overlap-region.md)
- [Intermediate asymptotic region](intermediate-asymptotic-region.md)
- [Interior layer at a simple zero of advection](interior-layer-at-a-simple-zero-of-advection.md)
  - [Endpoint layers for reversed diffusion](endpoint-layers-for-reversed-diffusion.md)
- [Distinguished limit](distinguished-limit.md)
- [Inner expansion](inner-expansion.md)
  - [Square-root-degenerate endpoint layer](square-root-degenerate-endpoint-layer.md)
  - [Inner variable](inner-variable.md)
- [Outer expansion](outer-expansion.md)
- [Additive composite expansion](additive-composite-expansion.md)
- [Multiplicative composite expansion](multiplicative-composite-expansion.md)
- [Outflow boundary layer](outflow-boundary-layer.md)
- [Switchback term](switchback-term.md)
  - [Logarithmic overlap creates a switchback term](logarithmic-overlap-creates-a-switchback-term.md)

## ↑ Ancestors (7)

1. [Singular perturbation](singular-perturbation-split.md)
2. [Ordinary differential equation](ordinary-differential-equation.md)
3. [Differential equation](differential-equation-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (20)

- [Intermediate asymptotic region](intermediate-asymptotic-region.md)
- [Large solitary pulse on a cylindrical film](large-solitary-pulse-on-a-cylindrical-film.md)
- [Matched asymptotic expansion](matched-asymptotic-expansion.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-76/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-79/1/a/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-82/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-67/3/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-67/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-73/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-74/2/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-74/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-72/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-336/2/a/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-336/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-336/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-336/2/2/3/solution.md)
- [Perturbation theory](perturbation-theory.md)
- [Radial modified Helmholtz equation](radial-modified-helmholtz-equation.md)
- [Small-argument expansion of the exponential integral](small-argument-expansion-of-the-exponential-integral.md)
- [Uniform asymptotic approximation](uniform-asymptotic-approximation.md)
