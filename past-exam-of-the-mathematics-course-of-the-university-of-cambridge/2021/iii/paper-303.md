# Paper 303

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2021/paper_303.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2021/paper_303.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
  - [d](#1/d)
    - [Solution](#1/d/solution)
  - [e](#1/e)
    - [i](#1/e/i)
      - [Solution](#1/e/i/solution)
    - [ii](#1/e/ii)
      - [Solution](#1/e/ii/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
  - [d](#2/d)
    - [Solution](#2/d/solution)
  - [e](#2/e)
    - [Solution](#2/e/solution)
  - [f](#2/f)
    - [i](#2/f/i)
      - [Solution](#2/f/i/solution)
    - [ii](#2/f/ii)
      - [Solution](#2/f/ii/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
  - [d](#3/d)
    - [Solution](#3/d/solution)
  - [e](#3/e)
    - [Solution](#3/e/solution)
  - [f](#3/f)
    - [Solution](#3/f/solution)

## 1

↑ **Parent:** [Paper 303](paper-303.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

The [equilibrium magnetization](../../../critical-phenomenon.md#equilibrium-magnetization) is a [global minimum](../../../analysis.md#global-minimum) of the [Landau free energy](../../../critical-phenomenon.md#landau-free-energy). Its candidates are the [stationary points](../../../calculus-of-variations.md#stationary-point)

$$
0=f'(m)=2m\left(a_2+2a_4m^2+3a_6m^4\right).
$$

Thus $m=0$, or $x=m^2\geq0$ is a nonnegative root of

$$
3a_6x^2+2a_4x+a_2=0.
$$

One retains candidates with nonnegative curvature $f''(m)$ and compares their free energies; the candidate with the smallest value is the equilibrium state. Equal global minima describe [phase coexistence](../../../critical-phenomenon.md#phase-coexistence).

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

At the [first-order phase transition](../../../thermodynamics.md#first-order-phase-transition), the central minimum $m=0$ and two nonzero minima $m=\pm m_0$ are degenerate, with barriers between them. Writing $x=m_0^2>0$, stationarity and equal free energies give

$$
a_2+2a_4x+3a_6x^2=0,
\qquad
a_2+a_4x+a_6x^2=0.
$$

Their difference gives $a_4x+2a_6x^2=0$, so

$$
m_0^2=-\frac{a_4}{2a_6},
\qquad
\boxed{a_2=\frac{a_4^2}{4a_6}}.
$$

The magnitude of the [magnetization](../../../electromagnetism.md#magnetization) therefore jumps from zero to

$$
\boxed{|m_0|=\sqrt{-\frac{a_4}{2a_6}}}.
$$

The two possible signs are related by the model's spin-reversal symmetry.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

At the [tricritical point](../../../critical-phenomenon.md#tricritical-point), $a_4=0$ and the zero-field [Landau free energy](../../../critical-phenomenon.md#landau-free-energy) is $f=a_2m^2+a_6m^6$. Below $T_c$, minimization gives

$$
m^4=-\frac{a_2}{3a_6}.
$$

Since $a_2\sim T-T_c$, the [order-parameter critical exponent](../../../critical-phenomenon.md#order-parameter-critical-exponent) is

$$
\boxed{\beta=\frac14}.
$$

At this minimum, $f_{\rm sing}=a_2m^2+a_6m^6$ is proportional to $-|T-T_c|^{3/2}$. Comparing this with $f_{\rm sing}\sim|T-T_c|^{2-\alpha}$ gives the [heat-capacity critical exponent](../../../critical-phenomenon.md#heat-capacity-critical-exponent)

$$
\boxed{\alpha=\frac12}.
$$

After adding the magnetic contribution $-Bm$, the inverse zero-field [magnetic susceptibility](../../../statistical-physics.md#magnetic-susceptibility) is the curvature $f''(m)$. Above $T_c$ it is $2a_2$, while below $T_c$ it is $-8a_2$, so $\chi\sim|T-T_c|^{-1}$ and the [magnetic-susceptibility critical exponent](../../../critical-phenomenon.md#magnetic-susceptibility-critical-exponent) is

$$
\boxed{\gamma=1}.
$$

Finally, exactly at $T_c$ the equation of state is $B=6a_6m^5$. Hence $m\sim B^{1/5}$ and the [critical-isotherm exponent](../../../critical-phenomenon.md#critical-isotherm-exponent) is

$$
\boxed{\delta=5}.
$$

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

The [mean-field approximation](../../../critical-phenomenon.md#mean-field-approximation) suppresses correlated order-parameter fluctuations. Near a [continuous phase transition](../../../critical-phenomenon.md#continuous-phase-transition), the [correlation length](../../../critical-phenomenon.md#correlation-length) diverges and long-wavelength fluctuations become increasingly important. The [Ginzburg criterion](../../../critical-phenomenon.md#ginzburg-criterion) therefore fails in sufficiently low dimension, and the interacting [renormalization-group fixed point](../../../critical-phenomenon.md#renormalization-group-fixed-point) changes the mean-field exponents. For the tricritical $m^6$ theory the [upper critical dimension](../../../critical-phenomenon.md#upper-critical-dimension) is three: below $d=3$ the exponents are generally non-mean-field, while at $d=3$ one expects logarithmic corrections to mean-field scaling.

<h3 id="1/e">e</h3>

↑ **Parent:** [1](#1)

<h4 id="1/e/i">i</h4>

↑ **Parent:** [E](#1/e)

<h5 id="1/e/i/solution">Solution</h5>

↑ **Parent:** [I](#1/e/i)

This is the [Blume–Capel model](../../../statistical-physics.md#blume-capel-model). In the [mean-field approximation](../../../critical-phenomenon.md#mean-field-approximation), write $m=\langle\sigma_i\rangle$ and replace

$$
\sigma_i\sigma_j\simeq m\sigma_i+m\sigma_j-m^2.
$$

Because every site has [coordination number](../../../statistical-physics.md#coordination-number-of-a-lattice) $q$, the resulting energy is

$$
E_{\rm MF}=\frac12NJqm^2+\sum_i\left[g\sigma_i^2-(Jqm+B)\sigma_i\right].
$$

The one-site [partition function](../../../statistical-physics.md#canonical-partition-function) is therefore

$$
Z_1=\sum_{\sigma=-1}^{1}e^{-\beta[g\sigma^2-(Jqm+B)\sigma]}
=1+2e^{-\beta g}\cosh\!\left(\beta(Jqm+B)\right).
$$

With $\kappa=e^{-\beta g}$, the mean-field partition function is $Z_{\rm MF}=e^{-\beta NJqm^2/2}Z_1^N$. Taking $F=-T\log Z_{\rm MF}$ gives

$$
\boxed{\frac FN=\frac12Jqm^2-T\log\!\left[1+2\kappa\cosh\!\left(\beta(Jqm+B)\right)\right]}.
$$

<h4 id="1/e/ii">ii</h4>

↑ **Parent:** [E](#1/e)

<h5 id="1/e/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/e/ii)

Set $B=0$, $h=\beta Jqm$, and $A=1+2\kappa$. The required [power series](../../../real-analysis.md#power-series) is obtained from

$$
1+2\kappa\cosh h=A+\kappa h^2+\frac{\kappa}{12}h^4+\frac{\kappa}{360}h^6+O(h^8).
$$

The quadratic Landau coefficient is

$$
a_2=\frac{Jq}{2}-\frac{\kappa(Jq)^2}{T(1+2\kappa)}.
$$

Its vanishing gives the line of continuous transitions

$$
T=\frac{2\kappa Jq}{1+2\kappa}.
$$

The quartic coefficient is

$$
a_4=-T(\beta Jq)^4\left[\frac{\kappa}{12A}-\frac{\kappa^2}{2A^2}\right].
$$

At a [tricritical point](../../../critical-phenomenon.md#tricritical-point), both $a_2$ and $a_4$ vanish. Since $A=1+2\kappa$, the condition $a_4=0$ gives $A=6\kappa$ and hence $\kappa=1/4$. Substitution into the critical line yields

$$
\boxed{\kappa_{\rm tri}=\frac14,
\qquad T_{\rm tri}=\frac{Jq}{3}}.
$$

The sextic coefficient is positive there, so the sixth-order term stabilizes the free energy. Equivalently, $g_{\rm tri}=T_{\rm tri}\log4$.

## 2

↑ **Parent:** [Paper 303](paper-303.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

A momentum-shell [renormalization group](../../../critical-phenomenon.md#renormalization-group) transformation consists of three steps. First split $\phi=\phi_-+\phi_+$ into slow modes with $|k|<\Lambda/\zeta$ and fast modes with $\Lambda/\zeta<|k|<\Lambda$, and integrate out $\phi_+$ to obtain a [Wilsonian effective action](../../../perturbative-quantum-field-theory.md#wilsonian-effective-action) for $\phi_-$. Next rescale momenta by $k'=\zeta k$, equivalently coordinates by $x'=x/\zeta$, to restore the cutoff to $\Lambda$. Finally rescale the field to restore the chosen normalization of the gradient term. Repeating these operations produces a [renormalization-group flow](../../../critical-phenomenon.md#renormalization-group-flow) of every permitted mass and coupling.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

The free energy is dimensionless, while $d^dx$ has engineering dimension $-d$ and each derivative has dimension one. Requiring

$$
\int d^dx\,(\nabla\phi)^2
$$

to be dimensionless gives $2+2[\phi]-d=0$. Thus the [engineering dimension](../../../critical-phenomenon.md#engineering-dimension) of the field is

$$
\boxed{[\phi]_{\rm eng}=\frac{d-2}{2}}.
$$

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

A scalar field of [scaling dimension](../../../string-theory.md#scaling-dimension) $\Delta_\phi$ has a scale-invariant [two-point correlation function](../../../critical-phenomenon.md#two-point-correlation-function) proportional to $|x|^{-2\Delta_\phi}$. Comparison with the stated form gives

$$
\boxed{\Delta_\phi=\frac{d-2+\eta}{2}}.
$$

The difference $\eta/2$ from the engineering value is the field's [anomalous dimension](../../../critical-phenomenon.md#anomalous-dimension), generated by fluctuations and interactions at a non-Gaussian [renormalization-group fixed point](../../../critical-phenomenon.md#renormalization-group-fixed-point).

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

Ignoring interactions, every field has dimension $(d-2)/2$, and every Laplacian contributes two derivatives. The operator $\phi^n(\nabla^2\phi)^m$ therefore has dimension

$$
\Delta_{\mathcal O}=\frac{(n+m)(d-2)}2+2m.
$$

Because the integrated interaction $\int d^dx\,g\mathcal O$ is dimensionless, the coupling has scaling dimension

$$
\boxed{\Delta_g=d-\frac{(n+m)(d-2)}2-2m}.
$$

It is a [relevant coupling](../../../perturbative-quantum-field-theory.md#relevant-coupling) when $\Delta_g>0$, a [marginal coupling](../../../perturbative-quantum-field-theory.md#marginal-coupling) when $\Delta_g=0$, and an [irrelevant coupling](../../../perturbative-quantum-field-theory.md#irrelevant-coupling) when $\Delta_g<0$.

<h3 id="2/e">e</h3>

↑ **Parent:** [2](#2)

<h4 id="2/e/solution">Solution</h4>

↑ **Parent:** [E](#2/e)

Expand the quintic interaction after the slow-fast split. Its term with three slow fields and two fast fields is

$$
\gamma_0\binom52\phi_-^3\phi_+^2.
$$

The first term of the [cumulant expansion](../../../probability-theory.md#cumulant-expansion) therefore contains

$$
10\gamma_0\int d^dx\,\phi_-^3(x)\langle\phi_+^2(x)\rangle_+.
$$

Since the coincident fast-mode propagator is

$$
\langle\phi_+^2(x)\rangle_+
=\int_{\Lambda/\zeta<|q|<\Lambda}\frac{d^dq}{(2\pi)^d}\frac1{q^2+\mu_0^2},
$$

the lowest-order correction is

$$
\boxed{\delta\alpha_0
=10\gamma_0\int_{\Lambda/\zeta<|q|<\Lambda}\frac{d^dq}{(2\pi)^d}\frac1{q^2+\mu_0^2}}.
$$

Its [Feynman diagram](../../../perturbative-quantum-field-theory.md#feynman-diagram) is one five-valent vertex with three external slow-field legs and the remaining two legs contracted into a [tadpole diagram](../../../perturbative-quantum-field-theory.md#tadpole-diagram).

<h3 id="2/f">f</h3>

↑ **Parent:** [2](#2)

<h4 id="2/f/i">i</h4>

↑ **Parent:** [F](#2/f)

<h5 id="2/f/i/solution">Solution</h5>

↑ **Parent:** [I](#2/f/i)

One cubic vertex cannot leave four external legs. Two cubic vertices can be joined by one contracted fast-field line, leaving four slow-field legs, so the first correction to $\lambda_0$ involving $\alpha_0$ is

$$
\boxed{O(\alpha_0^2)}.
$$

It arises from the second term of the [cumulant expansion](../../../probability-theory.md#cumulant-expansion).

<h4 id="2/f/ii">ii</h4>

↑ **Parent:** [F](#2/f)

<h5 id="2/f/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/f/ii)

A correction with three external legs can be made from one cubic and one quartic vertex by contracting four of their seven fields into internal lines. Consequently the first correction to $\alpha_0$ involving $\lambda_0$ is

$$
\boxed{O(\alpha_0\lambda_0)}.
$$

A purely quartic interaction cannot generate an odd interaction because its $\mathbb Z_2$ symmetry forbids odd powers of $\phi$.

## 3

↑ **Parent:** [Paper 303](paper-303.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

The constraint $\mathbf n\mathbin\cdot\mathbf n=1$ makes $\mathbf n$ dimensionless. Since $d^dx\,(\partial_i n_A)^2$ has engineering dimension $2-d$, dimensional consistency of the [O(N) nonlinear sigma model](../../../quantum-field-theory.md#o-n-nonlinear-sigma-model) gives

$$
\boxed{[g]_{\rm eng}=2-d}.
$$

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Choose the positive local branch of the constraint,

$$
\sigma=\sqrt{1-\boldsymbol\pi^2}.
$$

The [chain rule](../../../calculus.md#chain-rule) gives

$$
\partial_i\sigma=-\frac{\pi_a\partial_i\pi_a}{\sqrt{1-\boldsymbol\pi^2}},
$$

and therefore

$$
(\partial_i\mathbf n)^2=(\partial_i\pi_a)(\partial_i\pi_a)
+\frac{\pi_a(\partial_i\pi_a)\pi_b(\partial_i\pi_b)}{1-\boldsymbol\pi^2}.
$$

Substitution into the original free energy gives exactly

$$
\boxed{F[\boldsymbol\pi]=\int d^dx\,\frac1{2g}\left[(\partial_i\pi_a)(\partial_i\pi_a)+\frac{\pi_a(\partial_i\pi_a)\pi_b(\partial_i\pi_b)}{1-\boldsymbol\pi^2}\right]}.
$$

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

For small $\boldsymbol\pi$, expand $(1-\boldsymbol\pi^2)^{-1}=1+O(\boldsymbol\pi^2)$ and retain the quartic interaction $(\boldsymbol\pi\mathbin\cdot\partial_i\boldsymbol\pi)^2/(2g_0)$. Split $\boldsymbol\pi=\boldsymbol\pi^-+\boldsymbol\pi^+$ and contract the fast fields in the shell $\Lambda/\zeta<|q|<\Lambda$. To first order in

$$
I_d=\int_{\Lambda/\zeta}^{\Lambda}\frac{d^dq}{(2\pi)^d}\frac1{q^2},
$$

the contraction adds $I_d$ to the inverse coefficient of the slow-field kinetic term. The prescribed [wave-function renormalization](../../../perturbative-quantum-field-theory.md#wave-function-renormalization)

$$
\boldsymbol\pi'=\frac{\boldsymbol\pi^-}{A},
\qquad
A=1-\frac12(N-1)g_0I_d,
$$

then multiplies that coefficient by $A^2$. Hence

$$
\left(\frac1{g_0}+I_d\right)A^2
=\frac1{g_0}-(N-2)I_d+O(g_0I_d^2).
$$

Finally the coordinate rescaling contributes $\zeta^{d-2}$, and thus

$$
\boxed{\frac1{g(\zeta)}=\zeta^{d-2}\left[\frac1{g_0}+(2-N)I_d\right]}.
$$

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

Let $s=\log\zeta$. For an infinitesimal momentum shell,

$$
\frac{dI_d}{ds}=\frac{\Omega_{d-1}}{(2\pi)^d}\Lambda^{d-2}.
$$

Differentiating the inverse-coupling relation and using $d(1/g)/ds=-g^{-2}dg/ds$ gives the one-loop [beta function](../../../perturbative-quantum-field-theory.md#beta-function-physics)

$$
\frac{dg}{ds}=-(d-2)g+\frac{\Omega_{d-1}}{(2\pi)^d}\Lambda^{d-2}(N-2)g^2.
$$

For $d=2+\epsilon$, $\Omega_{d-1}/(2\pi)^d=1/(2\pi)+O(\epsilon)$, so

$$
\boxed{\frac{dg}{ds}\simeq-\epsilon g+(N-2)\Lambda^\epsilon\frac{g^2}{2\pi}}.
$$

<h3 id="3/e">e</h3>

↑ **Parent:** [3](#3)

<h4 id="3/e/solution">Solution</h4>

↑ **Parent:** [E](#3/e)

The [renormalization-group fixed points](../../../critical-phenomenon.md#renormalization-group-fixed-point) are the zeros of the [beta function](../../../perturbative-quantum-field-theory.md#beta-function-physics):

$$
\boxed{g_0^*=0,
\qquad
g_c^*=\frac{2\pi\epsilon}{(N-2)\Lambda^\epsilon}}.
$$

For $N>2$ and $\epsilon>0$, the positive fixed point $g_c^*$ separates the low-temperature ordered flow toward $g=0$ from the high-temperature strong-coupling flow. At $\epsilon=0$ the two perturbative fixed points merge at zero.

<h3 id="3/f">f</h3>

↑ **Parent:** [3](#3)

<h4 id="3/f/solution">Solution</h4>

↑ **Parent:** [F](#3/f)

Identifying $g$ with temperature, write $g=g_c^*+\delta g$ near the nonzero critical fixed point. The derivative of the beta function there is

$$
\beta'(g_c^*)=-\epsilon+2\frac{N-2}{2\pi}\Lambda^\epsilon g_c^*=\epsilon.
$$

Thus the temperature-like perturbation has renormalization-group eigenvalue $y_t=\epsilon$. Since the [correlation-length critical exponent](../../../critical-phenomenon.md#correlation-length-critical-exponent) satisfies $\nu=1/y_t$,

$$
\boxed{\nu=\frac1\epsilon+O(1)}.
$$

The Gaussian fixed point $g=0$ is the stable ordered-phase fixed point for $d>2$, rather than the finite-temperature transition. In exactly two dimensions the flow instead gives an essential, exponential correlation-length divergence, corresponding formally to $\nu=\infty$ rather than a finite power-law exponent.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2021](../../2021.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
