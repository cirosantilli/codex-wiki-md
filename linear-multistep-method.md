# Linear multistep method

↑ **Parent:** [Numerical analysis](numerical-analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Linear_multistep_method)

A linear multistep method approximates an ODE using several previous solution and derivative values.

**Table of contents**

- [Reciprocal-root three-step multistep family](#reciprocal-root-three-step-multistep-family)
- [Simpson multistep method](#simpson-multistep-method)
- [First Dahlquist barrier](#first-dahlquist-barrier)
  - [Newton-Cotes multistep methods attaining the first Dahlquist barrier](#newton-cotes-multistep-methods-attaining-the-first-dahlquist-barrier)
  - [Cayley coefficient proof of the first Dahlquist barrier](#cayley-coefficient-proof-of-the-first-dahlquist-barrier)
    - [Coefficient sign lemma for the first Dahlquist barrier](#coefficient-sign-lemma-for-the-first-dahlquist-barrier)
- [Two-step family with a third-order member](#two-step-family-with-a-third-order-member)
- [Adams-Bashforth method](#adams-bashforth-method)
  - [Adams-Bashforth stability for centered diffusion](#adams-bashforth-stability-for-centered-diffusion)
- [Common-factor cancellation defect in a multistep recurrence](#common-factor-cancellation-defect-in-a-multistep-recurrence)
- [Trapezoidal-BDF two-step family](#trapezoidal-bdf-two-step-family)
- [Multiderivative multistep method](#multiderivative-multistep-method)
  - [Symmetric sixth-order two-derivative method](#symmetric-sixth-order-two-derivative-method)
  - [Symmetric two-step two-derivative formula](#symmetric-two-step-two-derivative-formula)
    - [Bounded-root stability set of the symmetric two-derivative formula](#bounded-root-stability-set-of-the-symmetric-two-derivative-formula)
    - [Empty strict decay domain of the symmetric two-derivative formula](#empty-strict-decay-domain-of-the-symmetric-two-derivative-formula)
    - [Negative-real instability of the symmetric two-derivative formula](#negative-real-instability-of-the-symmetric-two-derivative-formula)
  - [A-stable third-order two-step multiderivative method](#a-stable-third-order-two-step-multiderivative-method)
  - [Convergence of a zero-stable multiderivative method](#convergence-of-a-zero-stable-multiderivative-method)
- [Zero-stability](#zero-stability)
  - [Root condition for a multistep method](#root-condition-for-a-multistep-method)
    - [Parasitic amplification root](#parasitic-amplification-root)
      - [Centered two-step discretization of exponential decay](#centered-two-step-discretization-of-exponential-decay)
    - [Root stability of a cubic multistep polynomial](#root-stability-of-a-cubic-multistep-polynomial)
- [Dahlquist equivalence theorem](#dahlquist-equivalence-theorem)
  - [Necessity of the root condition for multistep convergence](#necessity-of-the-root-condition-for-multistep-convergence)
- [Characteristic polynomials of a linear multistep method](#characteristic-polynomials-of-a-linear-multistep-method)
  - [Amplification polynomial of a multistep method](#amplification-polynomial-of-a-multistep-method)
    - [Amplification root](#amplification-root)
    - [Exterior roots of the derivative polynomial bound multistep stability](#exterior-roots-of-the-derivative-polynomial-bound-multistep-stability)
  - [Order conditions for a linear multistep method](#order-conditions-for-a-linear-multistep-method)
    - [Exponential-symbol order criterion for a multistep method](#exponential-symbol-order-criterion-for-a-multistep-method)
- [Adams–Moulton method](#adams-moulton-method)
- [Second Dahlquist barrier](#second-dahlquist-barrier)

## Reciprocal-root three-step multistep family

↑ **Parent:** [Linear multistep method](linear-multistep-method.md)

Take $\sigma(\zeta)=\zeta[(5+\alpha)\zeta^2-(4+8\alpha)\zeta+11-5\alpha]/6$. The [root condition for a multistep method](#root-condition-for-a-multistep-method) holds exactly for $-1<\alpha<1$. Since $\rho'(1)=\sigma(1)=2(1-\alpha)$, these and only these parameters give a convergent method. Its [exponential-symbol order criterion for a multistep method](#exponential-symbol-order-criterion-for-a-multistep-method) has defect $-(\alpha+5)z^4/12+O(z^5)$, giving formal order three except at $\alpha=-5$, where the first defect is $z^5/10$. None of the convergent family is [A-stable](numerical-analysis.md#a-stability): for a parasitic root $r=\alpha+i\sqrt{1-\alpha^2}$, perturbation of $\rho(r(z))-z\sigma(r(z))=0$ gives $\operatorname{Re}[r'(0)/r]=(\alpha-1)/12<0$. A small negative real $z$ therefore moves it outside the unit disk. At $\alpha=1$, cancellation would remove a double unit root, but the original recurrence retains that unstable parasitic behavior; it is not legitimately replaced by the reduced Backward Euler recurrence for arbitrary starting values.

## Simpson multistep method

↑ **Parent:** [Linear multistep method](linear-multistep-method.md)

Integrating a quadratic interpolant of the derivative over two steps gives this [linear multistep method](linear-multistep-method.md), which has order four. Its [local truncation error](numerical-analysis.md#local-truncation-error) is $-h^5y^{(5)}(t_{n+1})/90+O(h^7)$ and its [zero-stability](#zero-stability) polynomial is $\rho(\zeta)=\zeta^2-1$, with simple roots $1,-1$. The [Dahlquist equivalence theorem](#dahlquist-equivalence-theorem) therefore gives fourth-order convergence with sufficiently accurate starts. This attains the even two-step [first Dahlquist barrier](#first-dahlquist-barrier). Its undamped parasitic zero-step mode need not have favorable long-time [absolute stability](numerical-analysis.md#linear-stability-domain); finite-time convergence and stiff damping are separate requirements.

## First Dahlquist barrier

↑ **Parent:** [Linear multistep method](linear-multistep-method.md)

For a consistent [zero-stable](#zero-stability) real linear $k$-step method with constant coefficients and only first-derivative evaluations, the attainable order is at most $k+1$ for odd $k$ and $k+2$ for even $k$. For an explicit method the bound is $k$. These are order barriers under the [root condition for a multistep method](#root-condition-for-a-multistep-method), not bounds on multiderivative methods or on arbitrary variable-step formulations. The [Second Dahlquist barrier](#second-dahlquist-barrier) adds the stronger bound of order two for irreducible [A-stable](numerical-analysis.md#a-stability) methods.

### Newton-Cotes multistep methods attaining the first Dahlquist barrier

↑ **Parent:** [First Dahlquist barrier](#first-dahlquist-barrier)

Using [Newton-Cotes closed quadrature](numerical-integration.md#newton-cotes-closed-quadrature) for the integrated derivative yields the displayed [linear multistep method](linear-multistep-method.md). Its first [characteristic polynomial](linear-operator-theory.md#characteristic-polynomial) is $\rho(z)=z^s-1$, whose unit-circle roots are all simple, proving [zero-stability](#zero-stability). Quadrature exactness gives order $s+1$ for odd $s$ and at least $s+2$ for even $s$. The [first Dahlquist barrier](#first-dahlquist-barrier) gives equality, while the [Dahlquist equivalence theorem](#dahlquist-equivalence-theorem) gives convergence with consistent starts. These are finite-time convergence statements, not claims of [A-stability](numerical-analysis.md#a-stability).

### Cayley coefficient proof of the first Dahlquist barrier

↑ **Parent:** [First Dahlquist barrier](#first-dahlquist-barrier)

For a real consistent [zero-stable](#zero-stability) [linear multistep method](linear-multistep-method.md), transform its first [characteristic polynomial](linear-operator-theory.md#characteristic-polynomial) by $z=(1+x)/(1-x)$ to $(1-x)^s\rho(z)=xP(x)$. The [root condition for a multistep method](#root-condition-for-a-multistep-method) puts all finite roots of $P$ in the closed left half-plane; real linear factors and conjugate quadratic factors consequently give nonnegative coefficients, after choosing $P(0)>0$. The order criterion requires a [polynomial](polynomial.md) of degree at most $s$ to agree through degree $p-1$ with $P(x)x/(2\operatorname{arctanh}x)$. The latter quotient has strictly negative nonconstant even coefficients. Its first even coefficient beyond degree $s$ includes a strictly negative multiple of $P(0)$ and cannot vanish. This gives the stated bound.

#### Coefficient sign lemma for the first Dahlquist barrier

↑ **Parent:** [Cayley coefficient proof of the first Dahlquist barrier](#cayley-coefficient-proof-of-the-first-dahlquist-barrier)

Write $F(x)=\int_0^1(1+x)^t(1-x)^{1-t}\,dt=x/\operatorname{arctanh}x$. Pairing $t$ and $1-t$ after differentiating twice gives

$$
F''(x)=-4\int_0^1t(1-t)(1-x^2)^{-3/2}\cosh[(2t-1)\operatorname{arctanh}x]\,dt.
$$

The [power series](sequence-and-series.md#power-series) of $(1-x^2)^{-3/2}$ has strictly positive even coefficients, and the other factor has nonnegative even coefficients. Thus every even coefficient of $F''$ is negative. Since $F$ is even with $F(0)=1$, the displayed sign pattern follows. This supplies a short positivity argument for the [first Dahlquist barrier](#first-dahlquist-barrier).

## Two-step family with a third-order member

↑ **Parent:** [Linear multistep method](linear-multistep-method.md)

The [exponential-symbol order criterion for a multistep method](#exponential-symbol-order-criterion-for-a-multistep-method) gives leading defect $-(1+5a)z^3/12$, so the family has order two except at $a=-1/5$, where it has order three. The [root condition for a multistep method](#root-condition-for-a-multistep-method) holds exactly for $-1\leq a<1$, and the convergent [A-stable](numerical-analysis.md#a-stability) members are exactly $0\leq a<1$. At $a=0$ it reduces to the [trapezoidal rule](runge-kutta-method.md#trapezoidal-rule) after removal of a zero root. At $a=1$ a repeated root one destroys [convergence of a numerical method](numerical-analysis.md#convergence-of-a-numerical-method) of the original recurrence despite a common [polynomial](polynomial.md) factor and a formally vanishing second-order residual.

## Adams-Bashforth method

↑ **Parent:** [Linear multistep method](linear-multistep-method.md)

An explicit [linear multistep method](linear-multistep-method.md) that integrates a polynomial extrapolation of the past derivative values. The displayed two-step member is second order in time: the linear interpolant through $f_{n-1},f_n$, integrated over the next step, gives coefficients $3/2,-1/2$. For a spatially discretized partial differential equation, the spatial error must also be included in the total local defect.

### Adams-Bashforth stability for centered diffusion

↑ **Parent:** [Adams-Bashforth method](#adams-bashforth-method)

For centered-space diffusion, a [Fourier mode](fourier-analysis.md#fourier-mode) gives $z^2-(1-3a/2)z-a/2=0$, with $a=4\mu\sin^2(\theta/2)$. For $a>0$ the roots have opposite signs, the positive root lies in $(0,1)$, and the negative root lies in $[-1,0)$ exactly when $P(-1)=2-2a\geq0$. At $a=0,1$ the unit-modulus roots are simple. Hence the [root condition for a multistep method](#root-condition-for-a-multistep-method) holds for every Fourier frequency exactly when $\mu\leq1/4$. Under fixed $\mu$, the unscaled one-step defect is $-\Delta t^2u_{xxxx}/(12\mu)+O(\Delta t^3)$; dividing by the step changes its order to $O(\Delta t)$.

## Common-factor cancellation defect in a multistep recurrence

↑ **Parent:** [Linear multistep method](linear-multistep-method.md)

Canceling a common factor of the characteristic polynomials changes the allowed starting relations and can remove a parasitic mode rather than prove stability of the original recurrence. For example $\rho=(\zeta-1)^2$ and $\sigma=(\zeta^2-1)/2$ fail [zero-stability](#zero-stability). On $y'=0$, the original recurrence admits $y_n=y_0+n(y_1-y_0)$; starting perturbations $y_1-y_0=\sqrt h$ vanish but give divergent error at fixed positive time. The canceled one-step recurrence excludes these data, so its stability cannot be assigned to the original scheme.

## Trapezoidal-BDF two-step family

↑ **Parent:** [Linear multistep method](linear-multistep-method.md)

This real-parameter [linear multistep method](linear-multistep-method.md) has formal order two except at the degenerate value $\alpha=2$, where its local symbol vanishes to fourth degree. The zero-stability roots are $1$ and $\alpha-1$, so it is convergent exactly for $0\leq\alpha<2$. Every convergent member is [A-stable](numerical-analysis.md#a-stability): the [boundary-locus test for multistep A-stability](numerical-analysis.md#boundary-locus-test-for-multistep-a-stability) gives nonnegative real part $\alpha(2-\alpha)(1-\cos\theta)^2/(2|\sigma(e^{i\theta})|^2)$, with no unit-circle denominator zero for $0<\alpha<2$. At $\alpha=0$ the two interlaced sequences obey a trapezoidal step of length $2h$. At $\alpha=4/3$ it is the [BDF2 method](numerical-analysis.md#second-order-backward-differentiation-formula). The endpoint two fails the [root condition for a multistep method](#root-condition-for-a-multistep-method) even though canceling a common polynomial factor resembles the [trapezoidal rule](runge-kutta-method.md#trapezoidal-rule).

## Multiderivative multistep method

↑ **Parent:** [Linear multistep method](linear-multistep-method.md)

A multiderivative multistep method uses higher time derivatives as well as values and first derivatives from several time levels. For an autonomous [ordinary differential equation](differential-equation.md#ordinary-differential-equation) $y'=f(y)$, the second time derivative is $y''=f'(y)f(y)$ by the [chain rule](calculus.md#chain-rule). Its [local truncation error](numerical-analysis.md#local-truncation-error) must include the higher-derivative terms. Consequently the usual second-order barrier for [A-stable](numerical-analysis.md#a-stability) [linear multistep methods](linear-multistep-method.md), which only use first derivatives, does not apply.

### Symmetric sixth-order two-derivative method

↑ **Parent:** [Multiderivative multistep method](#multiderivative-multistep-method)

For $y'=f(y)$ and $g=f'f$, inserting a smooth exact solution into the displayed recurrence gives defect $h^7y^{(7)}(t_n)/4725+O(h^9)$. This follows by expanding $2\sinh z-(14/15)z\cosh z-(16/15)z+(2/15)z^2\sinh z$. The terms through $z^6$ vanish and the $z^7$ coefficient is nonzero. Its zero-step polynomial is $\zeta^2-1$, whose roots are simple and of unit modulus. Thus it is [zero-stable](#zero-stability) and has order six, provided starting values and derivative evaluations have corresponding accuracy.

### Symmetric two-step two-derivative formula

↑ **Parent:** [Multiderivative multistep method](#multiderivative-multistep-method)

For the [multiderivative multistep method](#multiderivative-multistep-method) $y_{n+1}-\alpha h f_{n+1}+\beta h^2g_{n+1}=\gamma h f_n+y_{n-1}+\alpha h f_{n-1}+\beta h^2g_{n-1}$, with $g=f'f$, centered expansion gives defect coefficients $2-2\alpha-\gamma$, $1/3-\alpha+2\beta$, and $1/60-\alpha/12+\beta/3$ at powers $h,h^3,h^5$. Their simultaneous vanishing gives the displayed parameters. The next coefficient is $1/4725$ at $h^7$, so the formal order is six. Reflection symmetry removes every even defect power. The method satisfies fifth-order conditions but cannot have exact order five.

#### Bounded-root stability set of the symmetric two-derivative formula

↑ **Parent:** [Symmetric two-step two-derivative formula](#symmetric-two-step-two-derivative-formula)

For the [symmetric two-step two-derivative formula](#symmetric-two-step-two-derivative-formula), the closed-disk [root condition for a multistep method](#root-condition-for-a-multistep-method) fails off the imaginary axis. Positive real part makes the product of root moduli exceed one; negative real part fails the [complex quadratic Schur criterion](numerical-analysis.md#complex-quadratic-schur-criterion), as in the [empty strict decay domain of the symmetric two-derivative formula](#empty-strict-decay-domain-of-the-symmetric-two-derivative-formula) proof. On $z=iy$, write $D=15-y^2-7iy=|D|e^{i\delta}$ and set $\xi=i e^{-i\delta}\eta$. The [amplification polynomial](#amplification-polynomial-of-a-multistep-method) becomes $\eta^2-16y\eta/|D|+1=0$. Its two roots are distinct and on the [unit circle](complex-analysis.md#complex-unit-circle) exactly when $|16y/|D||<2$, or $y^4-45y^2+225>0$. Thus the bounded-root set consists of the imaginary intervals $|y|<\sqrt{(45-15\sqrt5)/2}$ and $|y|>\sqrt{(45+15\sqrt5)/2}$, including $y=0$ and excluding the double-root endpoints. In particular, the set is unbounded. Unit-modulus oscillations are bounded but do not tend to zero.

#### Empty strict decay domain of the symmetric two-derivative formula

↑ **Parent:** [Symmetric two-step two-derivative formula](#symmetric-two-step-two-derivative-formula)

On the [Dahlquist test equation](numerical-analysis.md#dahlquist-test-equation), write the [amplification polynomial](#amplification-polynomial-of-a-multistep-method) as $D\xi^2-16z\xi-A$, where $D=z^2-7z+15$ and $A=z^2+7z+15$. The identity $|A|^2-|D|^2=28\operatorname{Re}z(|z|^2+15)$ shows that both [roots of a polynomial](polynomial.md#root-of-a-polynomial) can lie inside the open [unit disk](euclidean-geometry.md#unit-disk) only if $\operatorname{Re}z<0$. But the [complex quadratic Schur criterion](numerical-analysis.md#complex-quadratic-schur-criterion) would then require $32|\operatorname{Re}z|(|z|^2+15)<28|\operatorname{Re}z|(|z|^2+15)$, which is impossible. Thus the [strict linear stability domain](numerical-analysis.md#strict-linear-stability-domain) is empty. This concerns robust damping of all modes, rather than convergence on fixed time intervals or the [bounded-root stability set of the symmetric two-derivative formula](#bounded-root-stability-set-of-the-symmetric-two-derivative-formula).

#### Negative-real instability of the symmetric two-derivative formula

↑ **Parent:** [Symmetric two-step two-derivative formula](#symmetric-two-step-two-derivative-formula)

On the [Dahlquist test equation](numerical-analysis.md#dahlquist-test-equation), the [symmetric two-step two-derivative formula](#symmetric-two-step-two-derivative-formula) has amplification polynomial $F_z(w)=(z^2-7z+15)w^2-16zw-(z^2+7z+15)$. For every real $z<0$, its leading coefficient is positive and $F_z(-1)=2z<0$, whereas $F_z(w)\to+\infty$ as $w\to-\infty$. The [intermediate value theorem](calculus.md#intermediate-value-theorem) therefore gives a real root below minus one. Thus the method is not [A-stable](numerical-analysis.md#a-stability), without any appeal to a multistep order barrier.

### A-stable third-order two-step multiderivative method

↑ **Parent:** [Multiderivative multistep method](#multiderivative-multistep-method)

The endpoint expansion of this [multiderivative multistep method](#multiderivative-multistep-method) has unscaled defect $h^4y^{(4)}/3+O(h^5)$ and [zero-stability](#zero-stability) roots $1,1/7$, giving third-order convergence with suitably accurate starting values. On the [Dahlquist test equation](numerical-analysis.md#dahlquist-test-equation) its amplification roots obey $(7-6z+2z^2)\zeta^2-8\zeta+1=0$. The [complex quadratic Schur criterion](numerical-analysis.md#complex-quadratic-schur-criterion) puts both roots in the open unit disk for $\operatorname{Re}z<0$, and only the simple root one reaches the boundary at $z=0$. Thus it is [A-stable](numerical-analysis.md#a-stability); its higher derivative places it outside the hypotheses of the [Second Dahlquist barrier](#second-dahlquist-barrier).

### Convergence of a zero-stable multiderivative method

↑ **Parent:** [Multiderivative multistep method](#multiderivative-multistep-method)

For a fixed-step [multiderivative multistep method](#multiderivative-multistep-method), the ordinary [zero-stability](#zero-stability) root condition still controls propagation of the starting errors when all derivative evaluation maps are uniformly [Lipschitz continuous](real-analysis.md#lipschitz-continuity) on the relevant bounded region. A local defect $O(h^{p+1})$ then yields global error $O(h^p)$ over a fixed time interval, provided the starting errors are $O(h^p)$ and the implicit updates use the nearby solution branch.

For example, writing the numerical error equation as $\rho(E)e_n=hF_h(e_{n+s})+d_n$, with $F_h$ uniformly [Lipschitz continuous](real-analysis.md#lipschitz-continuity), a bounded impulse response for the [root condition for a multistep method](#root-condition-for-a-multistep-method) gives

$$
\max_{j\leq n}\|e_j\|
\leq C\left(\max_{j<s}\|e_j\|+\sum_{j<n}\|d_j\|\right)
+Ch\sum_{j\leq n}\max_{i\leq j}\|e_i\|.
$$

Absorbing the last current-step term for small $h$ and applying the [discrete Gronwall inequality](probability-and-statistics.md#discrete-gronwall-inequality) gives the stated order. The higher derivatives enter through $F_h$, whose bound stays uniform as $h\to0$.

## Zero-stability

↑ **Parent:** [Linear multistep method](linear-multistep-method.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Zero-stability)

Zero-stability requires the roots of the first characteristic polynomial to lie in the closed unit disc, with unit-modulus roots simple.

### Root condition for a multistep method

↑ **Parent:** [Zero-stability](#zero-stability)

The root condition is the polynomial criterion equivalent to zero-stability for a linear multistep method.

#### Parasitic amplification root

↑ **Parent:** [Root condition for a multistep method](#root-condition-for-a-multistep-method)

An amplification root of a [multistep method](linear-multistep-method.md) is parasitic when it represents an additional numerical mode rather than the principal mode approximating the exact differential-equation flow. For a consistent method the principal root starts at one as the step tends to zero, while other roots can start elsewhere. A simple parasitic root on the unit circle is compatible with [zero-stability](#zero-stability), but its motion outside the circle for a negative test parameter can destroy [absolute stability](numerical-analysis.md#linear-stability-domain). Fixed-time convergence and all-time damping must be distinguished.

##### Centered two-step discretization of exponential decay

↑ **Parent:** [Parasitic amplification root](#parasitic-amplification-root)

Replacing the derivative in $x'=-Kx$ by a [central finite difference](finite-difference.md#central-finite-difference) gives $x_{n+1}+2Khx_n-x_{n-1}=0$. Its principal root is $\rho_+=e^{-\operatorname{arsinh}(Kh)}$, while the [parasitic amplification root](#parasitic-amplification-root) is $\rho_-=-e^{\operatorname{arsinh}(Kh)}$. On a fixed time interval, $A_h\rho_+^n+B_h\rho_-^n$ converges uniformly to $Ce^{-Kt}$ exactly when $A_h\to C$ and $B_h\to0$. A fixed nonzero parasitic amplitude alternates between two incompatible limits, but a vanishing starting error can converge despite the root's modulus exceeding one. This distinguishes fixed-time [numerical convergence](numerical-analysis.md#convergence-of-a-numerical-method) from long-time [absolute stability](numerical-analysis.md#linear-stability-domain).

#### Root stability of a cubic multistep polynomial

↑ **Parent:** [Root condition for a multistep method](#root-condition-for-a-multistep-method)

The polynomial $\rho(w)=(w-1)(w^2+w+a)$ satisfies the [root condition for a multistep method](#root-condition-for-a-multistep-method) exactly for $0\leq a\leq1$. For $a<0$ a root is below $-1$; for $a>1$ the quadratic root product forces a root outside the unit disc. The endpoints have simple unit-modulus roots, and the repeated root at $a=1/4$ is strictly inside. A consistent method with this polynomial is convergent throughout the closed interval.

## Dahlquist equivalence theorem

↑ **Parent:** [Linear multistep method](linear-multistep-method.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Dahlquist_equivalence_theorem)

A consistent linear multistep method is convergent exactly when it is zero-stable.

### Necessity of the root condition for multistep convergence

↑ **Parent:** [Dahlquist equivalence theorem](#dahlquist-equivalence-theorem)

For a [linear multistep method](linear-multistep-method.md), convergence for every set of consistent starting values requires the [root condition for a multistep method](#root-condition-for-a-multistep-method). Apply the recurrence to $y'=0$ over $N$ steps. A root $\xi$ with $|\xi|>1$ gives the error mode $e_n=|\xi|^{-N}\xi^n$: its fixed-index starting errors vanish as $N\to\infty$, but $|e_N|=1$. A unit-modulus root of multiplicity $m\geq2$ instead gives $e_n=N^{-(m-1)}n^{m-1}\xi^n$, with the same failure. Repeated roots inside the unit disk are harmless because their polynomial growth is dominated by exponential decay.

## Characteristic polynomials of a linear multistep method

↑ **Parent:** [Linear multistep method](linear-multistep-method.md)

For $\sum_{j=0}^s\alpha_jy_{n+j}=h\sum_{j=0}^s\beta_jf_{n+j}$, the characteristic polynomials are $\rho(\zeta)=\sum_j\alpha_j\zeta^j$ and $\sigma(\zeta)=\sum_j\beta_j\zeta^j$. Applied to $y'=\lambda y$, the amplification roots solve $\rho(\zeta)-h\lambda\sigma(\zeta)=0$.

### Amplification polynomial of a multistep method

↑ **Parent:** [Characteristic polynomials of a linear multistep method](#characteristic-polynomials-of-a-linear-multistep-method)

Applying a [linear multistep method](linear-multistep-method.md) to the [Dahlquist test equation](numerical-analysis.md#dahlquist-test-equation) with $z=h\lambda$ produces a constant-coefficient recurrence whose modes satisfy $P_z(w)=0$. [Absolute stability](numerical-analysis.md#linear-stability-domain) requires the resulting [roots of a polynomial](polynomial.md#root-of-a-polynomial) to lie in the unit disk, with unit-modulus roots simple. Thus multistep stability depends on every recurrence mode, rather than a single one-step [stability function](numerical-analysis.md#stability-function).

#### Amplification root

↑ **Parent:** [Amplification polynomial of a multistep method](#amplification-polynomial-of-a-multistep-method)

An amplification root is a [root of a polynomial](polynomial.md#root-of-a-polynomial) governing a geometric mode $y_n=\xi^n$ of a numerical recurrence on the [Dahlquist test equation](numerical-analysis.md#dahlquist-test-equation). Its [modulus](complex-analysis.md#modulus) measures damping or growth per step. A repeated root produces additional modes such as $n\xi^n$; therefore a [unit-circle root](polynomial.md#unit-circle-root) can be permitted by a bounded-root condition only when it is simple. The principal root approximates $e^z$ near zero, while additional roots can describe [parasitic amplification roots](#parasitic-amplification-root).

#### Exterior roots of the derivative polynomial bound multistep stability

↑ **Parent:** [Amplification polynomial of a multistep method](#amplification-polynomial-of-a-multistep-method)

If the derivative [characteristic polynomial](linear-operator-theory.md#characteristic-polynomial) $\sigma$ of a [linear multistep method](linear-multistep-method.md) has a simple root outside the [unit disk](euclidean-geometry.md#unit-disk) and keeps its degree in the limit, then its [absolute stability](numerical-analysis.md#linear-stability-domain) region is bounded. Otherwise a stable sequence with $|z|\to\infty$ would give amplification polynomials $\sigma-\rho/z$ tending coefficientwise to $\sigma$. A root near the exterior root would persist by continuity, contradicting the [root condition for a multistep method](#root-condition-for-a-multistep-method). This argument excludes stability at every sufficiently large complex $z$, not only along the negative real axis.

### Order conditions for a linear multistep method

↑ **Parent:** [Characteristic polynomials of a linear multistep method](#characteristic-polynomials-of-a-linear-multistep-method)

A linear multistep method has order $p$ exactly when

$$
\sum_j\alpha_jj^q=q\sum_j\beta_jj^{q-1}
$$

for $0\leq q\leq p$, with the right side interpreted as zero for $q=0$, and the identity first fails at $q=p+1$.

#### Exponential-symbol order criterion for a multistep method

↑ **Parent:** [Order conditions for a linear multistep method](#order-conditions-for-a-linear-multistep-method)

The [Taylor expansion](calculus.md#taylor-expansion) of the exact-solution residual for a [linear multistep method](linear-multistep-method.md) has the same coefficient sequence as

$$
\rho(e^z)-z\sigma(e^z).
$$

Vanishing through degree $p$ is therefore equivalent to order at least $p$. Exact order $p$ additionally requires a nonzero coefficient at degree $p+1$. This symbol conveniently collects all polynomial consistency and order conditions.

<h2 id="adams-moulton-method">Adams–Moulton method</h2>

↑ **Parent:** [Linear multistep method](linear-multistep-method.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Adams–Moulton_method)

An Adams–Moulton method is an implicit [linear multistep method](linear-multistep-method.md) obtained by integrating an interpolation polynomial for the vector field that includes the new time level.

## Second Dahlquist barrier

↑ **Parent:** [Linear multistep method](linear-multistep-method.md)

An irreducible A-stable linear multistep method has order at most two.

This is an order restriction for an [A-stable](numerical-analysis.md#a-stability) [linear multistep method](linear-multistep-method.md).

## ↑ Ancestors (5)

1. [Numerical analysis](numerical-analysis.md)
2. [Analysis](analysis.md)
3. [Area of mathematics](mathematics.md#area-of-mathematics)
4. [Mathematics](mathematics.md)
5. [Codex Wiki](README.md)

## ← Incoming links (43)

- [Adams-Bashforth method](#adams-bashforth-method)
- [Adams–Moulton method](#adams-moulton-method)
- [Amplification polynomial of a multistep method](#amplification-polynomial-of-a-multistep-method)
- [Boundary-locus test for multistep A-stability](numerical-analysis.md#boundary-locus-test-for-multistep-a-stability)
- [Cayley coefficient proof of the first Dahlquist barrier](#cayley-coefficient-proof-of-the-first-dahlquist-barrier)
- [Convergence of a numerical method](numerical-analysis.md#convergence-of-a-numerical-method)
- [Explicit multistep methods cannot be A-stable](numerical-analysis.md#explicit-multistep-methods-cannot-be-a-stable)
- [Exponential-symbol order criterion for a multistep method](#exponential-symbol-order-criterion-for-a-multistep-method)
- [Exterior roots of the derivative polynomial bound multistep stability](#exterior-roots-of-the-derivative-polynomial-bound-multistep-stability)
- [Implicit time-stepping method](numerical-analysis.md#implicit-time-stepping-method)
- [Multiderivative multistep method](#multiderivative-multistep-method)
- [Necessity of the root condition for multistep convergence](#necessity-of-the-root-condition-for-multistep-convergence)
- [Newton-Cotes multistep methods attaining the first Dahlquist barrier](#newton-cotes-multistep-methods-attaining-the-first-dahlquist-barrier)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-57.md#7/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-60.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-69.md#5/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-69.md#6/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-69.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-68.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-80.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-72.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-72.md#7/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-63.md#1/2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-63.md#6/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-63.md#7/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/ib/paper-1.md#6c/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-66.md#2/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-66.md#6/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-68.md#7/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ib/paper-1.md#18d/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ib/paper-1.md#18d/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ib/paper-1.md#18d/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-341.md#2/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-341.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ib/paper-1.md#18c/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ib/paper-2.md#17c/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ib/paper-2.md#17c/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-341.md#6/solution)
- [Principal-root obstruction to A-stability](numerical-analysis.md#principal-root-obstruction-to-a-stability)
- [Second Dahlquist barrier](#second-dahlquist-barrier)
- [Second-order backward differentiation formula](numerical-analysis.md#second-order-backward-differentiation-formula)
- [Simpson multistep method](#simpson-multistep-method)
- [Trapezoidal-BDF two-step family](#trapezoidal-bdf-two-step-family)
