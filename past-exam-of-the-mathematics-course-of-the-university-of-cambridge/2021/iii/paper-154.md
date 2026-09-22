# Paper 154

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2021/paper_154.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2021/paper_154.pdf)

**Table of contents**

- [1](#1)
  - [1](#1/1)
    - [Solution](#1/1/solution)
  - [2](#1/2)
    - [Solution](#1/2/solution)
  - [3](#1/3)
    - [Solution](#1/3/solution)
  - [4](#1/4)
    - [Solution](#1/4/solution)
  - [5](#1/5)
    - [Solution](#1/5/solution)
- [2](#2)
  - [1](#2/1)
    - [Solution](#2/1/solution)
  - [2](#2/2)
    - [Solution](#2/2/solution)
  - [3](#2/3)
    - [Solution](#2/3/solution)
  - [4](#2/4)
    - [Solution](#2/4/solution)
- [3](#3)
  - [1](#3/1)
    - [Solution](#3/1/solution)
  - [2](#3/2)
    - [Solution](#3/2/solution)
  - [3](#3/3)
    - [Solution](#3/3/solution)
  - [4](#3/4)
    - [Solution](#3/4/solution)
  - [5](#3/5)
    - [Solution](#3/5/solution)

## 1

↑ **Parent:** [Paper 154](paper-154.md)

<h3 id="1/1">1</h3>

↑ **Parent:** [1](#1)

<h4 id="1/1/solution">Solution</h4>

↑ **Parent:** [1](#1/1)

Write the [Generalized Korteweg–De Vries equation](../../../nonlinear-analysis.md#generalized-korteweg-de-vries-equation) as

$$
u_t=-\partial_x(u_{xx}+u^p).
$$

For a sufficiently regular solution, [integration by parts](../../../calculus.md#integration-by-parts) gives

$$
\frac d{dt}\int_{\mathbb R}u^2\,dx
=-2\int_{\mathbb R}u\,\partial_x(u_{xx}+u^p)\,dx
=2\int_{\mathbb R}u_xu_{xx}\,dx
+2\int_{\mathbb R}u^pu_x\,dx=0.
$$

Thus [KdV mass conservation](../../../nonlinear-analysis.md#kdv-mass-and-energy-conservation) gives

$$
\boxed{\|u(t)\|_2=\|u_0\|_2}
$$

is conserved.

<h3 id="1/2">2</h3>

↑ **Parent:** [1](#1)

<h4 id="1/2/solution">Solution</h4>

↑ **Parent:** [2](#1/2)

Differentiate the proposed energy and integrate the kinetic term by parts:

$$
\frac d{dt}E(u(t))
=\int_{\mathbb R}(-u_{xx}-u^p)u_t\,dx.
$$

Putting $F=u_{xx}+u^p$, the equation says $u_t=-F_x$, so

$$
\frac d{dt}E(u(t))
=\int_{\mathbb R}F F_x\,dx
=\frac12\int_{\mathbb R}\partial_x(F^2)\,dx=0.
$$

Hence [KdV energy conservation](../../../nonlinear-analysis.md#kdv-mass-and-energy-conservation) gives

$$
\boxed{E(u(t))=E(u_0)}.
$$

<h3 id="1/3">3</h3>

↑ **Parent:** [1](#1)

<h4 id="1/3/solution">Solution</h4>

↑ **Parent:** [3](#1/3)

The one-dimensional [Gagliardo-Nirenberg interpolation inequality](../../../sobolev-space.md#gagliardo-nirenberg-interpolation-inequality) yields

$$
\|u\|_{p+1}^{p+1}
\leq C_p\|u_x\|_2^{(p-1)/2}\|u\|_2^{(p+3)/2}.
$$

Mass conservation fixes $\|u\|_2$. If $X=\|u_x\|_2$, energy conservation therefore gives

$$
E(u_0)
\geq\frac12X^2-C(u_0)X^{(p-1)/2}.
$$

For $p<5$, the second exponent is strictly smaller than two. The right side tends to infinity with $X$, so this inequality bounds $X$ uniformly throughout the lifespan. The conserved $L^2$ norm then bounds $\|u(t)\|_{H^1}$. The stated blowup criterion rules out a finite endpoint, proving [Global existence for the energy-subcritical generalized KdV equation](../../../nonlinear-analysis.md#global-existence-for-the-energy-subcritical-generalized-kdv-equation).

<h3 id="1/4">4</h3>

↑ **Parent:** [1](#1)

<h4 id="1/4/solution">Solution</h4>

↑ **Parent:** [4](#1/4)

Set $z=x-ct$ and $u(t,x)=Q_c(z)$. Substitution into the equation gives

$$
\partial_z(Q_c''-cQ_c+Q_c^p)=0.
$$

Decay at infinity makes the integration constant zero. If

$$
Q_c(x)=c^{1/(p-1)}Q(\sqrt c\,x),
$$

then every term in $Q_c''-cQ_c+Q_c^p$ equals $c^{1+1/(p-1)}$ times the corresponding term in $Q''-Q+Q^p$. Thus the required [Generalized KdV solitary wave](../../../nonlinear-analysis.md#generalized-kdv-solitary-wave) is

$$
\boxed{Q_c(x)=c^{1/(p-1)}Q(\sqrt c\,x)}.
$$

<h3 id="1/5">5</h3>

↑ **Parent:** [1](#1)

<h4 id="1/5/solution">Solution</h4>

↑ **Parent:** [5](#1/5)

For every $p<5$, the wave $Q_c$ has [Orbital stability of a generalized KdV solitary wave](../../../nonlinear-analysis.md#orbital-stability-of-a-generalized-kdv-solitary-wave) in $H^1(\mathbb R)$ modulo translation: for every $\varepsilon>0$ there is $\delta>0$ such that

$$
\|u_0-Q_c\|_{H^1}<\delta
\quad\Longrightarrow\quad
\sup_t\inf_{y\in\mathbb R}
\|u(t)-Q_c(\,\cdot-y)\|_{H^1}<\varepsilon.
$$

The relevant stability slope has the correct sign because scaling gives

$$
\|Q_c\|_2^2
=c^{2/(p-1)-1/2}\|Q\|_2^2
=c^{(5-p)/(2(p-1))}\|Q\|_2^2,
$$

which is strictly increasing in $c$ precisely for $p<5$. Together with the constrained variational characterization of $Q_c$, the conserved mass and energy provide a coercive [Lyapunov function](../../../dynamical-systems.md#lyapunov-function) transverse to the translation direction.

<h2 id="2">2</h2>

↑ **Parent:** [Paper 154](paper-154.md)

<h3 id="2/1">1</h3>

↑ **Parent:** [2](#2)

<h4 id="2/1/solution">Solution</h4>

↑ **Parent:** [1](#2/1)

The [Gravitational Hartree equation](../../../nonlinear-analysis.md#gravitational-hartree-equation) can be written

$$
u_t=i\Delta u-i\phi u,
$$

where $\phi$ is real. Consequently

$$
\frac d{dt}\int_{\mathbb R^N}|u|^2\,dx
=2\operatorname{Re}\int_{\mathbb R^N}u_t\overline u\,dx
=2\operatorname{Re}\left(
i\int\Delta u\,\overline u-i\int\phi|u|^2
\right)=0,
$$

because both integrals multiplied by $i$ are purely imaginary after [integration by parts](../../../calculus.md#integration-by-parts). Hence [Hartree mass conservation](../../../nonlinear-analysis.md#hartree-mass-and-energy-conservation) holds.

<h3 id="2/2">2</h3>

↑ **Parent:** [2](#2)

<h4 id="2/2/solution">Solution</h4>

↑ **Parent:** [2](#2/2)

Since $\Delta\phi=|u|^2$, integration by parts gives

$$
\int|\nabla\phi|^2=-\int\phi|u|^2.
$$

The Newtonian convolution operator is [self-adjoint](../../../linear-operator-theory.md#self-adjoint-operator), so differentiating this identity symmetrically gives

$$
\frac d{dt}\int|\nabla\phi|^2
=-2\int\phi\,\partial_t|u|^2.
$$

It follows that

$$
\begin{aligned}
\frac d{dt}E(u)
&=-\operatorname{Re}\int\Delta u\,\overline{u_t}
+\frac12\int\phi\,\partial_t|u|^2\\
&=\operatorname{Re}\int(-\Delta u+\phi u)\overline{u_t}.
\end{aligned}
$$

The equation says $-\Delta u+\phi u=i u_t$, and therefore the final real part is $\operatorname{Re}\int i|u_t|^2=0$. This proves [Hartree energy conservation](../../../nonlinear-analysis.md#hartree-mass-and-energy-conservation).

<h3 id="2/3">3</h3>

↑ **Parent:** [2](#2)

<h4 id="2/3/solution">Solution</h4>

↑ **Parent:** [3](#2/3)

In three dimensions, the [Hardy–Littlewood–Sobolev inequality](../../../nonlinear-analysis.md#hardy-littlewood-sobolev-inequality) applied to the Newtonian kernel gives

$$
\int_{\mathbb R^3}|\nabla\phi|^2
=-\int\phi|u|^2
\lesssim\||u|^2\|_{6/5}^2
=\|u\|_{12/5}^4.
$$

The [Gagliardo-Nirenberg interpolation inequality](../../../sobolev-space.md#gagliardo-nirenberg-interpolation-inequality) then gives

$$
\|u\|_{12/5}^4
\lesssim\|u\|_2^3\|\nabla u\|_2.
$$

Writing $X=\|\nabla u\|_2$ and using the conserved mass, conservation of energy implies

$$
E(u_0)\geq\frac12X^2-C(u_0)X.
$$

**Thus $X$ remains bounded. Together with the conserved $L^2$ norm this bounds $\|u(t)\|_{H^1}$, and the supplied blowup criterion proves [Global H1 solutions of the three-dimensional gravitational Hartree equation](../../../nonlinear-analysis.md#global-h1-solutions-of-the-three-dimensional-gravitational-hartree-equation).**

<h3 id="2/4">4</h3>

↑ **Parent:** [2](#2)

<h4 id="2/4/solution">Solution</h4>

↑ **Parent:** [4](#2/4)

Let

$$
I(t)=\int_{\mathbb R^4}|x|^2|u(t,x)|^2\,dx.
$$

The first [virial identity](../../../nonlinear-analysis.md#virial-identity), obtained from the equation by integration by parts, is

$$
I'(t)=4\operatorname{Im}\int_{\mathbb R^4}\overline u\,x\mathbin{\cdot}\nabla u\,dx.
$$

Differentiating once more gives

$$
I''(t)=8\int|\nabla u|^2-4\int x\mathbin{\cdot}\nabla\phi\,|u|^2.
$$

Write $\phi=W*|u|^2$, where $W(x)=-1/(C_4|x|^2)$ is homogeneous of degree $-2$. Symmetrizing the double integral and applying Euler's identity $z\cdot\nabla W(z)=-2W(z)$ yields

$$
\int x\mathbin{\cdot}\nabla\phi(x)|u(x)|^2\,dx
=-\int\phi|u|^2
=\int|\nabla\phi|^2.
$$

Therefore

$$
\boxed{I''(t)
=8\int|\nabla u|^2-4\int|\nabla\phi|^2
=16E(u)}.
$$

Not all solutions are global. Choose smooth finite-variance data of negative energy, which is possible by multiplying any nonzero test function by a sufficiently large constant: the kinetic term is quadratic in the amplitude and the attractive potential term is quartic. If such a solution were global, the [Virial identity for the four-dimensional gravitational Hartree equation](../../../nonlinear-analysis.md#virial-identity-for-the-four-dimensional-gravitational-hartree-equation) would make the nonnegative function $I(t)$ strictly concave with constant negative second derivative, forcing it below zero in finite time. The solution must therefore blow up in finite time.

<h2 id="3">3</h2>

↑ **Parent:** [Paper 154](paper-154.md)

<h3 id="3/1">1</h3>

↑ **Parent:** [3](#3)

<h4 id="3/1/solution">Solution</h4>

↑ **Parent:** [1](#3/1)

Let

$$
\Sigma=\{u\in H^1(\mathbb R^2):|x|u\in L^2(\mathbb R^2)\}
$$

be the [harmonic-oscillator energy space](../../../nonlinear-analysis.md#harmonic-oscillator-energy-space), and denote the minimized quadratic functional by $J(u)$. A minimizing sequence $(u_n)\subset\mathcal A(M)$ is bounded in $\Sigma$, because $J$ is its squared Hilbert norm with positive coefficients. After taking a subsequence, $u_n\rightharpoonup u$ weakly in $\Sigma$.

The embedding $\Sigma\hookrightarrow L^4(\mathbb R^2)$ is compact. On any fixed ball this follows from the [Rellich-Kondrachov compactness theorem](../../../sobolev-space.md#rellich-kondrachov-theorem). Outside a large ball, the moment bound makes the $L^2$ tail uniformly small, and interpolation with the uniform $H^1\hookrightarrow L^q$ bounds for some $q>4$ makes the $L^4$ tail uniformly small. Hence $u_n\to u$ strongly in $L^4$.

The constraint passes to the limit, so $\int|u|^4=M$. Weak lower semicontinuity gives $J(u)\leq\liminf J(u_n)=I(M)$. Therefore $u$ attains the infimum. This is [Fixed-L4 minimization in the harmonic-oscillator energy space](../../../nonlinear-analysis.md#fixed-l4-minimization-in-the-harmonic-oscillator-energy-space).

<h3 id="3/2">2</h3>

↑ **Parent:** [3](#3)

<h4 id="3/2/solution">Solution</h4>

↑ **Parent:** [2](#3/2)

Replacing a minimizer by its absolute value does not increase its gradient norm, so choose a nonnegative minimizer $P$. The [Euler-Lagrange equation](../../../analysis.md#euler-lagrange-equation) is

$$
-\Delta P+P+\frac\eta4|x|^2P=\mu P^3
$$

for a [Lagrange multiplier](../../../mathematical-optimization.md#lagrange-multiplier) $\mu$. Multiplication by $P$ and integration show that

$$
\mu M=\int|\nabla P|^2+\int|P|^2+\frac\eta4\int|x|^2|P|^2>0,
$$

so $\mu>0$. Set $P_\eta=\sqrt\mu P$. Then $P_\eta$ is nonzero, belongs to $H^1(\mathbb R^2)$, and satisfies the [trapped focusing cubic ground-state equation](../../../nonlinear-analysis.md#trapped-focusing-cubic-ground-state-equation)

$$
\boxed{\Delta P_\eta-P_\eta-\frac\eta4|x|^2P_\eta+P_\eta^3=0}.
$$

Standard elliptic regularity and the [strong minimum principle for elliptic operators](../../../elliptic-boundary-value-problem.md#strong-minimum-principle-for-elliptic-operators) make the nonnegative solution positive.

<h3 id="3/3">3</h3>

↑ **Parent:** [3](#3)

<h4 id="3/3/solution">Solution</h4>

↑ **Parent:** [3](#3/3)

From $b_s+b^2=-\eta$ one obtains

$$
\frac d{ds}\sqrt{b^2+\eta}
=\frac{bb_s}{\sqrt{b^2+\eta}}
=-b\sqrt{b^2+\eta}.
$$

Since $\lambda_s=-b\lambda$, the ratio $\sqrt{b^2+\eta}/\lambda$ is constant. Its value at $t=-1$ is one, so

$$
b^2+\eta=\lambda^2.
$$

Using $s_t=\lambda^{-2}$ and $\lambda_s=-b\lambda$ gives

$$
\lambda_t=-\frac b\lambda,
\qquad
b_t=-\frac{b^2+\eta}{\lambda^2}=-1.
$$

The initial conditions now give

$$
\boxed{b_\eta(t)=-t,
\qquad \lambda_\eta(t)=\sqrt{t^2+\eta}}.
$$

Finally,

$$
s(t)-s(-1)
=\int_{-1}^t\frac{d\tau}{\tau^2+\eta}
=\frac1{\sqrt\eta}
\left(\arctan\frac t{\sqrt\eta}
+\arctan\frac1{\sqrt\eta}\right).
$$

These are the [explicit lens parameters](../../../nonlinear-analysis.md#explicit-expanding-focusing-schrodinger-lens).

<h3 id="3/4">4</h3>

↑ **Parent:** [3](#3)

<h4 id="3/4/solution">Solution</h4>

↑ **Parent:** [4](#3/4)

Substitute the [Focusing Schrödinger lens ansatz](../../../nonlinear-analysis.md#focusing-schrodinger-lens-ansatz) into

$$
i u_t+\Delta u+|u|^2u=0.
$$

The imaginary terms proportional to $P_\eta+y\cdot\nabla P_\eta$ cancel because $b=-\lambda\lambda_t$. After multiplying the remaining real equation by $\lambda^3$, one obtains

$$
\Delta P_\eta+P_\eta^3
-\lambda^2\gamma_tP_\eta
+\frac{\lambda^2b_t+b^2}{4}|y|^2P_\eta=0.
$$

The dynamical system gives $\lambda^2b_t+b^2=-\eta$. Comparison with the equation for $P_\eta$ therefore requires

$$
\gamma_\eta'(t)=\frac1{\lambda_\eta(t)^2}
=\frac1{t^2+\eta}.
$$

Thus, up to an arbitrary constant phase,

$$
\boxed{\gamma_\eta(t)
=\gamma_\eta(-1)
+\frac1{\sqrt\eta}
\left(\arctan\frac t{\sqrt\eta}
+\arctan\frac1{\sqrt\eta}\right)}.
$$

<h3 id="3/5">5</h3>

↑ **Parent:** [3](#3)

<h4 id="3/5/solution">Solution</h4>

↑ **Parent:** [5](#3/5)

For $T_2>T_1\geq-1$, the dual [Strichartz estimate for the free Schrödinger equation](../../../nonlinear-analysis.md#strichartz-estimate-for-the-free-schrodinger-equation) gives

$$
\left\|
\int_{T_1}^{T_2}S(-s)(u_\eta|u_\eta|^2)(s)\,ds
\right\|_2
\lesssim
\|u_\eta|u_\eta|^2\|_{L^{4/3}_{t,x}([T_1,T_2])}
=\|u_\eta\|_{L^4_{t,x}([T_1,T_2])}^3.
$$

The assumed finite global $L^4_{t,x}$ norm makes the right side tend to zero as $T_1,T_2\to\infty$. The displayed family is therefore a [Cauchy sequence](../../../real-analysis.md#cauchy-sequence) in the complete space $L^2$ and has a strong limit $F_\infty$.

The [Duhamel principle](../../../diffusion-equation.md#duhamel-s-principle) gives

$$
S(-t)u_\eta(t)
=S(1)u_\eta(-1)
+i\int_{-1}^tS(-s)(u_\eta|u_\eta|^2)(s)\,ds.
$$

Define

$$
u_\eta^\infty=S(1)u_\eta(-1)+iF_\infty\in L^2.
$$

Since the free Schrödinger group is [unitary](../../../fiber-bundle.md#unitary-connection),

$$
\|u_\eta(t)-S(t)u_\eta^\infty\|_2
=\|S(-t)u_\eta(t)-u_\eta^\infty\|_2\longrightarrow0.
$$

This is [scattering from a finite Strichartz norm](../../../nonlinear-analysis.md#scattering-from-a-finite-strichartz-norm).

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2021](../../2021.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
