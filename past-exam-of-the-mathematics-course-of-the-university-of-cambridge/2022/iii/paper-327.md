# Paper 327

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2022/paper_327.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2022/paper_327.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [i](#1/b/i)
      - [Solution](#1/b/i/solution)
    - [ii](#1/b/ii)
      - [Solution](#1/b/ii/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
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
- [3](#3)
  - [Solution](#3/solution)
  - [i](#3/i)
    - [Solution](#3/i/solution)
  - [ii](#3/ii)
    - [Solution](#3/ii/solution)
  - [iii](#3/iii)
    - [Solution](#3/iii/solution)

## 1

↑ **Parent:** [Paper 327](paper-327.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Using [multi-index notation](../../../distribution-theory.md#multi-index-notation), the [Schwartz space](../../../fourier-analysis.md#schwartz-space) is

$$
\mathcal S(\mathbb R^n)=\left\{\varphi\in C^\infty(\mathbb R^n):p_{\alpha,\beta}(\varphi)=\sup_{x\in\mathbb R^n}|x^\alpha\partial^\beta\varphi(x)|<\infty\text{ for all }\alpha,\beta\right\}.
$$

A [sequence](../../../real-analysis.md#sequence) $\varphi_m$ converges to $\varphi$ in this [Fréchet space](../../../topological-vector-space.md#frechet-space) when $p_{\alpha,\beta}(\varphi_m-\varphi)\to0$ for every $\alpha,\beta$. The space $\mathcal S'(\mathbb R^n)$ of [tempered distributions](../../../fourier-analysis.md#tempered-distribution) is the [continuous dual](../../../continuous-dual-space.md) of $\mathcal S(\mathbb R^n)$, and $u_m\to u$ there means [weak convergence of distributions](../../../distribution-theory.md#weak-convergence-of-distributions), namely $\langle u_m,\varphi\rangle\to\langle u,\varphi\rangle$ for every $\varphi\in\mathcal S$.

Continuity of a [linear functional](../../../linear-algebra.md#linear-functional) immediately implies that $\varphi_m\to0$ entails $\langle u,\varphi_m\rangle\to0$. Conversely, enumerate the Schwartz [seminorms](../../../topological-vector-space.md#seminorm) as $p_1,p_2,\ldots$. If $u$ were not continuous, then for each $m$ one could choose $\varphi_m$ such that

$$
p_j(\varphi_m)\leq\frac1m\quad(1\leq j\leq m),
\qquad
|\langle u,\varphi_m\rangle|\geq1.
$$

Every fixed seminorm tends to zero along this sequence, so $\varphi_m\to0$ in $\mathcal S$, contradicting the assumed sequential property. This is the [sequential continuity criterion for a linear map on a metrizable topological vector space](../../../topological-vector-space.md#sequential-continuity-criterion-for-a-linear-map-on-a-metrizable-topological-vector-space).

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

The angular-frequency [Fourier transform](../../../analysis.md#fourier-transform) and its inverse on $\mathcal S(\mathbb R^n)$ are

$$
\widehat\varphi(\lambda)=\int_{\mathbb R^n}e^{-i\lambda\cdot x}\varphi(x)\,dx,
\qquad
\varphi(x)=\frac1{(2\pi)^n}\int_{\mathbb R^n}e^{i\lambda\cdot x}\widehat\varphi(\lambda)\,d\lambda.
$$

It extends to a [tempered distribution](../../../fourier-analysis.md#tempered-distribution) by duality:

$$
\langle\widehat u,\varphi\rangle=\langle u,\widehat\varphi\rangle.
$$

<h4 id="1/b/i">i</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/i/solution">Solution</h5>

↑ **Parent:** [I](#1/b/i)

Since $\delta_{1/t}\varphi(x)=\varphi(x/t)$ maps the [Schwartz space](../../../fourier-analysis.md#schwartz-space) continuously to itself, the formula

$$
\langle\delta_tu,\varphi\rangle=t^{-n}\langle u,\delta_{1/t}\varphi\rangle
$$

defines a continuous [linear functional](../../../linear-algebra.md#linear-functional) on $\mathcal S$, hence a [tempered distribution](../../../fourier-analysis.md#tempered-distribution). For a [locally integrable function](../../../distribution-theory.md#locally-integrable-function) $u$, the [change of variables formula](../../../calculus.md#change-of-variables-formula) $y=tx$ gives

$$
\int_{\mathbb R^n}u(tx)\varphi(x)\,dx
=t^{-n}\int_{\mathbb R^n}u(y)\varphi(y/t)\,dy,
$$

so this [dilation of a distribution](../../../distribution-theory.md#dilation-of-a-distribution) agrees with ordinary function dilation.

<h4 id="1/b/ii">ii</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/b/ii)

The [scaling property of the Fourier transform](../../../analysis.md#scaling-property-of-the-fourier-transform) gives, first for [Schwartz functions](../../../fourier-analysis.md#schwartz-function) and then by duality,

$$
\widehat{\delta_tu}=t^{-n}\delta_{1/t}\widehat u.
$$

If the [homogeneous distribution](../../../distribution-theory.md#homogeneous-distribution) $u$ has degree $\sigma$, then

$$
t^\sigma\widehat u=t^{-n}\delta_{1/t}\widehat u.
$$

Putting $s=1/t$ yields $\delta_s\widehat u=s^{-n-\sigma}\widehat u$. Thus the [Fourier transform of a homogeneous distribution](../../../distribution-theory.md#fourier-transform-of-a-homogeneous-distribution) has degree $\boxed{-n-\sigma}$.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Because $0<\alpha<n$, $|x|^{-\alpha}$ is [locally integrable](../../../distribution-theory.md#locally-integrable-function) at the origin and has only [polynomial growth](../../../analysis.md#polynomial-growth) at infinity, so it defines a [tempered distribution](../../../fourier-analysis.md#tempered-distribution). It is a [homogeneous distribution](../../../distribution-theory.md#homogeneous-distribution) of degree $-\alpha$ and is [radial](../../../partial-differential-equation.md#radial-function). Its Fourier transform is therefore radial and homogeneous of degree $\alpha-n$, so it must have the form $c_\alpha|\lambda|^{\alpha-n}$. In particular, $\boxed{\beta=n-\alpha}$.

To determine the constant, use the stated [Gamma integral](../../../complex-analysis.md#gamma-integral) representation, [Fubini's theorem](../../../measure-theory.md#fubini-s-theorem), and the [Fourier transform of a Gaussian](../../../fourier-analysis.md#fourier-transform-of-a-gaussian):

$$
\begin{aligned}
\widehat u_\alpha(\lambda)
&=\frac1{\Gamma(\alpha/2)}\int_0^\infty\tau^{\alpha/2-1}
\left(\int_{\mathbb R^n}e^{-\tau|x|^2-i\lambda\cdot x}\,dx\right)d\tau\\
&=\frac{\pi^{n/2}}{\Gamma(\alpha/2)}
\int_0^\infty\tau^{(\alpha-n)/2-1}e^{-|\lambda|^2/(4\tau)}\,d\tau.
\end{aligned}
$$

The [change of variables formula](../../../calculus.md#change-of-variables-formula) $s=|\lambda|^2/(4\tau)$ then gives

$$
\widehat u_\alpha(\lambda)
=2^{n-\alpha}\pi^{n/2}
\frac{\Gamma((n-\alpha)/2)}{\Gamma(\alpha/2)}
|\lambda|^{\alpha-n}.
$$

This is precisely the [Fourier transform of the Riesz kernel](../../../distribution-theory.md#riesz-kernel).

## 2

↑ **Parent:** [Paper 327](paper-327.md)

The [space of smooth functions](../../../distribution-theory.md#space-of-smooth-functions) $\mathcal E(X)=C^\infty(X)$ has the topology of uniform convergence of every derivative on every [compact set](../../../topology.md#compact-space) $K\Subset X$. Thus $f_j\to f$ exactly when

$$
\sup_{x\in K}|\partial^\alpha(f_j-f)(x)|\longrightarrow0
$$

for every $K$ and every [multi-index](../../../distribution-theory.md#multi-index-notation) $\alpha$. Its [continuous dual](../../../continuous-dual-space.md) $\mathcal E'(X)$ is the [compactly supported distribution space](../../../distribution-theory.md#compactly-supported-distribution-space); convergence in the weak dual topology means pointwise convergence on every $f\in\mathcal E(X)$.

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Let $K$ contain the support of $u\in\mathcal E'(\mathbb R^n)$. Choose a [cutoff function](../../../distribution-theory.md#cutoff-function) that equals one near $K$. It makes

$$
\widehat u(\lambda)=\langle u(x),e^{-i\lambda\cdot x}\rangle
$$

well-defined, and differentiating the parameter under the pairing gives

$$
\partial_\lambda^\gamma\widehat u(\lambda)
=\langle u(x),(-ix)^\gamma e^{-i\lambda\cdot x}\rangle.
$$

Thus the [Fourier transform of a compactly supported distribution](../../../distribution-theory.md#fourier-transform-of-a-compactly-supported-distribution) is a [smooth function](../../../analysis.md#smooth-function). Since a compactly supported distribution has finite order, some $N$ and $C$ satisfy

$$
|\langle u,\psi\rangle|\leq C\sum_{|\alpha|\leq N}\sup_K|\partial^\alpha\psi|.
$$

Applying this estimate to the exponential yields $|\widehat u(\lambda)|\leq C'\langle\lambda\rangle^N$.

Now take $v\in\mathcal E'(X)$, multiply by a [cutoff function](../../../distribution-theory.md#cutoff-function) supported in $X$ and equal to one near $\operatorname{supp}v$, and regard the result as an element of $\mathcal E'(\mathbb R^n)$. Choose $m$ so large that

$$
g(\lambda)=\langle\lambda\rangle^{-2m}\widehat v(\lambda)
$$

is [Lebesgue integrable](../../../measure-theory.md#lebesgue-integrable-function). The inverse [Fourier transform](../../../analysis.md#fourier-transform) $f=\mathcal F^{-1}g$ is a bounded [continuous function](../../../calculus.md#continuous-function), and the [Fourier transform of a derivative](../../../fourier-analysis.md#fourier-transform-of-a-derivative) gives

$$
v=(1-\Delta)^m f
$$

as a [distributional identity](../../../distribution-theory.md#distributional-identity). This is the [Bessel potential](../../../distribution-theory.md#bessel-potential) proof of the [structure theorem for compactly supported distributions](../../../distribution-theory.md#structure-theorem-for-compactly-supported-distributions).

The function $f$ itself need not have [compact support](../../../function.md#compact-support). Choose another cutoff $\rho\in\mathcal D(X)$ equal to one near $\operatorname{supp}v$. Then $v=\rho(1-\Delta)^mf$. Repeatedly using

$$
\rho\,\partial^\alpha f
=\sum_{\beta\leq\alpha}(-1)^{|\alpha-\beta|}\binom{\alpha}{\beta}
\partial^\beta\bigl(f\,\partial^{\alpha-\beta}\rho\bigr)
$$

expresses $v$ as a finite sum $\sum_\beta\partial^\beta f_\beta$, where every coefficient $f_\beta$ is continuous and compactly supported in $X$.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/i">i</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/i/solution">Solution</h5>

↑ **Parent:** [I](#2/b/i)

By [multiplication of a distribution by a smooth function](../../../distribution-theory.md#multiplication-of-a-distribution-by-a-smooth-function), for every [test function](../../../distribution-theory.md#test-function) $\psi$,

$$
\langle\rho\delta_0,\psi\rangle
=\langle\delta_0,\rho\psi\rangle
=\rho(0)\psi(0)=\psi(0)
=\langle\delta_0,\psi\rangle.
$$

**Hence $\rho\delta_0=\delta_0$.**

<h4 id="2/b/ii">ii</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/b/ii)

The [distributional derivative of the Heaviside step function](../../../distribution-theory.md#distributional-derivative-of-the-heaviside-step-function) is $H'=\delta_0$. The [Leibniz rule](../../../calculus.md#leibniz-rule) and $x\delta_0=0$ therefore give

$$
\boxed{(xH)'=H+x\delta_0=H,
\qquad
(xH)''=H'=\delta_0.}
$$

<h4 id="2/b/iii">iii</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#2/b/iii)

Applying the distributional [Leibniz rule](../../../calculus.md#leibniz-rule) twice gives

$$
(\varphi u)''=\varphi''u+2\varphi'u'+\varphi u'',
\qquad
(\varphi'u)'=\varphi''u+\varphi'u'.
$$

Eliminating the middle term proves

$$
\varphi u''=\varphi''u-2(\varphi'u)'+(\varphi u)''.
$$

Choose $\rho\in\mathcal D(\mathbb R)$ with $\rho(0)=1$. Parts i and ii and the identity just proved, with $\varphi=\rho$ and $u=xH$, yield

$$
\delta_0=\rho(xH)''=\rho''xH-2(\rho'xH)'+(\rho xH)''.
$$

Thus explicit [continuous functions](../../../calculus.md#continuous-function) of [compact support](../../../function.md#compact-support) are

$$
\boxed{f_0=xH\rho'',\qquad f_1=-2xH\rho',\qquad f_2=xH\rho}.
$$

## 3

↑ **Parent:** [Paper 327](paper-327.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

The [Malgrange–Ehrenpreis theorem](../../../distribution-theory.md#malgrange-ehrenpreis-theorem) states that every nonzero constant-coefficient [linear partial differential operator](../../../partial-differential-equation.md#linear-partial-differential-operator) $P(D)$ on $\mathbb R^n$ has a [fundamental solution of a linear differential operator](../../../distribution-theory.md#fundamental-solution-of-a-linear-differential-operator): there is an $E\in\mathcal D'(\mathbb R^n)$ such that $P(D)E=\delta_0$.

Write $D=-i\partial$. After an [orthogonal change of coordinates](../../../linear-algebra.md#orthogonal-matrix) and multiplication by a nonzero constant, its polynomial symbol may be written as a monic polynomial in the last frequency,

$$
P(\xi',z)=z^M+\sum_{m=0}^{M-1}a_m(\xi')z^m.
$$

For each real $\mu'$, this polynomial has $M$ complex roots counted with multiplicity. Among a fixed finite collection of horizontal lines at bounded heights, one can choose a line that stays a positive distance from all those roots. Continuity of the roots preserves the choice on a neighborhood $N(\mu')$. Take a countable locally finite cover by such neighborhoods, refine it to a measurable disjoint partition $\mathbb R^{n-1}=\bigsqcup_j\Delta_j$, and let $c_j$ be the chosen height on $\Delta_j$. The resulting [Hörmander staircase](../../../distribution-theory.md#hormander-staircase)

$$
\Sigma=\bigcup_j\{(\xi',s+ic_j):\xi'\in\Delta_j,\ s\in\mathbb R\}
$$

has bounded heights and may be chosen so that $|P(\xi',s+ic_j)|\geq1$ on each step.

For a [test function](../../../distribution-theory.md#test-function) $\varphi$, define

$$
\langle E,\varphi\rangle
=\frac1{(2\pi)^n}\sum_j
\int_{\Delta_j}\int_{\mathbb R+ic_j}
\frac{\widehat\varphi(-\xi',-z)}{P(\xi',z)}\,dz\,d\xi'.
$$

The [Paley–Wiener–Schwartz theorem](../../../distribution-theory.md#paley-wiener-schwartz-theorem) gives rapid decay in the real frequency directions and at most a fixed exponential factor in the bounded imaginary direction. Together with $|P|\geq1$, this proves that the integral defines a continuous [distribution](../../../distribution-theory.md#distribution-mathematical-analysis). Applying $P(D)$ cancels the denominator. The remaining integrand is [entire](../../../complex-analysis.md#entire-function) in $z$, so the [Cauchy integral theorem](../../../complex-analysis.md#cauchy-s-integral-theorem) shifts every horizontal contour to the real axis; the partition then recombines into $\mathbb R^{n-1}$. The [Fourier inversion theorem](../../../fourier-analysis.md#fourier-inversion-theorem) gives

$$
\langle P(D)E,\varphi\rangle=\varphi(0)=\langle\delta_0,\varphi\rangle,
$$

which proves the theorem.

<h3 id="3/i">i</h3>

↑ **Parent:** [3](#3)

<h4 id="3/i/solution">Solution</h4>

↑ **Parent:** [I](#3/i)

For the [wave operator](../../../wave-equation.md) $\partial_x^2-\partial_y^2$, use the symbol

$$
P(\xi,\eta)=\eta^2-\xi^2
$$

and complexify $\eta$. Its roots $\eta=\pm\xi$ are real for every real $\xi$, so the single horizontal step

$$
\boxed{\operatorname{Im}\eta=1}
$$

never meets a root and is an explicit [Hörmander staircase](../../../distribution-theory.md#hormander-staircase).

<h3 id="3/ii">ii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#3/ii)

For the [Laplace operator](../../../partial-differential-equation.md#laplace-operator), an irrelevant nonzero factor gives the symbol $P(\xi,\eta)=\xi^2+\eta^2$. The roots in complex $\eta$ are $\eta=\pm i|\xi|$, so no fixed horizontal line avoids them for every $\xi$. A two-step staircase is

$$
\boxed{
\operatorname{Im}\eta=
\begin{cases}
2,&|\xi|\leq1,\\
0,&|\xi|>1.
\end{cases}}
$$

On the first step the roots have imaginary part in $[-1,1]$, and on the second they are nonreal, so neither step meets the zero set.

<h3 id="3/iii">iii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#3/iii)

For the [heat operator](../../../diffusion-equation.md#heat-equation) $\partial_x-\partial_y^2$, complexify the first frequency. Its symbol is

$$
P(\xi,\eta)=i\xi+\eta^2,
$$

whose root in $\xi$ is $\xi=i\eta^2$ and therefore lies in the closed upper half-plane for real $\eta$. The single step

$$
\boxed{\operatorname{Im}\xi=-1}
$$

lies strictly below every root and is an explicit [Hörmander staircase](../../../distribution-theory.md#hormander-staircase).

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2022](../../2022.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
