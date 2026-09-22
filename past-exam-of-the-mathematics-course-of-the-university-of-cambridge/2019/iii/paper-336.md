# Paper 336

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2019/paper_336.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2019/paper_336.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
    - [i](#1/b/i)
      - [Solution](#1/b/i/solution)
    - [ii](#1/b/ii)
      - [Solution](#1/b/ii/solution)
    - [iii](#1/b/iii)
      - [Solution](#1/b/iii/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)

## 1

↑ **Parent:** [Paper 336](paper-336.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

There are two positive roots for $u>1$: the [derivative](../../../calculus.md#derivative) of $xe^{1/x}$ is $e^{1/x}(1-1/x)$, so the function decreases to its minimum $e$ at $x=1$ and then increases. Negative $x$ cannot solve the equation. For the larger root, expansion of the [exponential function](../../../calculus.md#exponential-function) in $1/x$ gives

$$
xe^{1/x}=x+1+\frac1{2x}+O(x^{-2}),
$$

so [series reversion](../../../analysis.md#series-reversion) yields

$$
\boxed{x_{\rm large}=e^u-1+O(e^{-u}).}
$$

For the smaller root, set $y=1/x$ and take a [logarithm](../../../calculus.md#logarithm). Then $y-\log y=u$, so successive substitution gives $y=u+\log u+O(\log u/u)$ and

$$
\boxed{x_{\rm small}=\frac1u-\frac{\log u}{u^2}+O\left(\frac{(\log u)^2}{u^3}\right).}
$$

These are the first two nonzero terms of the two [asymptotic expansions](../../../analysis.md#asymptotic-expansion). Equivalently, the roots are $-1/W_0(-e^{-u})$ and $-1/W_{-1}(-e^{-u})$, from the [real branches of Lambert W](../../../analysis.md#real-branches-of-lambert-w).

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

The three fixed-$a$ estimates below cease to be uniform as the minimum of the phase approaches the endpoint. For the [cubic endpoint-to-saddle transition](../../../analysis.md#cubic-endpoint-to-saddle-transition), write

$$
a=1+l\nu^{-2/3},\qquad t=2^{1/3}\nu^{-1/3}s.
$$

The [Taylor series](../../../calculus.md#taylor-series) of the [hyperbolic sine](../../../calculus.md#hyperbolic-sine) gives, for bounded $s$ and fixed $l$,

$$
\nu(a\sinh t-t)=2^{1/3}ls+\frac{s^3}3+O(\nu^{-2/3}).
$$

The cubic term controls the tail, so localization of the [Laplace integral](../../../analysis.md#laplace-integral) gives the uniform leading formula

$$
\boxed{A_\nu(\nu+l\nu^{1/3})\sim2^{1/3}\nu^{-1/3}I(-2^{1/3}l),\qquad I(x)=\int_0^\infty e^{xs-s^3/3}\,ds.}
$$

Here $I$ is the [cubic Laplace transition integral](../../../analysis.md#cubic-laplace-transition-integral), equal to $\pi\operatorname{Hi}$ in terms of the [Scorer Hi function](../../../analysis.md#scorer-hi-function).

To recover the endpoint regime, let $l\to+\infty$. Scale $s=v/(2^{1/3}l)$ in $I$; the cubic term becomes negligible and $I(-2^{1/3}l)\sim(2^{1/3}l)^{-1}$. Therefore

$$
A_\nu\sim\frac{\nu^{-1/3}}l=\frac1{\nu(a-1)},
$$

which agrees with part (i) in the overlap $1\ll l\ll\nu^{2/3}$. At $l=0$, the [Gamma integral](../../../complex-analysis.md#gamma-integral) gives $I(0)=3^{-2/3}\Gamma(1/3)$, recovering part (iii).

For $l\to-\infty$, set $M=-2^{1/3}l>0$. The exponent $Ms-s^3/3$ has its maximum at $s=\sqrt M$, with second [derivative](../../../calculus.md#derivative) $-2\sqrt M$. Thus [Laplace's method](../../../analysis.md#laplace-s-method) gives

$$
I(M)\sim\sqrt\pi M^{-1/4}e^{2M^{3/2}/3},
$$

and the transition formula becomes

$$
A_\nu\sim2^{1/4}\sqrt\pi\nu^{-1/3}(-l)^{-1/4}\exp\left[\frac{2\sqrt2}3(-l)^{3/2}\right].
$$

For $a=1-\eta$ with $\eta\downarrow0$, part (ii) has

$$
\operatorname{arcosh}(1/a)-\sqrt{1-a^2}=\frac{2\sqrt2}3\eta^{3/2}+O(\eta^{5/2}),\qquad (1-a^2)^{-1/4}\sim(2\eta)^{-1/4}.
$$

Putting $\eta=(-l)\nu^{-2/3}$ reproduces both the exponential and its prefactor. For relative agreement of these leading exponentials, one may use the overlap $1\ll-l\ll\nu^{4/15}$, which makes $\nu\eta^{5/2}\to0$. Thus the same transition integral connects all three regimes.

<a id="1/b/image-the-cubic-endpoint-to-saddle-transition"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-336-cubic-transition.png)

**[Figure 1](#1/b/image-the-cubic-endpoint-to-saddle-transition). The cubic endpoint-to-saddle transition**. Direct numerical integration of the original phase approaches the same cubic transition function as the large parameter increases. Negative transition parameter places the minimum inside the interval; positive parameter leaves an ordinary endpoint minimum.

<h4 id="1/b/i">i</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/i/solution">Solution</h5>

↑ **Parent:** [I](#1/b/i)

Let $S(t)=a\sinh t-t$. For $a>1$, $S'(t)=a\cosh t-1>0$ on the integration interval, so its minimum is the endpoint $t=0$. The [Taylor series](../../../calculus.md#taylor-series) is

$$
S(t)=(a-1)t+\frac a6t^3+O(t^5).
$$

On the contributing scale $t=O(\nu^{-1})$, the higher terms are negligible. The endpoint form of [Laplace's method](../../../analysis.md#laplace-s-method), or the [Watson lemma](../../../analysis.md#watson-s-lemma), therefore gives

$$
\boxed{A_\nu(a\nu)\sim\int_0^\infty e^{-\nu(a-1)t}\,dt=\frac1{\nu(a-1)}.}
$$

<h4 id="1/b/ii">ii</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/b/ii)

For $0<a<1$, the phase has an interior minimum at

$$
t_*=\operatorname{arcosh}(1/a),\qquad \sinh t_*=\frac{\sqrt{1-a^2}}a.
$$

The [inverse hyperbolic cosine](../../../calculus.md#inverse-hyperbolic-cosine) selects the positive [stationary point](../../../calculus-of-variations.md#stationary-point). At this point,

$$
S(t_*)=\sqrt{1-a^2}-\operatorname{arcosh}(1/a),\qquad S''(t_*)=\sqrt{1-a^2}>0.
$$

Expanding the phase to second order and evaluating the resulting [Gaussian integral](../../../calculus.md#gaussian-integral) by [Laplace's method](../../../analysis.md#laplace-s-method) yields

$$
\boxed{A_\nu(a\nu)\sim\sqrt{\frac{2\pi}{\nu\sqrt{1-a^2}}}\exp\left\{\nu\left[\operatorname{arcosh}(1/a)-\sqrt{1-a^2}\right]\right\}.}
$$

The exponential grows because the minimum of $S$ is negative; the original integral remains convergent because $a\sinh t$ dominates $t$ at infinity.

<h4 id="1/b/iii">iii</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#1/b/iii)

At $a=1$, the endpoint is degenerate: $S(t)=\sinh t-t=t^3/6+O(t^5)$. The contributing width is therefore $t=O(\nu^{-1/3})$, rather than the width in part (i). With $v=\nu t^3/6$, the formula for a [degenerate endpoint in Laplace's method](../../../analysis.md#degenerate-endpoint-in-laplace-s-method) gives

$$
\boxed{A_\nu(\nu)\sim\int_0^\infty e^{-\nu t^3/6}\,dt=\frac{6^{1/3}}{3\nu^{1/3}}\Gamma(1/3).}
$$

The coefficient is a [Gamma function](../../../complex-analysis.md#gamma-function) value obtained by the [Gamma integral](../../../complex-analysis.md#gamma-integral).

## 2

↑ **Parent:** [Paper 336](paper-336.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

At fixed $r$, the leading equation is $(r^2f_0')'=0$. Its solution compatible with the eventual decaying far field and the boundary value at one is $f_0=1/r$. This decay implies $f=O(\epsilon)$ at distances $r=O(\epsilon^{-1})$. Balancing radial [derivatives](../../../calculus.md#derivative) against the linear screening term identifies

$$
\boxed{\beta=1,\qquad x=\epsilon r.}
$$

The distant region is governed by the [modified Helmholtz equation](../../../partial-differential-equation.md#modified-helmholtz-equation); its decaying homogeneous profile is $e^{-x}/x$.

For a [matched asymptotic expansion](../../../differential-equation.md#matched-asymptotic-expansion), write the fixed-$r$ approximation as $f=f_0+\epsilon f_1+\epsilon^2f_2+\cdots$, allowing logarithms of $\epsilon$ in the coefficients. Successive equations are

$$
(r^2f_0')'=0,\qquad (r^2f_1')'=0,\qquad (r^2f_2')'=r+1.
$$

The boundary condition imposes $f_0(1)=1$ and $f_1(1)=f_2(1)=0$. Before matching, their integrated forms can be written

$$
f_0=\frac1r,\qquad f_1=C_1\left(1-\frac1r\right),\qquad f_2=\frac r2+\log r+D-\frac{D+1/2}{r}.
$$

In particular a pure power series with parameter-independent coefficients will be insufficient: the [logarithmic overlap creates a switchback term](../../../differential-equation.md#logarithmic-overlap-creates-a-switchback-term).

In the distant region set $f=\epsilon F_0(x)+\epsilon^2F_1(x)+\cdots$. The scaled equation is $f_{xx}+2f_x/x-f=xf^3/\epsilon$, so

$$
F_0''+\frac2xF_0'-F_0=0,\qquad F_1''+\frac2xF_1'-F_1=\frac{e^{-3x}}{x^2}.
$$

Decay and leading matching give $F_0=e^{-x}/x$. The [radial modified Helmholtz equation](../../../partial-differential-equation.md#radial-modified-helmholtz-equation) gives the supplied particular integral in terms of the [exponential integral](../../../complex-analysis.md#exponential-integral):

$$
F_1(x)=\alpha\frac{e^{-x}}x+\frac{e^{-x}E_1(2x)-e^xE_1(4x)}{2x}.
$$

As $x\downarrow0$, the [small-argument expansion of the exponential integral](../../../complex-analysis.md#small-argument-expansion-of-the-exponential-integral) yields

$$
F_1(x)=\frac{\alpha+\tfrac12\log2}{x}+\log x-\alpha+\tfrac32\log2+\gamma-1+O(x\log x),
$$

where $\gamma$ is the [Euler--Mascheroni constant](../../../complex-analysis.md#euler-s-constant). Substitute $x=\epsilon r$ to compare the two expansions in $1\ll r\ll\epsilon^{-1}$:

$$
\epsilon F_0+\epsilon^2F_1=\frac1r-\epsilon+\epsilon^2\frac r2+\frac{\epsilon}{r}\left(\alpha+\tfrac12\log2\right)+\epsilon^2\left[\log r+\log\epsilon-\alpha+\tfrac32\log2+\gamma-1\right]+\cdots.
$$

The constant at order $\epsilon$ fixes $C_1=-1$. Its $1/r$ coefficient then fixes $\alpha+\tfrac12\log2=1$, and the constant at order $\epsilon^2$ fixes $D$. Hence

$$
\boxed{\alpha=1-\tfrac12\log2,\qquad D=\log\epsilon+2\log2+\gamma-2.}
$$

The required [inner expansion](../../../differential-equation.md#inner-expansion) at fixed $r$ is

$$
\boxed{f=\frac1r+\epsilon\left(\frac1r-1\right)+\epsilon^2\left[\frac{r-r^{-1}}2+\log r+\left(\log\epsilon+2\log2+\gamma-2\right)\left(1-\frac1r\right)\right]+o(\epsilon^2).}
$$

At fixed positive $x=\epsilon r$, the [outer expansion](../../../differential-equation.md#outer-expansion) is

$$
\boxed{f=\epsilon\frac{e^{-x}}x+\epsilon^2\left[\left(1-\tfrac12\log2\right)\frac{e^{-x}}x+\frac{e^{-x}E_1(2x)-e^xE_1(4x)}{2x}\right]+o(\epsilon^2).}
$$

Both display every term through the requested order, including the $\epsilon^2\log\epsilon$ [switchback term](../../../differential-equation.md#switchback-term) in the fixed-$r$ region.

To form an [additive composite expansion](../../../differential-equation.md#additive-composite-expansion), subtract the common overlap from the sum of the inner and outer expressions. Their retained common part is

$$
f_{\rm overlap}=\frac1r+\epsilon\left(\frac1r-1\right)+\epsilon^2\left[\frac r2+\log r+D\right].
$$

Thus one composite is $\epsilon F_0(\epsilon r)+\epsilon^2F_1(\epsilon r)-\epsilon^2(D+1/2)/r$. The last term can be screened by multiplying it by $e^{-\epsilon r}$ without changing either retained expansion. This gives a useful exponentially decaying version:

$$
\boxed{f_{\rm comp}(r)=\frac{e^{-\epsilon r}}r\left[1-\epsilon^2(D+1/2)\right]+\epsilon^2F_1(\epsilon r).}
$$

Its boundary value is $1+o(\epsilon^2)$. If exact satisfaction of the boundary value is desired, use instead

$$
f_{\rm comp}^{\rm normalized}(r)=\left[1-\epsilon^2F_1(\epsilon)\right]\frac{e^{-\epsilon(r-1)}}r+\epsilon^2F_1(\epsilon r).
$$

The [small-argument expansion of the exponential integral](../../../complex-analysis.md#small-argument-expansion-of-the-exponential-integral) shows that this normalized composite has the same two retained expansions; it equals one at $r=1$ and tends to zero at infinity.

## 3

↑ **Parent:** [Paper 336](paper-336.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

The linear [dispersion relation](../../../wave-equation.md#dispersion-relation) for a mode $e^{i(kx-\omega t)}$ is $5\omega^2=k^4+4$. The proposed modes share [phase velocity](../../../wave-equation.md#phase-velocity) $c$, so $5c^2k_j^2=k_j^4+4$. A [quadratic wave interaction](../../../differential-equation.md#quadratic-wave-interaction) generates the second harmonic and the difference harmonic. With only two positive [wavenumbers](../../../wave-equation.md#wavenumber), [phase matching for a quadratic wave interaction](../../../differential-equation.md#phase-matching-for-a-quadratic-wave-interaction) requires $k_2=2k_1$. Equating their phase velocities gives

$$
k_1^2+\frac4{k_1^2}=4k_1^2+\frac1{k_1^2},
$$

and therefore

$$
\boxed{k_1=1,\qquad k_2=2,\qquad c=1.}
$$

This is a [two-to-one resonance of dispersive waves](../../../differential-equation.md#two-to-one-resonance-of-dispersive-waves). Its amplitude changes accumulate on $t=O(\epsilon^{-1})$. Choose the [slow time](../../../differential-equation.md#slow-time) $T=\epsilon t/5$; this harmless constant rescaling makes the later amplitude formulas simple. With $\xi=x-t$, the leading real field is $A_0e^{i\xi}+B_0e^{2i\xi}+\overline A_0e^{-i\xi}+\overline B_0e^{-2i\xi}$.

For the fundamental, the order-$\epsilon$ cross derivative in $5\psi_{tt}$ is $-2i(A_0)_T e^{i\xi}$, while the fundamental coefficient in $\psi_0\psi_{0x}$ is $i\overline A_0B_0$. For the second harmonic the corresponding terms are $-4i(B_0)_T e^{2i\xi}$ and $iA_0^2$. The [solvability condition in the method of multiple scales](../../../differential-equation.md#solvability-condition-in-the-method-of-multiple-scales) removes the resonant forcing and gives

$$
\boxed{(A_0)_T=-\frac12\overline A_0B_0,\qquad (B_0)_T=-\frac14A_0^2.}
$$

The nonresonant third and fourth harmonics enter the correction. They do not change these leading [amplitude equations](../../../dynamical-systems.md#amplitude-equation).

Write $A_0=Re^{i\theta}$, $B_0=Pe^{i\phi}$ and $\delta=\phi-2\theta$. Taking real and imaginary parts gives the [explosive two-to-one amplitude system](../../../differential-equation.md#explosive-two-to-one-amplitude-system) in polar form:

$$
\boxed{R_T=-\frac{RP}2\cos\delta,\qquad \theta_T=-\frac P2\sin\delta,\qquad P_T=-\frac{R^2}4\cos\delta,\qquad \phi_T=\frac{R^2}{4P}\sin\delta.}
$$

The polar phases are used where their corresponding amplitudes are nonzero. These equations imply

$$
(R^2-2P^2)_T=0,\qquad (R^2P\sin\delta)_T=0.
$$

For the second identity, differentiate using $\delta_T=(R^2/(4P)+P)\sin\delta$: the terms proportional to $\sin\delta\cos\delta$ cancel. Therefore

$$
R^2\theta_T=-\frac12R^2P\sin\delta,\qquad P^2\phi_T=\frac14R^2P\sin\delta
$$

are [first integrals](../../../differential-equation.md#first-integral), and in particular

$$
\boxed{(R^2\theta_T)_T=0,\qquad(P^2\phi_T)_T=0.}
$$

For constant phases with $\phi=2\theta+\pi$, these real equations reduce to $R_T=RP/2$ and $P_T=R^2/4$. The initial data give $R^2-2P^2=8$, so the [Riccati equation](../../../analysis.md#riccati-equation) for $P$ is $2P_T=P^2+4$. Integrating and using $P(0)=2$ gives

$$
\boxed{P(T)=2\tan(T+\pi/4),\qquad R(T)=2\sqrt2\sec(T+\pi/4),\qquad 0\leq T<\pi/4.}
$$

The [tangent](../../../geometry-and-topology.md#tangent) and [secant function](../../../geometry-and-topology.md#secant-trigonometry) have a pole at $T=\pi/4$, corresponding to $t=5\pi/(4\epsilon)$. Both modes grow through their locked resonant interaction. This is formal [finite-time blowup](../../../differential-equation.md#finite-time-blowup) of the reduced [amplitude equations](../../../dynamical-systems.md#amplitude-equation); the [weakly nonlinear expansion](../../../differential-equation.md#weakly-nonlinear-expansion) loses validity as the amplitudes become large, so it cannot establish a singularity of the full partial differential equation.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Interpret the displayed two-harmonic form as a leading term in a [weakly nonlinear expansion](../../../differential-equation.md#weakly-nonlinear-expansion). Write $\xi=(1+\epsilon\kappa)x-t$ and $\Psi_0=\alpha\cos\xi+\beta\cos2\xi$. The linear operator multiplies $\cos m\xi$ by

$$
m^4(1+\epsilon\kappa)^4-5m^2+4.
$$

For $m=1,2$, this is $4\epsilon\kappa+O(\epsilon^2)$ and $64\epsilon\kappa+O(\epsilon^2)$, respectively. Thus [detuning of a wave resonance](../../../differential-equation.md#detuning-of-a-wave-resonance) enters at the same order as the quadratic forcing. The [cosine addition formula](../../../geometry-and-topology.md#cosine-addition-formula) gives

$$
\Psi_0^2=\frac{\alpha^2+\beta^2}2+\alpha\beta\cos\xi+\frac{\alpha^2}2\cos2\xi+\alpha\beta\cos3\xi+\frac{\beta^2}2\cos4\xi.
$$

Projection onto the two resonant harmonics by [harmonic balance](../../../differential-equation.md#harmonic-balance) requires

$$
4\kappa\alpha=\alpha\beta,\qquad64\kappa\beta=\frac{\alpha^2}2.
$$

The nonzero branches are therefore

$$
\boxed{\beta(\kappa)=4\kappa,\qquad\alpha(\kappa)=\pm16\sqrt2\,\kappa.}
$$

The two signs are related by a half-period translation of $\xi$; the trivial branch $\alpha=\beta=0$ also exists.

The nonresonant first correction supplies the generated mean, third harmonic and fourth harmonic. Their linear multipliers at $\epsilon=0$ are $4,40,180$, giving the nonresonant part

$$
\Psi_1^{\rm nonres}=\frac{\alpha^2+\beta^2}8+\frac{\alpha\beta}{40}\cos3\xi+\frac{\beta^2}{360}\cos4\xi.
$$

Further resonant amplitude corrections are determined at higher order. Consequently the nonzero answer describes an asymptotic periodic [travelling wave](../../../analysis.md#travelling-wave) with additional harmonics. Literally retaining only the two displayed harmonics cannot be an exact nonzero solution: their square has a positive constant term, while the linear operator applied to the two cosines has no constant term. The distinction is essential to interpreting this perturbative ansatz.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2019](../../2019.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
