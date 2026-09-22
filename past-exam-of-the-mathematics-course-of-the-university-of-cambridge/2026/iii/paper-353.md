# Paper 353

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2026/III%20Paper%20353.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2026/III%20Paper%20353.pdf)

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
  - [c](#1/c)
    - [i](#1/c/i)
      - [Solution](#1/c/i/solution)
    - [ii](#1/c/ii)
      - [Solution](#1/c/ii/solution)
    - [iii](#1/c/iii)
      - [Solution](#1/c/iii/solution)
- [2](#2)
  - [a](#2/a)
    - [i](#2/a/i)
      - [Solution](#2/a/i/solution)
    - [ii](#2/a/ii)
      - [Solution](#2/a/ii/solution)
    - [iii](#2/a/iii)
      - [Solution](#2/a/iii/solution)
  - [b](#2/b)
    - [i](#2/b/i)
      - [Solution](#2/b/i/solution)
    - [ii](#2/b/ii)
      - [Solution](#2/b/ii/solution)
    - [iii](#2/b/iii)
      - [Solution](#2/b/iii/solution)
- [3](#3)
  - [i](#3/i)
    - [Solution](#3/i/solution)
  - [ii](#3/ii)
    - [Solution](#3/ii/solution)
  - [iii](#3/iii)
    - [Solution](#3/iii/solution)
  - [iv](#3/iv)
    - [Solution](#3/iv/solution)
  - [v](#3/v)
    - [Solution](#3/v/solution)
  - [vi](#3/vi)
    - [Solution](#3/vi/solution)
  - [vii](#3/vii)
    - [Solution](#3/vii/solution)
  - [viii](#3/viii)
    - [Solution](#3/viii/solution)
- [4](#4)
  - [a](#4/a)
    - [i](#4/a/i)
      - [Solution](#4/a/i/solution)
    - [ii](#4/a/ii)
      - [Solution](#4/a/ii/solution)
    - [iii](#4/a/iii)
      - [Solution](#4/a/iii/solution)
  - [b](#4/b)
    - [i](#4/b/i)
      - [Solution](#4/b/i/solution)
    - [ii](#4/b/ii)
      - [Solution](#4/b/ii/solution)
  - [c](#4/c)
    - [i](#4/c/i)
      - [Solution](#4/c/i/solution)
    - [ii](#4/c/ii)
      - [Solution](#4/c/ii/solution)

## 1

↑ **Parent:** [Paper 353](paper-353.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/i">i</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/i/solution">Solution</h5>

↑ **Parent:** [I](#1/a/i)

Stationarity makes the covariance depend only on $\tau=t-s$. For $\tau>0$,

$$
G(\tau)=e^{-\tau A}\sigma.
$$

At the reversed lag, the $s>t$ formula gives

$$
G(-\tau)=\sigma e^{-\tau A^T},
$$

and therefore

$$
\boxed{G(\tau)=G(-\tau)^T}.
$$

The same identity follows directly by exchanging the two random variables in $G_{ij}(t,s)=\langle x_i(t)x_j(s)\rangle$.

<h4 id="1/a/ii">ii</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/a/ii)

Split the Fourier integral at zero and use the two stationary covariance branches:

$$
s(\omega)=\int_0^\infty e^{-(A+i\omega I)\tau}\sigma\,d\tau
+\int_0^\infty e^{-(A-i\omega I)\tau}\!{}^T\sigma\,d\tau.
$$

Equivalently, Fourier transforming the [Multivariate Ornstein-Uhlenbeck process](../../../stochastic-process.md#multivariate-ornstein-uhlenbeck-process) equation gives

$$
(A+i\omega I)x(\omega)=b\Lambda(\omega).
$$

Unit white-noise covariance then yields the [Ornstein-Uhlenbeck power spectrum](../../../stochastic-process.md#ornstein-uhlenbeck-power-spectrum)

$$
s(\omega)=(A+i\omega I)^{-1}bb^T(A^T-i\omega I)^{-1},
$$

so

$$
\boxed{(A+i\omega I)s(\omega)(A^T-i\omega I)=bb^T}.
$$

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/i">i</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/i/solution">Solution</h5>

↑ **Parent:** [I](#1/b/i)

For $X=(x,p)^T$,

$$
\boxed{A=\begin{pmatrix}0&-1/m\\ \lambda&\gamma/m\end{pmatrix}},
\qquad
\boxed{bb^T=\begin{pmatrix}0&0\\0&2k_BT\gamma\end{pmatrix}}.
$$

Solving $A\sigma+\sigma A^T=bb^T$ gives

$$
\boxed{\sigma=
\begin{pmatrix}
k_BT/\lambda&0\\0&mk_BT
\end{pmatrix}}.
$$

The [canonical ensemble](../../../statistical-physics.md#canonical-ensemble) density proportional to $e^{-H/(k_BT)}$ for $H=p^2/(2m)+\lambda x^2/2$ factorizes into independent centered Gaussians. Its equipartition variances are exactly $\langle x^2\rangle=k_BT/\lambda$ and $\langle p^2\rangle=mk_BT$, while the absence of an $xp$ term gives $\sigma_{12}=0$.

<h4 id="1/b/ii">ii</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/b/ii)

Let

$$
\Delta(\omega)=\frac\lambda m-\omega^2+i\frac{\gamma\omega}{m}.
$$

The second column of $(A+i\omega I)^{-1}$ is $\Delta^{-1}(1/m,i\omega)^T$. Hence

$$
\boxed{s(\omega)=
\frac{2k_BT\gamma}{|\Delta|^2}
\begin{pmatrix}
m^{-2}&-i\omega/m\\
i\omega/m&\omega^2
\end{pmatrix}}.
$$

In particular,

$$
\boxed{s_{xx}(\omega)=
\frac{2k_BT\gamma}
{m^2(\omega^2-\lambda/m)^2+\gamma^2\omega^2}}.
$$

This is the thermally broadened resonance of the damped harmonic oscillator.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/i">i</h4>

↑ **Parent:** [C](#1/c)

<h5 id="1/c/i/solution">Solution</h5>

↑ **Parent:** [I](#1/c/i)

The stationary solution of

$$
dq=-\nu q\,dt+\sqrt{\alpha\nu}\,dW
$$

is

$$
q(t)=\sqrt{\alpha\nu}\int_{-\infty}^te^{-\nu(t-u)}\,dW_u.
$$

It follows from the [Itô isometry](../../../stochastic-calculus.md#ito-isometry) that

$$
\boxed{\langle q(t)q(t+\tau)\rangle
=\frac\alpha2e^{-\nu|\tau|}}.
$$

**Thus $q$ is zero-mean [colored noise](../../../stochastic-process.md#colored-noise) with correlation time $\nu^{-1}$. The equation $\dot x=\mu(-\lambda x+q)$ is an overdamped harmonic particle of mobility $\mu$ driven by that correlated random force.**

<h4 id="1/c/ii">ii</h4>

↑ **Parent:** [C](#1/c)

<h5 id="1/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/c/ii)

For $X=(x,q)^T$,

$$
A=\begin{pmatrix}\mu\lambda&-\mu\\0&\nu\end{pmatrix},
\qquad
bb^T=\begin{pmatrix}0&0\\0&\alpha\nu\end{pmatrix}.
$$

The Lyapunov equation gives $\sigma_{qq}=\alpha/2$, $\sigma_{xq}=\lambda\sigma_{xx}$, and $(\mu\lambda+\nu)\sigma_{xq}=\mu\sigma_{qq}$. Therefore

$$
\boxed{\sigma=
\begin{pmatrix}
\dfrac{\mu\alpha}{2\lambda(\mu\lambda+\nu)}&
\dfrac{\mu\alpha}{2(\mu\lambda+\nu)}\\[8pt]
\dfrac{\mu\alpha}{2(\mu\lambda+\nu)}&\dfrac\alpha2
\end{pmatrix}}.
$$

<h4 id="1/c/iii">iii</h4>

↑ **Parent:** [C](#1/c)

<h5 id="1/c/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#1/c/iii)

Take $\nu\to\infty$ with

$$
\frac\alpha\nu=\frac{2k_BT}{\mu}.
$$

Since $(\nu/2)e^{-\nu|\tau|}\to\delta(\tau)$,

$$
\langle q(t)q(t+\tau)\rangle
=\frac\alpha2e^{-\nu|\tau|}
\longrightarrow\frac{2k_BT}{\mu}\delta(\tau).
$$

Thus $\mu q$ tends to thermal white forcing of covariance $2\mu k_BT\delta(\tau)$, as required by the fluctuation--dissipation relation. The equal-time position variance becomes

$$
\sigma_{xx}=
\frac{\mu\alpha}{2\lambda(\mu\lambda+\nu)}
=\frac{k_BT\nu}{\lambda(\mu\lambda+\nu)}
\longrightarrow\boxed{\frac{k_BT}{\lambda}},
$$

the equilibrium harmonic variance.

## 2

↑ **Parent:** [Paper 353](paper-353.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/i">i</h4>

↑ **Parent:** [A](#2/a)

<h5 id="2/a/i/solution">Solution</h5>

↑ **Parent:** [I](#2/a/i)

Set

$$
\boxed{D=\frac\kappa2}.
$$

The stated curl-free condition says that $C_j=(\kappa^{-1})_{ji}a_i$ is a gradient, $C=\nabla\Psi$. Define

$$
\boxed{V=-2\Psi},
\qquad
\partial_jV=-2(\kappa^{-1})_{ji}a_i.
$$

Then $a=-D\nabla V$, and the [Fokker-Planck probability current](../../../probability-theory.md#fokker-planck-probability-current) becomes

$$
J=aP-D\nabla P
=\boxed{-PD\nabla(V+\log P)}.
$$

This is the [potential condition for a Fokker--Planck equation](../../../probability-theory.md#potential-condition-for-a-fokker-planck-equation).

<h4 id="2/a/ii">ii</h4>

↑ **Parent:** [A](#2/a)

<h5 id="2/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/a/ii)

Normalization makes the derivative of the additive $1$ in $\delta F/\delta P=V+\log P+1$ vanish. Using $\dot P=-\nabla\cdot J$, the no-flux boundary condition, and integration by parts gives

$$
\dot F=\int(V+\log P+1)(-\nabla\cdot J)\,dx
=\int\nabla(V+\log P)\cdot J\,dx.
$$

Substituting the gradient current,

$$
\boxed{\dot F=-\int P\,
\nabla(V+\log P)^TD\nabla(V+\log P)\,dx\leq0}.
$$

Positive definiteness makes equality possible only when $\nabla(V+\log P)=0$, equivalently $J=0$. Thus $F$ is a strict [Fokker--Planck free-energy functional](../../../probability-theory.md#fokker-planck-free-energy-functional) away from stationarity.

<h4 id="2/a/iii">iii</h4>

↑ **Parent:** [A](#2/a)

<h5 id="2/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#2/a/iii)

Let $Z=\int_Xe^{-V}dx$ and $P_B=e^{-V}/Z$. Then

$$
F[P]=\int P\log\frac{P}{P_B}\,dx-\log Z
=D_{\rm KL}(P\|P_B)-\log Z.
$$

By nonnegativity of [Kullback-Leibler divergence](../../../probability-and-statistics.md#kullback-leibler-divergence),

$$
\boxed{F[P]\geq-\log Z},
$$

with equality exactly when $P=P_B$ almost everywhere. Hence a normalizable $P_B$ is the unique minimizer and, because $\dot F<0$ elsewhere, the unique steady density compatible with the boundary condition.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/i">i</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/i/solution">Solution</h5>

↑ **Parent:** [I](#2/b/i)

The independent additive noises give diagonal diffusion $\kappa=\operatorname{diag}(b_1^2,b_2^2)$. Thus

$$
\boxed{
\begin{aligned}
\partial_tP={}&-\partial_{x_1}\!\left[
(r_1x_1-r_1c_1x_1x_2^2-d_1x_1^2)P\right]
+\frac{b_1^2}{2}\partial_{x_1}^2P\\
&-\partial_{x_2}\!\left[
(r_2x_2-r_2c_2x_2x_1^2-d_2x_2^2)P\right]
+\frac{b_2^2}{2}\partial_{x_2}^2P.
\end{aligned}}
$$

The mixed derivatives of $\kappa^{-1}a$ are

$$
\partial_{x_2}\frac{a_1}{b_1^2}
=-\frac{2r_1c_1x_1x_2}{b_1^2},
\qquad
\partial_{x_1}\frac{a_2}{b_2^2}
=-\frac{2r_2c_2x_1x_2}{b_2^2}.
$$

They agree precisely when

$$
\boxed{r_1c_1b_2^2=r_2c_2b_1^2}.
$$

<h4 id="2/b/ii">ii</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/b/ii)

Under the potential condition, integrate $\partial_i\Psi=a_i/b_i^2$ to obtain

$$
\Psi=\frac{r_1x_1^2}{2b_1^2}
-\frac{d_1x_1^3}{3b_1^2}
+\frac{r_2x_2^2}{2b_2^2}
-\frac{d_2x_2^3}{3b_2^2}
-\frac{r_1c_1x_1^2x_2^2}{2b_1^2}.
$$

Since $V=-2\Psi$, the zero-current steady density on the positive quadrant is

$$
\boxed{P_{\rm ss}(x_1,x_2)=\frac1Z\exp\!\left[
\frac{r_1x_1^2}{b_1^2}-\frac{2d_1x_1^3}{3b_1^2}
+\frac{r_2x_2^2}{b_2^2}-\frac{2d_2x_2^3}{3b_2^2}
-\frac{r_1c_1x_1^2x_2^2}{b_1^2}
\right]}.
$$

The equivalent coefficient $r_2c_2/b_2^2$ may be used for the cross term.

<h4 id="2/b/iii">iii</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#2/b/iii)

If $c_1,c_2<0$, the cross term in the exponent becomes positive. Along rays with both densities large it grows quartically, while the self-limiting death terms are only negative cubics. The candidate density is therefore not normalizable and the [Fokker--Planck free-energy functional](../../../probability-theory.md#fokker-planck-free-energy-functional) is not bounded below. Deterministically, mutual nutrient enhancement eventually overwhelms each species' quadratic crowding death and drives runaway growth, potentially in finite time. The stochastic model consequently has no steady probability density and sends probability toward arbitrarily large populations. This signals failure of the idealized growth law at high density; resource depletion or stronger saturation must regularize a biological model.

## 3

↑ **Parent:** [Paper 353](paper-353.md)

<h3 id="3/i">i</h3>

↑ **Parent:** [3](#3)

<h4 id="3/i/solution">Solution</h4>

↑ **Parent:** [I](#3/i)

The functional derivatives are

$$
\frac{\delta F}{\delta\phi}=a\phi+c\psi-\kappa\nabla^2\phi,
\qquad
\frac{\delta F}{\delta\psi}=\bar a\psi+c\phi-\bar\kappa\nabla^2\psi.
$$

With the stated Fourier convention,

$$
\boxed{\dot\phi_{\mathbf q}
=-Mq^2[(a+\kappa q^2)\phi_{\mathbf q}+c\psi_{\mathbf q}]
-i\sqrt{2M}\,\mathbf q\cdot\boldsymbol\Lambda_{\mathbf q}},
$$



$$
\boxed{\dot\psi_{\mathbf q}
=-\Gamma[(\bar a+\bar\kappa q^2)\psi_{\mathbf q}
+c\phi_{\mathbf q}]+\sqrt{2\Gamma}\,\Lambda_{\mathbf q}}.
$$

The first is [conserved order-parameter dynamics](../../../critical-phenomenon.md#conserved-order-parameter-dynamics); its deterministic rate and conserved-noise amplitude vanish at $q=0$. The second is [nonconserved order-parameter dynamics](../../../critical-phenomenon.md#nonconserved-order-parameter-dynamics).

<h3 id="3/ii">ii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#3/ii)

The deterministic relaxation matrix is

$$
\boxed{R(q)=
\begin{pmatrix}
Mq^2(a+\kappa q^2)&Mcq^2\\
\Gamma c&\Gamma(\bar a+\bar\kappa q^2)
\end{pmatrix}}.
$$

Its right eigenvectors are the [hydrodynamic modes](../../../critical-phenomenon.md#hydrodynamic-mode). Writing $A_q=a+\kappa q^2$ and $B_q=\bar a+\bar\kappa q^2$, their decay rates obey

$$
\boxed{(\lambda-Mq^2A_q)(\lambda-\Gamma B_q)
-M\Gamma c^2q^2=0}.
$$

<h3 id="3/iii">iii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#3/iii)

For $M=\Gamma=1$, $a=\bar a$, and $\kappa=\bar\kappa$, put $s=a+\kappa q^2$. Then

$$
R=\begin{pmatrix}q^2s&cq^2\\c&s\end{pmatrix}.
$$

At small $q$, second-order perturbation in $c$ gives the slow conserved and fast nonconserved eigenvalues

$$
\lambda_B=q^2s-\frac{c^2q^2}{s(1-q^2)}+O(c^4),
$$



$$
\lambda_A=s+\frac{c^2q^2}{s(1-q^2)}+O(c^4).
$$

Keeping terms through $q^2$,

$$
\boxed{\lambda_B=q^2\left(a-\frac{c^2}{a}\right)},
\qquad
\boxed{\lambda_A=a+\left(\kappa+\frac{c^2}{a}\right)q^2}.
$$

Stability of the long-wavelength mode requires $a^2>c^2$.

<h3 id="3/iv">iv</h3>

↑ **Parent:** [3](#3)

<h4 id="3/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#3/iv)

For the slow mode choose $e_B=(1,\beta)^T$. The second row gives $c+s\beta=\lambda_B\beta$, so to the requested order

$$
\boxed{\beta=-\frac ca}.
$$

For the fast mode choose $e_A=(\alpha,1)^T$. The first row gives $(\lambda_A-q^2s)\alpha=cq^2$, hence

$$
\boxed{\alpha=\frac{cq^2}{a}}.
$$

**Thus the conserved mode contains an order-one slaved nonconserved component, while the fast mode contains only an $O(q^2)$ conserved component.**

<h3 id="3/v">v</h3>

↑ **Parent:** [3](#3)

<h4 id="3/v/solution">Solution</h4>

↑ **Parent:** [V](#3/v)

Write $(\phi_q(0),0)^T=C_Be_B+C_Ae_A$. The equations $C_A=-\beta C_B$ and $\phi_q(0)=C_B(1-\alpha\beta)$ give

$$
f_1=\frac{C_B}{\phi_q(0)}=\frac1{1-\alpha\beta},
\qquad
f_2=\frac{\alpha C_A}{\phi_q(0)}
=\frac{-\alpha\beta}{1-\alpha\beta}.
$$

Since $\alpha\beta=-c^2q^2/a^2$,

$$
\boxed{f_1(q)=1-\frac{c^2q^2}{a^2}+O(q^4)},
\qquad
\boxed{f_2(q)=\frac{c^2q^2}{a^2}+O(q^4)}.
$$

Therefore $G_\phi=f_1e^{-\lambda_Bt}+f_2e^{-\lambda_At}$. At $q=0$, conservation makes $\phi_0$ exactly constant. Any nonzero overlap with the fast mode would change it on the finite timescale $a^{-1}$, so conservation requires $f_2\to0$; the explicit $q^2$ factor enforces this.

<h3 id="3/vi">vi</h3>

↑ **Parent:** [3](#3)

<h4 id="3/vi/solution">Solution</h4>

↑ **Parent:** [Vi](#3/vi)

At $|\mathbf q|=1$, let $s=a+\kappa$. The matrix is symmetric:

$$
R(1)=\begin{pmatrix}s&c\\c&s\end{pmatrix}.
$$

Its modes are

$$
\boxed{\lambda_-=s-c,\quad e_-=(1,-1)^T},
\qquad
\boxed{\lambda_+=s+c,\quad e_+=(1,1)^T}.
$$

Because $(1,0)^T=(e_-+e_+)/2$,

$$
\boxed{G_\phi(t)=\frac12e^{-(s-c)t}
+\frac12e^{-(s+c)t}=e^{-st}\cosh(ct)}.
$$

<h3 id="3/vii">vii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/vii/solution">Solution</h4>

↑ **Parent:** [Vii](#3/vii)

The second components of $e_-$ and $e_+$ have opposite signs. Therefore

$$
\boxed{\langle\psi_{\mathbf q}(t)\rangle
=\frac{\phi_{\mathbf q}(0)}2
\left[-e^{-(s-c)t}+e^{-(s+c)t}\right]
=-\phi_{\mathbf q}(0)e^{-st}\sinh(ct)}.
$$

<h3 id="3/viii">viii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/viii/solution">Solution</h4>

↑ **Parent:** [Viii](#3/viii)

For $|\mathbf q|=1$, the quadratic free-energy kernel is

$$
K=\begin{pmatrix}s&c\\c&s\end{pmatrix},
\qquad s=a+\kappa.
$$

The equilibrium covariance is $VK^{-1}$ under the Fourier normalization in the question. Since

$$
K^{-1}=\frac1{s^2-c^2}
\begin{pmatrix}s&-c\\-c&s\end{pmatrix},
$$

the steady cross-correlator is

$$
\boxed{\langle\psi_{\mathbf q}^*\phi_{\mathbf q}\rangle
=-\frac{Vc}{(a+\kappa)^2-c^2}}.
$$

If Fourier modes are normalized by $V^{-1/2}$, the factor $V$ is absent. The negative sign reflects the energetic preference for opposite signs when $c>0$.

## 4

↑ **Parent:** [Paper 353](paper-353.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/i">i</h4>

↑ **Parent:** [A](#4/a)

<h5 id="4/a/i/solution">Solution</h5>

↑ **Parent:** [I](#4/a/i)

For the [Poisson process](../../../probability-theory.md#poisson-process),

$$
G(\lambda)=\sum_{n=0}^\infty e^{\lambda n}
\frac{(\mu t)^n}{n!}e^{-\mu t}
=\boxed{\exp[\mu t(e^\lambda-1)]}.
$$

Differentiating at zero gives

$$
\boxed{\mathbb E N_t=\mu t},
\qquad
\boxed{\operatorname{Var}(N_t)=\mu t}.
$$

<h4 id="4/a/ii">ii</h4>

↑ **Parent:** [A](#4/a)

<h5 id="4/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#4/a/ii)

The scaled cumulant-generating function is

$$
\frac1t\log G(\lambda)=\mu(e^\lambda-1).
$$

By [Cramér theorem](../../../probability-theory.md#cramer-s-theorem), its Legendre transform is stationary at $e^{\lambda_*}=x/\mu$ for $x\geq0$. Thus

$$
\boxed{I(x)=x\log\frac x\mu-x+\mu},
\qquad x\geq0,
$$

with $I(x)=+\infty$ for $x<0$ and the continuous convention $0\log0=0$.

<h4 id="4/a/iii">iii</h4>

↑ **Parent:** [A](#4/a)

<h5 id="4/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#4/a/iii)

Assume $\mu_2>\mu_1$, so the upper tail is governed by its boundary. The [large deviation principle](../../../convergence-of-random-variables.md#large-deviation-principle) gives the exponentially equivalent estimate

$$
\boxed{\mathbb P(N_t/t\geq\mu_2)
\asymp e^{-tI(\mu_2)}},
$$

where now $I(x)=x\log(x/\mu_1)-x+\mu_1$. Increasing capacity to $\mu_3>\mu_2$ reduces this estimate by at least $10^6$ when

$$
\boxed{t[I(\mu_3)-I(\mu_2)]\geq6\log10}.
$$

Equivalently,

$$
\boxed{\mu_3\log\frac{\mu_3}{\mu_1}-\mu_3
-\mu_2\log\frac{\mu_2}{\mu_1}+\mu_2
\geq\frac{6\log10}{t}}.
$$

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/i">i</h4>

↑ **Parent:** [B](#4/b)

<h5 id="4/b/i/solution">Solution</h5>

↑ **Parent:** [I](#4/b/i)

A [Brownian motion](../../../brownian-motion.md) has independent stationary Gaussian increments, so

$$
\boxed{W_{t+h}-W_t\sim N(0,h)}.
$$

<h4 id="4/b/ii">ii</h4>

↑ **Parent:** [B](#4/b)

<h5 id="4/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#4/b/ii)

The increment law immediately gives

$$
\boxed{\mathbb E(W_{t+h}-W_t)^2=h}.
$$

The difference quotient has second moment

$$
\mathbb E\left(\frac{W_{t+h}-W_t}{h}\right)^2=\frac1h\to\infty.
$$

**Thus increments scale as $\sqrt h$, rather than $h$, and no finite derivative is suggested. In fact this heuristic is strengthened by the theorem on [nowhere differentiability of Brownian motion](../../../brownian-motion.md#nowhere-differentiability-of-brownian-motion).**

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/i">i</h4>

↑ **Parent:** [C](#4/c)

<h5 id="4/c/i/solution">Solution</h5>

↑ **Parent:** [I](#4/c/i)

Let $Q=(\sigma\sigma^T)^{-1}$ and use its induced inner product. The autonomous Lagrangian is

$$
L=\frac12\|\dot\phi-a\|^2.
$$

Its conserved Hamiltonian is

$$
H=\frac12(\|\dot\phi\|^2-\|a\|^2).
$$

On an infinite-duration fluctuation path $H=0$, so $\|\dot\phi\|=\|a\|$. Expanding the action then gives

$$
I=\int\left(\|\dot\phi\|^2-a\cdot\dot\phi\right)dt.
$$

Since metric arclength satisfies $ds=\|d\phi\|=\|\dot\phi\|dt=\|a\|dt$,

$$
\boxed{I[\phi]=\int_\phi\|a\|\,ds-a\cdot d\phi}.
$$

This is the [geometric minimum action](../../../convergence-of-random-variables.md#geometric-minimum-action) representation and is independent of the speed used to parametrize the path.

<h4 id="4/c/ii">ii</h4>

↑ **Parent:** [C](#4/c)

<h5 id="4/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#4/c/ii)

For constant isotropic diffusion and detailed balance, the drift has gradient form

$$
a=-M\nabla V
$$

for a positive scalar mobility $M$ after absorbing temperature and diffusion constants into $V$. Deterministic relaxation follows $a$ downhill. The least-action escape trajectory is its time reverse,

$$
\dot\phi=-a=M\nabla V.
$$

Its tangent is therefore parallel to $\nabla V$. Since the gradient is normal to every level set $V=\text{constant}$, the escape path from a local minimum crosses all equipotentials orthogonally.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2026](../../2026.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
