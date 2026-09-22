# Wronskian

↑ **Parent:** [Second-order linear differential equation](second-order-linear-differential-equation.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Wronskian)

For two [differentiable functions](differentiable-function.md) $f,g$ on an [interval](interval-mathematics.md) $I$, their [Wronskian](wronskian.md) is the [function](function-split.md)

$$
W(f,g)(x)=\det\begin{pmatrix}f(x)&g(x)\\f'(x)&g'(x)\end{pmatrix}=f(x)g'(x)-f'(x)g(x).
$$

The order matters: exchanging $f$ and $g$ reverses the sign. For $n$ sufficiently [differentiable functions](differentiable-function.md), the [Wronskian](wronskian.md) is the [determinant](determinant.md) $\det(f_j^{(i-1)}(x))_{i,j=1}^n$.[NIST Digital Library of Mathematical Functions; §1.13(i), equation 1.13.4 and the following n-argument definition](nist-digital-library-of-mathematical-functions/1-algebraic-and-analytic-methods.md)

The [Wronskian](wronskian.md) measures whether the [vectors](vector.md) $(f(x),f'(x))$ and $(g(x),g'(x))$ supply independent value-and-[derivative](derivative.md) data at that point. For real-valued [functions](function-split.md), its absolute value is the [area](surface-area.md) of the [parallelogram](parallelogram.md) they span. If a constant [linear combination](linear-combination.md) $af+bg$ is zero throughout $I$, then $af'+bg'=0$ too. A nonzero [Wronskian](wronskian.md) at even one point makes this pair of [linear equations](linear-equation.md) invertible and forces $a=b=0$. Thus a nonzero [Wronskian](wronskian.md) somewhere always proves [linear independence](linear-independence.md) of the [functions](function-split.md) on $I$.

For an explicit example, the [exponential functions](exponential-function.md)

$$
y_1(x)=e^{-x},\qquad y_2(x)=e^{2x}
$$

solve the same [homogeneous linear differential equation](homogeneous-linear-differential-equation.md) $y''-y'-2y=0$ on the whole real line: substitution gives $1+1-2=0$ and $4-2-2=0$, respectively. Their [Wronskian](wronskian.md) is

$$
W(y_1,y_2)=e^{-x}(2e^{2x})-(-e^{-x})e^{2x}=3e^x>0.
$$

For the [initial value problem](initial-value-problem.md) $y(0)=2$, $y'(0)=-1$, the [linear combination](linear-combination.md) $y=c_1y_1+c_2y_2$ requires $c_1+c_2=2$ and $-c_1+2c_2=-1$. Hence $c_1=5/3$, $c_2=1/3$, and $y=\frac53e^{-x}+\frac13e^{2x}$. The nonzero [Wronskian](wronskian.md) makes the two [initial conditions](initial-condition.md) independently adjustable.

<a id="image-independent-exponential-functions-supply-independent-initial-data-with-wronskian-equal-to-the-oriented-parallelogram-area"></a>
![](wronskian-exponential-solutions-and-area.png)

