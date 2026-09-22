# Paper 303

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2019/paper_303.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2019/paper_303.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
- [3](#3)
  - [i](#3/i)
    - [Solution](#3/i/solution)
  - [ii](#3/ii)
    - [Solution](#3/ii/solution)
  - [iii](#3/iii)
    - [Solution](#3/iii/solution)
  - [iv](#3/iv)
    - [Solution](#3/iv/solution)

## 1

↑ **Parent:** [Paper 303](paper-303.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

A [momentum-shell renormalization group](../../../critical-phenomenon.md#momentum-shell-renormalization-group) step has three parts. First split the field into slow and fast [Fourier modes](../../../fourier-analysis.md#fourier-mode), $\phi=\phi_<+\phi_>$, and integrate over the shell $\Lambda/\zeta<|q|<\Lambda$. Second rescale $q'=\zeta q$, or equivalently $x'=x/\zeta$, to restore the [ultraviolet cutoff](../../../quantum-field-theory.md#ultraviolet-cutoff) to $\Lambda$. Third rescale the field so that the coefficient of $(\nabla\phi)^2/2$ returns to its chosen normalization. The resulting [free energy](../../../thermodynamics.md#thermodynamic-free-energy) has the same operator expansion but new couplings; iteration traces a [renormalization-group flow](../../../critical-phenomenon.md#renormalization-group-flow) in coupling space.

For the first step only, write $F=F_0+V$ and average over the fast modes of the [Gaussian field theory](../../../critical-phenomenon.md#gaussian-field-theory). The [cumulant expansion](../../../probability-theory.md#cumulant-expansion) gives

$$
F_{\rm eff}[\phi_<]=F_0[\phi_<]+\langle V\rangle_>
-\frac12\langle V^2\rangle_{>,c}
+\frac16\langle V^3\rangle_{>,c}+\cdots.
$$

Here

$$
V=\lambda_0\int d^dx\,
(\phi_<^3+3\phi_<^2\phi_>+3\phi_<\phi_>^2+\phi_>^3).
$$

At order $\lambda_0^2$, the connected contraction of two $3\lambda_0\phi_<\phi_>^2$ vertices gives the low-momentum two-point term. Since $\langle\phi_>^2(x)\phi_>^2(y)\rangle_c=2G_>(x-y)^2$,

$$
\delta F^{(2)}=-9\lambda_0^2
\int d^dx\,d^dy\,\phi_<(x)G_>(x-y)^2\phi_<(y).
$$

Expanding at small external momentum and matching $(\mu'^2/2)\int\phi_<^2$ yields

$$
\boxed{\mu'^2=\mu_0^2-18\lambda_0^2
\int_{\Lambda/\zeta<|q|<\Lambda}\frac{d^dq}{(2\pi)^d}
\frac1{(q^2+\mu_0^2)^2}+O(\lambda_0^4).}
$$

The first cumulant also produces a term linear in $\phi_<$; it is removed by fixing the one-point function, or equivalently by a [field redefinition](../../../perturbative-quantum-field-theory.md#field-redefinition), and does not change the displayed [one-particle-irreducible correlation function](../../../perturbative-quantum-field-theory.md#one-particle-irreducible-correlation-function) correction to the mass.

The leading vertex correction is order $\lambda_0^3$. Taking $3\lambda_0\phi_<\phi_>^2$ from each of three vertices, the connected [Wick contractions](../../../perturbative-quantum-field-theory.md#wick-contraction) form a triangle. There are eight contractions, so the third cumulant contributes $27\times8/3!=36$ times the triangle integral. At zero external momentum,

$$
\boxed{\lambda'=\lambda_0+36\lambda_0^3
\int_{\Lambda/\zeta<|q|<\Lambda}\frac{d^dq}{(2\pi)^d}
\frac1{(q^2+\mu_0^2)^3}+O(\lambda_0^5).}
$$

For nonzero external momenta the three propagators carry the corresponding shifted loop momenta, with every internal line restricted to the fast shell.

## 2

↑ **Parent:** [Paper 303](paper-303.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Write $m_i=\mu_i^2$ and $r^2=\phi_1^2+\phi_2^2$. The uniform [Landau free energy](../../../critical-phenomenon.md#landau-free-energy) is

$$
V(\phi_1,\phi_2)=\frac12m_1\phi_1^2+\frac12m_2\phi_2^2+gr^4,
$$

so stationarity requires

$$
\phi_i(m_i+4gr^2)=0.
$$

For $m_1,m_2>0$, the unique [ground state](../../../quantum-mechanics.md#ground-state) is $(0,0)$ and the $\mathbb Z_2\times\mathbb Z_2$ [discrete symmetry](../../../physics.md#discrete-symmetry) is unbroken. If $m_1<0$ and $|m_1|>|m_2|$, then

$$
\boxed{(\phi_1,\phi_2)=\left(\pm\sqrt{\frac{-m_1}{4g}},0\right),}
$$

which breaks the first $\mathbb Z_2$ and leaves the second intact. This includes the case in which both masses are negative, because $m_1$ is then the more negative one. The remaining possible ordered case under the stated inequality is $m_1>0>m_2$, for which

$$
\boxed{(\phi_1,\phi_2)=\left(0,\pm\sqrt{\frac{-m_2}{4g}}\right),}
$$

and only the second $\mathbb Z_2$ is broken. The [Hessian matrix](../../../calculus.md#hessian-matrix) in each ordered state is positive because the uncondensed direction has squared mass $m_k-m_j>0$, where $m_j$ is the condensed, more negative mass.

Near either continuous transition the nonzero order parameter is proportional to $(-m_i)^{1/2}$. Hence the [mean-field critical exponents](../../../critical-phenomenon.md#mean-field-critical-exponent) are

$$
\boxed{\beta_1=\beta_2=\frac12.}
$$

The [lower critical dimension](../../../critical-phenomenon.md#lower-critical-dimension) is the dimension at or below which fluctuations destroy the proposed finite-temperature ordered phase. Here the broken symmetry is discrete, so $d_{\rm l}=1$. In one dimension a [domain wall](../../../critical-phenomenon.md#domain-wall) interpolating between the two signs has finite energy, whereas its possible position gives an [entropy](../../../thermodynamics.md#entropy) growing as $\log L$. Domain walls therefore occur with nonzero density at every positive [temperature](../../../thermodynamics.md#temperature) and split the system into domains of finite typical length. Thus **there is no finite-temperature ordered phase in one dimension**.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

When $m_1=m_2=\mu^2$, the [free energy](../../../thermodynamics.md#thermodynamic-free-energy) has [continuous symmetry](../../../physics.md#continuous-symmetry) $O(2)$. Its ordered minima satisfy

$$
\rho_0^2=\phi_1^2+\phi_2^2=-\frac{\mu^2}{4g}.
$$

Continuous phase fluctuations make the lower critical dimension $d_{\rm l}=2$, in agreement with the [Mermin-Wagner theorem](../../../critical-phenomenon.md#mermin-wagner-theorem). In two dimensions write the complex [order parameter](../../../critical-phenomenon.md#order-parameter) as $\psi=\rho_0e^{i\theta}$. Neglecting the massive [amplitude mode](../../../quantum-field-theory.md#higgs-mode) gives the [Goldstone-mode effective free energy](../../../critical-phenomenon.md#goldstone-mode-effective-free-energy)

$$
F_\theta=\frac{\rho_0^2}{2}\int d^2x\,(\nabla\theta)^2.
$$

The [phase-difference variance](../../../critical-phenomenon.md#phase-difference-variance) is

$$
\langle[\theta(x)-\theta(0)]^2\rangle
=\frac1{\pi\rho_0^2}\log\frac r a+O(1),
$$

and therefore

$$
\langle\psi(x)\psi(0)^*\rangle
\sim \rho_0^2\exp\left[-\frac12
\langle(\theta(x)-\theta(0))^2\rangle\right]
\sim r^{-\eta},
$$

with

$$
\boxed{\eta=\frac1{2\pi\rho_0^2}=-\frac{2g}{\pi\mu^2}.}
$$

Thus [spin waves](../../../critical-phenomenon.md#spin-wave) replace true long-range order by [quasi-long-range order](../../../critical-phenomenon.md#quasi-long-range-order).

A [vortex](../../../critical-phenomenon.md#phase-vortex)-antivortex pair of separation $R$ has the logarithmic energy $E_{\rm pair}\simeq2\pi\rho_0^2\log(R/a)$. The number of pair separations below $R$ grows as $R^2$, giving the coarse entropy $S_{\rm pair}\simeq2\log(R/a)$. Thus

$$
F_{\rm pair}\simeq2(\pi\rho_0^2-1)\log(R/a),
$$

and widely separated pairs become favorable at $\rho_0^2\simeq1/\pi$. Substituting the mean-field stiffness gives

$$
\boxed{\mu^2\simeq-\frac{4g}{\pi},}
$$

suggesting a [Berezinskii–Kosterlitz–Thouless transition](../../../critical-phenomenon.md#berezinskii-kosterlitz-thouless-transition). The numerical location is only a bare-stiffness estimate: vortex-core fluctuations renormalize the stiffness near the transition.

## 3

↑ **Parent:** [Paper 303](paper-303.md)

<h3 id="3/i">i</h3>

↑ **Parent:** [3](#3)

<h4 id="3/i/solution">Solution</h4>

↑ **Parent:** [I](#3/i)

At a critical point, a [local field operator](../../../quantum-field-theory.md#local-operator-physics) $\mathcal O$ has [scaling dimension](../../../string-theory.md#scaling-dimension) $\Delta_{\mathcal O}$ if $\mathcal O(x)\mapsto b^{-\Delta_{\mathcal O}}\mathcal O(x/b)$ under coarse-graining by $b$. The coupling $u$ in $\int d^dx\,u\mathcal O$ has renormalization-group [eigenvalue](../../../linear-operator-theory.md#eigenvalue)

$$
y_u=d-\Delta_{\mathcal O}.
$$

A perturbation is a [relevant operator](../../../critical-phenomenon.md#relevant-operator) when $y_u>0$, an [irrelevant operator](../../../critical-phenomenon.md#irrelevant-operator) when $y_u<0$, and a [marginal operator](../../../critical-phenomenon.md#marginal-operator) when $y_u=0$; nonlinear terms in its [renormalization-group beta function](../../../perturbative-quantum-field-theory.md#beta-function-physics) decide the fate of a marginal coupling. Irrelevant microscopic interactions decay under coarse-graining, so many distinct systems approach the same fixed point and share one [universality class](../../../critical-phenomenon.md#universality-class).

Near criticality the singular [free energy](../../../thermodynamics.md#thermodynamic-free-energy) density is of order one per correlation volume:

$$
f_{\rm s}\sim\xi^{-d}\sim t^{\nu d}.
$$

The [heat capacity](../../../thermodynamics.md#heat-capacity) contains two derivatives with respect to [temperature](../../../thermodynamics.md#temperature), so

$$
c_{\rm s}\sim\frac{d^2f_{\rm s}}{dt^2}
\sim t^{\nu d-2}=t^{-\alpha}.
$$

Consequently the [hyperscaling relation](../../../critical-phenomenon.md#hyperscaling-relation) is

$$
\boxed{\alpha=2-d\nu.}
$$

<h3 id="3/ii">ii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#3/ii)

The critical [two-point correlation function](../../../critical-phenomenon.md#two-point-correlation-function) shows that the field has scaling dimension

$$
\Delta_\phi=\frac{d-2+\eta}{2}.
$$

In the ordered phase the [correlation length](../../../critical-phenomenon.md#correlation-length) is the only diverging scale, so the [order parameter](../../../critical-phenomenon.md#order-parameter) scales as

$$
\phi\sim\xi^{-\Delta_\phi}
\sim t^{\nu\Delta_\phi}.
$$

Therefore

$$
\boxed{\beta=\frac\nu2(d-2+\eta).}
$$

<h3 id="3/iii">iii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#3/iii)

The [Gaussian fixed point](../../../critical-phenomenon.md#gaussian-fixed-point) is

$$
\boxed{(\mu_*^2,g_*)=(0,0).}
$$

Linearizing there gives $d\mu^2/ds=2\mu^2+\cdots$, so the [mass term](../../../quantum-field-theory.md#mass-term) is relevant with [eigenvalue](../../../linear-operator-theory.md#eigenvalue) $y_{\mu^2}=2$. The coupling $g$ has no linear term and is classically marginal, $y_g=0$; for positive $g$ the term $bg^2$ makes it marginally relevant in the infrared convention of the question. Since the inverse thermal eigenvalue is the [correlation-length critical exponent](../../../critical-phenomenon.md#correlation-length-critical-exponent),

$$
\boxed{\nu_{\rm G}=\frac1{y_{\mu^2}}=\frac12.}
$$

<h3 id="3/iv">iv</h3>

↑ **Parent:** [3](#3)

<h4 id="3/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#3/iv)

Besides $g=0$, the coupling beta function vanishes at

$$
g_*^2=\frac bc.
$$

The mass fixed-point equation is

$$
\mu_*^2(\Lambda^2+\mu_*^2)=\Lambda^4g_*^2,
$$

so the root continuously connected to the origin is

$$
\boxed{\frac{\mu_*^2}{\Lambda^2}
=\frac{-1+\sqrt{1+4b/c}}2
=\frac bc+O\left(\frac{b^2}{c^2}\right),
\qquad g_*^2=\frac bc.}
$$

Perturbation theory requires **$b/c\ll1$**, ensuring that the fixed-point coupling is small and the omitted higher powers are suppressed.

<a id="3/iv/image-renormalization-group-flow-near-the-gaussian-and-interacting-fixed-points"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-303-rg-flow.png)

**[Figure 1](#3/iv/image-renormalization-group-flow-near-the-gaussian-and-interacting-fixed-points). Renormalization-group flow near the Gaussian and interacting fixed points**. The arrows point toward the infrared. The Gaussian fixed point lies at the origin, the interacting fixed point lies at positive mass and coupling, and the red tuned critical trajectory connects their neighborhoods. Flows away from that trajectory leave along the relevant mass direction.

For increasing infrared scale $s$, positive $g<g_*$ flows upward toward $g_*$ and $g>g_*$ flows downward toward it. The mass direction remains relevant, so only the tuned critical trajectory reaches the interacting fixed point; trajectories on either side leave toward the two phases.

The relevant thermal [eigenvalue](../../../linear-operator-theory.md#eigenvalue) is obtained from the [stability matrix of a renormalization-group fixed point](../../../critical-phenomenon.md#stability-matrix-of-a-renormalization-group-fixed-point) by differentiating the mass beta function:

$$
y_t=\left.\frac{\partial\beta_{\mu^2}}{\partial\mu^2}\right|_*
=2+\frac{2\Lambda^4g_*^2}{(\Lambda^2+\mu_*^2)^2}
=2+2g_*^2+O(g_*^4).
$$

It follows that

$$
\boxed{\nu_*=\frac1{y_t}
=\frac1{2+2g_*^2}+O(g_*^4)
=\frac12\left(1-\frac bc\right)
+O\left(\frac{b^2}{c^2}\right).}
$$

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2019](../../2019.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
