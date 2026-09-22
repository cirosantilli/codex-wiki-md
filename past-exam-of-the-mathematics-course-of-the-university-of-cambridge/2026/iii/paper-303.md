# Paper 303

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2026/III%20Paper%20303.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2026/III%20Paper%20303.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [i](#1/a/i)
      - [Solution](#1/a/i/solution)
    - [ii](#1/a/ii)
      - [Solution](#1/a/ii/solution)
  - [b](#1/b)
    - [i](#1/b/i)
      - [Solution](#1/b/i/solution)
    - [ii](#1/b/ii)
      - [Solution](#1/b/ii/solution)
    - [iii](#1/b/iii)
      - [Solution](#1/b/iii/solution)
    - [iv](#1/b/iv)
      - [Solution](#1/b/iv/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [i](#2/b/i)
      - [Solution](#2/b/i/solution)
    - [ii](#2/b/ii)
      - [Solution](#2/b/ii/solution)
    - [iii](#2/b/iii)
      - [Solution](#2/b/iii/solution)
    - [iv](#2/b/iv)
      - [Solution](#2/b/iv/solution)
  - [c](#2/c)
    - [i](#2/c/i)
      - [Solution](#2/c/i/solution)
    - [ii](#2/c/ii)
      - [Solution](#2/c/ii/solution)
    - [iii](#2/c/iii)
      - [Solution](#2/c/iii/solution)
- [3](#3)
  - [a](#3/a)
    - [i](#3/a/i)
      - [Solution](#3/a/i/solution)
    - [ii](#3/a/ii)
      - [Solution](#3/a/ii/solution)
    - [iii](#3/a/iii)
      - [Solution](#3/a/iii/solution)
    - [iv](#3/a/iv)
      - [Solution](#3/a/iv/solution)
    - [v](#3/a/v)
      - [Solution](#3/a/v/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)

## 1

↑ **Parent:** [Paper 303](paper-303.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/i">i</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/i/solution">Solution</h5>

↑ **Parent:** [I](#1/a/i)

Write $t=T-T_c$. Analyticity gives $\alpha_2=at+O(t^2)$ with $a>0$ and $\alpha_4(T_c)=u>0$. For $t<0$, minimization gives $m^2=-\alpha_2/\alpha_4\sim-at/u$, so $\beta=1/2$. At the minima,

$$
F_{\min}=-\frac{\alpha_2^2}{4\alpha_4}\sim-\frac{a^2}{4u}t^2.
$$

Two temperature derivatives give a finite heat-capacity jump, hence $\alpha=0$. This is the ordinary [mean-field](../../../critical-phenomenon.md#mean-field-critical-exponent) transition of [Landau theory](../../../critical-phenomenon.md#landau-theory).

<h4 id="1/a/ii">ii</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/a/ii)

At the [tricritical point](../../../critical-phenomenon.md#tricritical-point), let $\alpha_2=at+O(t^2)$, $\alpha_4=bt+O(t^2)$ and $\alpha_6(T_c)=u>0$. The nonzero stationarity equation is

$$
at+btm^2+um^4+\cdots=0.
$$

The middle term is subleading, so $m^4\sim-at/u$ and $\beta=1/4$. Substitution gives $F_{\min}\asymp-|t|^{3/2}$, so the heat capacity behaves as $|t|^{-1/2}$ and $\alpha=1/2$.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/i">i</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/i/solution">Solution</h5>

↑ **Parent:** [I](#1/b/i)

Fourier expansion in volume $V$ diagonalizes the quadratic [Landau-Ginzburg theory](../../../critical-phenomenon.md#landau-ginzburg-theory):

$$
F=\frac12\sum_{|k|<\Lambda}K(T,k^2)|\phi_k|^2,
$$

where

$$
K=\mu^2+\gamma k^2+\sum_{n\geq2}\delta_n(k^2)^n
=\mu^2+\gamma k^2+(k^2)^2g(T,k^2),
\qquad
g=\sum_{n\geq2}\delta_n(k^2)^{n-2}.
$$

Each independent real mode contributes a [Gaussian integral](../../../calculus.md#gaussian-integral) proportional to $(T/K)^{1/2}$. Taking $-T\log Z$, dividing by $V$, and replacing the sum by an integral gives, up to field-independent conventions,

$$
\boxed{-\frac T2\int_{|k|<\Lambda}\frac{d^dk}{(2\pi)^d}
\log\frac{\pi VT}{K(T,k^2)}.}
$$

<h4 id="1/b/ii">ii</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/b/ii)

For one mode put $f=-\tfrac T2\log(CT/K)$. Since $c=-T\partial_T^2f$,

$$
c_k=\frac12-\frac{TK_T}{K}-\frac{T^2K_{TT}}{2K}
+\frac{T^2K_T^2}{2K^2}.
$$

Thus

$$
A(T,k^2)=\frac{T^2}{2}\left(\frac{\partial K}{\partial T}\right)^2.
$$

At $(T_c,0)$, $K_T=(\mu^2)'(T_c)\ne0$ because $\mu^2$ has a simple zero, so $A(T_c,0)\ne0$.

<h4 id="1/b/iii">iii</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#1/b/iii)

Near the ordinary critical point, $K\sim at+\gamma k^2$. Rescaling $k=t^{1/2}q$ gives the [Gaussian fluctuation correction near a critical point](../../../critical-phenomenon.md#gaussian-fluctuation-correction-near-a-critical-point)

$$
\int\frac{d^dk}{(t+k^2)^2}\asymp t^{d/2-2}.
$$

**Thus $\alpha_{\mathrm{fl}}=2-d/2$. It becomes as important as the mean-field value $\alpha=0$ at $d=4$, so the ordinary [upper critical dimension](../../../critical-phenomenon.md#upper-critical-dimension) is $d_c=4$.**

<h4 id="1/b/iv">iv</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#1/b/iv)

The quadratic kernel still has $K\sim at+\gamma k^2$, so $\alpha_{\mathrm{fl}}=2-d/2$. The tricritical mean-field exponent is $\alpha=1/2$. Equating them gives $2-d/2=1/2$, hence the tricritical [upper critical dimension](../../../critical-phenomenon.md#upper-critical-dimension) is $d_c=3$.

## 2

↑ **Parent:** [Paper 303](paper-303.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

A Wilsonian [renormalization group](../../../critical-phenomenon.md#renormalization-group) step:

- integrates out fast modes $\Lambda/\zeta<|k|<\Lambda$;
- rescales $x'=x/\zeta$ and $k'=\zeta k$ to restore the cutoff;
- rescales the field to restore the chosen gradient-term normalization.

The resulting effective free energy defines the transformed couplings and their flow.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/i">i</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/i/solution">Solution</h5>

↑ **Parent:** [I](#2/b/i)

At the [Gaussian fixed point](../../../critical-phenomenon.md#gaussian-fixed-point), set $a_d=12\Omega_{d-1}\Lambda^{d-2}/(2\pi)^d$. The linearized flow is

$$
\frac d{d\log\zeta}
\begin{pmatrix}\mu^2\\g\end{pmatrix}
=\begin{pmatrix}2&a_d\\0&4-d\end{pmatrix}
\begin{pmatrix}\mu^2\\g\end{pmatrix}.
$$

The mass direction, corresponding to $\phi^2$, has coupling dimension $y_t=2$. For $d\ne2$, the second eigendirection is

$$
(\delta\mu^2,\delta g)=\left(-\frac{a_d}{d-2},1\right)\delta g
$$

and has $y_g=4-d$; it is the tadpole-subtracted mixture of $\phi^4$ and $\phi^2$. The corresponding operator dimensions are $d-2$ and $2d-4$.

<h4 id="2/b/ii">ii</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/b/ii)

For $d<4$, $y_g=4-d>0$, so the quartic coupling is a [relevant direction of a fixed point](../../../critical-phenomenon.md#relevant-direction-of-a-fixed-point). Generic Ising-like systems therefore flow away from the Gaussian point toward the interacting [Wilson-Fisher fixed point](../../../critical-phenomenon.md#wilson-fisher-fixed-point), which controls the Ising [universality class](../../../critical-phenomenon.md#universality-class) below four dimensions.

<h4 id="2/b/iii">iii</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#2/b/iii)

Put $r=\mu^2/\Lambda^2$ and $\widetilde g=\Lambda^{d-4}g$. At $d=4-\epsilon$, $\Omega_3/(2\pi)^4=1/(8\pi^2)$ gives

$$
\beta_r=2r+\frac{3}{2\pi^2}\frac{\widetilde g}{1+r},
\qquad
\beta_{\widetilde g}=\epsilon\widetilde g-\frac9{2\pi^2}
\frac{\widetilde g^2}{(1+r)^2}.
$$

The nonzero fixed point is

$$
\widetilde g_*=\frac{2\pi^2}{9}\epsilon+O(\epsilon^2),
\qquad
r_*=-\frac\epsilon6+O(\epsilon^2),
$$

which is the stated [Wilson-Fisher fixed point](../../../critical-phenomenon.md#wilson-fisher-fixed-point).

<h4 id="2/b/iv">iv</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#2/b/iv)

Linearization at the fixed point gives

$$
y_t=2-\frac\epsilon3+O(\epsilon^2),
\qquad
y_{\mathrm{irr}}=-\epsilon+O(\epsilon^2).
$$

The relevant eigendirection is $(\delta r,\delta\widetilde g)=(1,O(\epsilon^2))$. An irrelevant eigendirection is

$$
(\delta r,\delta\widetilde g)
=\left(-\frac3{4\pi^2},1\right)+O(\epsilon).
$$

**Thus the mass-like combination is relevant and the quartic-like combination is irrelevant; neither is marginal for $\epsilon>0$.**

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/i">i</h4>

↑ **Parent:** [C](#2/c)

<h5 id="2/c/i/solution">Solution</h5>

↑ **Parent:** [I](#2/c/i)

The coefficient $A$ comes from one sextic vertex with two external slow legs and two fast tadpole loops. The coefficient $B$ comes from one sextic vertex with four external slow legs and one fast tadpole. The coefficient $C$ comes from one quartic and one sextic vertex joined by two fast propagators, leaving six external slow legs.

<h4 id="2/c/ii">ii</h4>

↑ **Parent:** [C](#2/c)

<h5 id="2/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/c/ii)

Choosing two slow legs in $h(\phi_<+\phi_>)^6$ and contracting four fast legs gives $\binom62(3)hI_1^2\phi_<^2$. Since the mass term is $\mu^2\phi_<^2/2$,

$$
A=90.
$$

Choosing four slow legs and contracting the remaining pair gives $B=\binom64=15$. For the connected quartic-sextic cumulant, the factor is $\binom42\binom62 2!=180$ and the cumulant has a minus sign, so

$$
B=15,\qquad C=-180.
$$

As a check, two quartic vertices give $-\tfrac12\binom42^2 2!=-36$, matching the supplied coefficient.

<h4 id="2/c/iii">iii</h4>

↑ **Parent:** [C](#2/c)

<h5 id="2/c/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#2/c/iii)

The canonical eigenvalue of $h$ is

$$
y_h=d-6\frac{d-2}{2}=6-2d=-2+2\epsilon.
$$

Thus $\beta_h=(-2+O(\epsilon))h+O(g^3)+O(h^2)$. At a fixed point this forces $h_*=O(g_*^3)=O(\epsilon^3)$. Its feedback into the mass and quartic flows begins only at order $\epsilon^3$, so the order-$\epsilon$ fixed point from part (b)(iii) is unaffected.

## 3

↑ **Parent:** [Paper 303](paper-303.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/i">i</h4>

↑ **Parent:** [A](#3/a)

<h5 id="3/a/i/solution">Solution</h5>

↑ **Parent:** [I](#3/a/i)

At a fixed point, the [order parameter](../../../critical-phenomenon.md#order-parameter) can be chosen as a dilation eigenoperator. Therefore, for $x'=x/\zeta$,

$$
\phi'(x')=\zeta^{\Delta_\phi}\phi(x).
$$

Interactions shift $\Delta_\phi$ from $(d-2)/2$ to $(d-2+\eta)/2$.

<h4 id="3/a/ii">ii</h4>

↑ **Parent:** [A](#3/a)

<h5 id="3/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/a/ii)

If $t'=\zeta^{\Delta_t}t$, lengths shrink by $\zeta$, so $\xi(t')=\zeta^{-1}\xi(t)$. Substituting $\xi(t)\sim t^{-\nu}$ gives $\zeta^{-\nu\Delta_t}=\zeta^{-1}$ and hence

$$
\boxed{\Delta_t=\frac1\nu.}
$$

<h4 id="3/a/iii">iii</h4>

↑ **Parent:** [A](#3/a)

<h5 id="3/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#3/a/iii)

The source term transforms as

$$
\int d^dx\,B\phi
=\int d^dx'\,\zeta^{d-\Delta_\phi}B\phi'.
$$

Therefore

$$
\boxed{\Delta_B=d-\Delta_\phi=\frac{d+2-\eta}{2}.}
$$

<h4 id="3/a/iv">iv</h4>

↑ **Parent:** [A](#3/a)

<h5 id="3/a/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#3/a/iv)

Choose $\zeta=t^{-\nu}$. The singular free-energy density scales as $t^{d\nu}$, giving the [hyperscaling relation](../../../critical-phenomenon.md#hyperscaling-relation) $\alpha=2-d\nu$. The order parameter gives

$$
\beta=\nu\Delta_\phi=\frac12(d-2+\eta)\nu.
$$

The susceptibility has exponent

$$
\gamma=\nu(d-2\Delta_\phi)=\nu(2-\eta).
$$

At $t=0$, choosing $\zeta=B^{-1/\Delta_B}$ gives

$$
\boxed{\delta=\frac{\Delta_B}{\Delta_\phi}
=\frac{d+2-\eta}{d-2+\eta}.}
$$

<h4 id="3/a/v">v</h4>

↑ **Parent:** [A](#3/a)

<h5 id="3/a/v/solution">Solution</h5>

↑ **Parent:** [V](#3/a/v)

For $d>4$, the quartic coupling has $y_g=4-d<0$, but setting it to zero removes the stabilizing term. It is a [dangerously irrelevant coupling](../../../critical-phenomenon.md#dangerously-irrelevant-coupling). At $t=0$, minimizing $g\phi^4-B\phi$ gives $\phi\sim(B/g)^{1/3}$ and $\delta=3$. This is consistent with Gaussian scaling because

$$
\frac{\Delta_B-y_g}{3}
=\frac{(d+2)/2-(4-d)}3
=\frac{d-2}{2}=\Delta_\phi.
$$

For $d<4$, $g$ flows to a nonzero [Wilson-Fisher fixed point](../../../critical-phenomenon.md#wilson-fisher-fixed-point), so no dangerously irrelevant zero-coupling limit spoils the ordinary [scaling relations](../../../critical-phenomenon.md#scaling-relation-for-critical-exponents).

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Put $\rho_i=|\psi_i|^2$. The uniform potential is

$$
V=\mu_1^2\rho_1+\mu_2^2\rho_2+g(\rho_1+\rho_2)^2.
$$

If both masses are positive, $\rho_1=\rho_2=0$. If $\mu_1^2<\min(0,\mu_2^2)$, only $\psi_1$ condenses, with $\rho_1=-\mu_1^2/(2g)$; symmetrically, only $\psi_2$ condenses when $\mu_2^2<\min(0,\mu_1^2)$. The positive coordinate axes are continuous-transition lines. On $\mu_1^2=\mu_2^2=\mu^2<0$, every pair with

$$
|\psi_1|^2+|\psi_2|^2=-\frac{\mu^2}{2g}
$$

is a minimum; crossing this diagonal exchanges the two condensates, so it is a coexistence line ending at the origin.

Away from the diagonal the symmetry is $U(1)_1\times U(1)_2$. It is unbroken in the normal phase. In either one-condensate phase one factor is broken and the other remains, giving one [Goldstone boson](../../../critical-phenomenon.md#goldstone-boson). On the diagonal the symmetry is enhanced to $U(2)$. For positive equal mass it is unbroken; for negative equal mass it breaks as $U(2)\to U(1)$ and gives three Goldstone bosons. At the origin $U(2)$ is unbroken although both quadratic modes are critical.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2026](../../2026.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