**[Figure 1](#image-independent-exponential-functions-supply-independent-initial-data-with-wronskian-equal-to-the-oriented-parallelogram-area). Independent exponential functions supply independent initial data, with Wronskian equal to the oriented parallelogram area**.

The stronger converse requires a common equation. Suppose $y_1,y_2$ solve $y''+p(x)y'+q(x)y=0$ with [continuous functions](continuous-function.md) $p,q$ on one [interval](interval-mathematics.md) $I$. Then the [functions](function-split.md) are [linearly independent](linear-independence.md) if and only if their [Wronskian](wronskian.md) is nonzero at one point, equivalently at every point. If $W(x_0)=0$, choose constants $a,b$, not both zero, making $z=ay_1+by_2$ satisfy $z(x_0)=z'(x_0)=0$. The [superposition principle](superposition-principle.md) makes $z$ a [solution of a differential equation](solution-of-a-differential-equation.md) for the same equation, and the [uniqueness theorem for ordinary differential equations](uniqueness-theorem-for-ordinary-differential-equations.md) forces $z$ to be identically zero. This proves [linear dependence](linear-dependence.md).[18.03 Supplementary Notes by Haynes Miller; Chapter 15, The Wronskian, printed pp. 72–73: initial-data system (3) and the zero-or-nowhere-zero theorem](18-03-supplementary-notes-by-haynes-miller/the-wronskian.md)

For arbitrary [differentiable functions](differentiable-function.md), an identically zero [Wronskian](wronskian.md) need not imply [linear dependence](linear-dependence.md). Consider, on $I=(-2,2)$,

$$
f(x)=x^4,\qquad g(x)=x|x|^3=\begin{cases}-x^4,&x<0,\\x^4,&x\geq0.\end{cases}
$$

Both [functions](function-split.md) have three continuous [derivatives](derivative.md). On each side of zero, $g$ is a constant multiple of $f$, so $W(f,g)=0$; at zero their values and first [derivatives](derivative.md) are all zero, so the [Wronskian](wronskian.md) is zero there too. Nevertheless $af+bg=0$ evaluated at $x=-1$ gives $a-b=0$, while evaluation at $x=1$ gives $a+b=0$. Hence $a=b=0$: these [functions](function-split.md) are [linearly independent](linear-independence.md) on the whole [interval](interval-mathematics.md). There is no single constant multiplier valid on both sides of the common zero.

<a id="image-an-identically-zero-wronskian-can-coexist-with-linear-independence-when-the-common-regular-equation-hypothesis-is-absent"></a>
![](wronskian-zero-with-independent-functions.png)

**[Figure 2](#image-an-identically-zero-wronskian-can-coexist-with-linear-independence-when-the-common-regular-equation-hypothesis-is-absent). An identically zero Wronskian can coexist with linear independence when the common regular equation hypothesis is absent**.

These [functions](function-split.md) cannot both solve any equation $y''+py'+qy=0$ with [continuous functions](continuous-function.md) $p,q$ throughout $(-2,2)$: even $f$ alone would contradict uniqueness because $f(0)=f'(0)=0$ but $f$ is not identically zero. They do solve the singular equation $x^2y''-3xy'=0$, whose leading coefficient vanishes at zero. Dividing by $x^2$ gives $p=-3/x$ only away from zero; [Abel's identity](abel-s-identity.md) cannot be applied across that point. The example pinpoints why checking the equation and its [interval](interval-mathematics.md) is essential before using a zero [Wronskian](wronskian.md) to infer [linear dependence](linear-dependence.md).

**Table of contents**

- [Abel's identity](abel-s-identity.md)

## ↑ Ancestors (8)

1. [Second-order linear differential equation](second-order-linear-differential-equation.md)
2. [Linear ordinary differential equation](linear-ordinary-differential-equation-split.md)
3. [Ordinary differential equation](ordinary-differential-equation.md)
4. [Differential equation](differential-equation-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (118)

- [Abel's identity](abel-s-identity.md)
- [Airy function](airy-function.md)
- [Airy power-series fundamental pair](airy-power-series-fundamental-pair.md)
- [Apparent regular singular point](apparent-regular-singular-point.md)
- [Associated Legendre differential equation](associated-legendre-differential-equation.md)
- [Boundary-decaying Green kernel for an inverse-square differential operator](boundary-decaying-green-kernel-for-an-inverse-square-differential-operator.md)
- [Bunch-Davies mode normalization in a finite comoving volume](bunch-davies-mode-normalization-in-a-finite-comoving-volume.md)
- [Causal Green function for a repeated-root Euler operator](causal-green-function-for-a-repeated-root-euler-operator.md)
- [Dirichlet Green function for a radial power operator on an interval](dirichlet-green-function-for-a-radial-power-operator-on-an-interval.md)
- [Dirichlet Green kernel for an Euler operator with exponents one and minus four](dirichlet-green-kernel-for-an-euler-operator-with-exponents-one-and-minus-four.md)
- [Dirichlet Helmholtz Green function on an interval](dirichlet-helmholtz-green-function-on-an-interval.md)
- [Dirichlet modified Helmholtz Green function on an interval](dirichlet-modified-helmholtz-green-function-on-an-interval.md)
- [Discrete Wronskian](discrete-wronskian.md)
- [Ermakov-Pinney equation](ermakov-pinney-equation.md)
- [Exact late slope of an exponentially damped oscillator](exact-late-slope-of-an-exponentially-damped-oscillator.md)
- [First correction to a regular singular solution by reduction of order](first-correction-to-a-regular-singular-solution-by-reduction-of-order.md)
- [Green kernel with a vanishing Wronskian at an interior singular point](green-kernel-with-a-vanishing-wronskian-at-an-interior-singular-point.md)
- [Green kernels for a radial dipole Euler equation](green-kernels-for-a-radial-dipole-euler-equation.md)
- [Half-line Green function for the first cylindrical harmonic](half-line-green-function-for-the-first-cylindrical-harmonic.md)
- [KdV Schrodinger spectral problem](kdv-schrodinger-spectral-problem.md)
- [Mészáros equation solution basis](meszaros-equation-solution-basis.md)
- [Neutral Rayleigh-mode dispersion correction](neutral-rayleigh-mode-dispersion-correction.md)
- [Nondegeneracy of one-dimensional bound states](nondegeneracy-of-one-dimensional-bound-states.md)
- [Nonunique Green kernel at a singular endpoint with two vanishing modes](nonunique-green-kernel-at-a-singular-endpoint-with-two-vanishing-modes.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/ia/paper-2/6b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/ib/paper-1/11h/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ia/paper-2/7d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-71/6/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/ia/paper-2/6d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/ib/paper-1/11d/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-64/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-8/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/ia/paper-2/2b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/ia/paper-2/5b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/ib/paper-4/16c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ia/paper-2/2b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ia/paper-2/8b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ia/paper-2/7b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ib/paper-2/15g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ii/paper-1/33a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ii/paper-2/14b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ii/paper-3/8b/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ii/paper-3/8b/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ii/paper-3/8b/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-62/3/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-65/4/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-80/4/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ia/paper-2/6a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ii/paper-3/8c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ib/paper-4/16a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-76/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ia/paper-2/6a/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ia/paper-2/6a/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ia/paper-2/6a/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2011/ia/paper-2/7a/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2011/ia/paper-2/7a/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/ia/paper-2/1a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-76/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-48/4/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/ia/paper-2/7b/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ia/paper-2/6a/a/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ia/paper-2/6a/a/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ia/paper-2/7a/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ia/paper-2/7c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-3/7e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-4/7e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-328/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ii/paper-1/14b/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ii/paper-1/34a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-308/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-336/3/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-2/32c/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ia/paper-2/2a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-308/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ia/paper-2/5c/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ib/paper-3/6d/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-2/34e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ib/paper-1/13b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/ia/paper-2/5c/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-166/3/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2001/paper-1/8/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2002/paper-1/8/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2002/paper-1/8/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2003/paper-1/8/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2004/paper-1/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2006/paper-1/6/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2006/paper-1/8/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2007/paper-1/8/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2008/paper-1/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2009/paper-1/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2010/paper-1/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2011/paper-1/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2012/paper-1/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2013/paper-1/3/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2015/paper-1/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2016/paper-1/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2016/paper-1/8/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2019/paper-1/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2019/paper-1/3/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2019/paper-1/3/d/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2021/paper-1/3/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2022/paper-1/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2022/paper-1/8/b/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2023/paper-1/8/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2024/paper-1/3/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2024/paper-1/8/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2024/paper-1/8/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2025/paper-1/3/b/solution.md)
- [Power substitution for an oscillatory second-order equation](power-substitution-for-an-oscillatory-second-order-equation.md)
- [Radial modified Helmholtz Green function on the half-line](radial-modified-helmholtz-green-function-on-the-half-line.md)
- [Rational multiplicity bound for a linear auxiliary polynomial](rational-multiplicity-bound-for-a-linear-auxiliary-polynomial.md)
- [Reduction of order across a zero of the known solution](reduction-of-order-across-a-zero-of-the-known-solution.md)
- [Repeated-root constant-coefficient differential equation](repeated-root-constant-coefficient-differential-equation.md)
- [Resolvent kernel for Neumann advection-diffusion on an interval](resolvent-kernel-for-neumann-advection-diffusion-on-an-interval.md)
- [Thue-Siegel auxiliary polynomial](thue-siegel-auxiliary-polynomial.md)
- [Variation of parameters](variation-of-parameters.md)
- [Wronskian](wronskian.md)
- [Wronskian of a rational map](wronskian-of-a-rational-map.md)
