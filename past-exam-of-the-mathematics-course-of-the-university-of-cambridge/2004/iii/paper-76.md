# Paper 76

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2004/Paper76.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2004/Paper76.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
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
  - [i](#2/i)
    - [Solution](#2/i/solution)
  - [ii](#2/ii)
    - [Solution](#2/ii/solution)
  - [iii](#2/iii)
    - [Solution](#2/iii/solution)
  - [iv](#2/iv)
    - [Solution](#2/iv/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [a](#4/a)
    - [i](#4/a/i)
      - [Solution](#4/a/i/solution)
    - [ii](#4/a/ii)
      - [Solution](#4/a/ii/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
- [5](#5)
  - [a](#5/a)
    - [i](#5/a/i)
      - [Solution](#5/a/i/solution)
    - [ii](#5/a/ii)
      - [Solution](#5/a/ii/solution)
    - [iii](#5/a/iii)
      - [Solution](#5/a/iii/solution)
  - [b](#5/b)
    - [Solution](#5/b/solution)

## 1

↑ **Parent:** [Paper 76](paper-76.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

For $0<\lambda<1$ fixed, the denominator stays away from zero, so [dominated convergence](../../../measure-theory.md#dominated-convergence-theorem) gives

$$
J\sim\int_0^1\frac{dx}{(1-\lambda+\lambda x)^2}=\boxed{\frac1{1-\lambda}}.
$$

This approximation remains appropriate on the left of the transition when $1-\lambda\gg\epsilon$. To resolve the [Lorentzian peak approaching an integration endpoint](../../../analysis.md#lorentzian-peak-approaching-an-integration-endpoint), let $\lambda-1=\epsilon\tau$ with bounded $\tau$, and put $x=\epsilon X$. The cosine is $1+O(\epsilon^2X^2)$ in the contributing region. Therefore

$$
J\sim\frac1\epsilon\int_0^\infty\frac{dX}{(\lambda X-\tau)^2+1}
=\boxed{\frac1{\epsilon\lambda}\left[\frac\pi2+\arctan\frac{\lambda-1}{\epsilon}\right]}.
$$

Thus the distinguished transition has width **$|\lambda-1|=O(\epsilon)$**. For large negative $\tau$ this expression matches $1/(1-\lambda)$ to leading order; for large positive $\tau$ it gives the full interior-peak contribution.

For $\lambda>1$ away from the transition, the denominator has a narrow minimum at $x_*=1-1/\lambda$. Set $c_* =\cos(\pi x_*/2)=\sin(\pi/(2\lambda))$ and $x-x_*=(\epsilon c_*/\lambda)s$. The slowly varying cosine may be frozen over the peak and the integration limits extended, giving

$$
J\sim\frac1{\epsilon\lambda c_*}\int_{-\infty}^{\infty}\frac{ds}{1+s^2}
=\boxed{\frac\pi{\epsilon\lambda\sin(\pi/(2\lambda))}}.
$$

The small parameter controlling the left-end truncation near $\lambda=1$ is $\epsilon/(\lambda-1)$, so this formula requires $\lambda-1\gg\epsilon$ there.

For $\lambda\gg1$, the peak approaches $x=1$, but its width is $\epsilon\pi/(2\lambda^2)$ whereas its distance from that endpoint is $1/\lambda$. Their ratio is $O(\epsilon/\lambda)$, and the relative variation of the cosine across the peak is also $O(\epsilon/\lambda)$. Hence proximity to the endpoint does not destroy the approximation: the peak becomes narrower still. Equivalently, $s=\lambda(1-x)$ gives $J=\lambda^{-1}\int_0^\lambda[(1-s)^2+\epsilon^2\sin^2(\pi s/(2\lambda))]^{-1}ds$, with its peak at $s=1$. The large-$\lambda$ limit of the leading result is **$J\sim2/\epsilon$**.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/i">i</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/i/solution">Solution</h5>

↑ **Parent:** [I](#1/b/i)

Take the usual [Heaviside step function](../../../analysis.md#heaviside-step-function), $H(x)=1$ for $x>0$ and $0$ for $x<0$. Its [Fourier transform](../../../analysis.md#fourier-transform) must be interpreted as a [tempered distribution](../../../fourier-analysis.md#tempered-distribution). For $a>0$, exponential damping gives an ordinary integral:

$$
\widehat{e^{-ax}H(x)}(k)=\int_0^\infty e^{-(a+ik)x}\,dx
=\frac1{a+ik}=\frac a{a^2+k^2}-i\frac{k}{a^2+k^2}.
$$

Against any [Schwartz function](../../../fourier-analysis.md#schwartz-function) $\varphi$, the first term is an [approximate identity](../../../fourier-analysis.md#approximate-identity) of total mass $\pi$: changing variables $k=au$ gives the limit $\pi\varphi(0)$. For the second term, pair positive and negative $k$ near zero. The difference $\varphi(k)-\varphi(-k)=O(k)$ removes the singularity and gives the [Cauchy principal value](../../../complex-analysis.md#cauchy-principal-value) of $1/k$. The tails converge by [dominated convergence](../../../measure-theory.md#dominated-convergence-theorem). Since the damped functions also approach $H$ as [tempered distributions](../../../fourier-analysis.md#tempered-distribution), continuity of the [Fourier transform](../../../analysis.md#fourier-transform) yields the [Fourier transform of the Heaviside step function](../../../fourier-analysis.md#fourier-transform-of-the-heaviside-step-function):

$$
\boxed{\widehat H(k)=\pi\delta(k)-i\operatorname{PV}\frac1k}.
$$

**The printed plus sign is inconsistent with the printed $e^{-ikx}$ convention for this $H$.** In fact $H'=\delta$ requires $ik\widehat H=1$; the printed expression would give $-1$. Its plus sign would instead be correct for $H(-x)$.

To find the [Fourier transform of a principal-value reciprocal](../../../fourier-analysis.md#principal-value-fourier-transform-of-a-real-pole), exponential damping of its odd part gives

$$
\widehat{e^{-a|x|}\operatorname{PV}(1/x)}(k)
=-2i\int_0^\infty e^{-ax}\frac{\sin(kx)}x\,dx.
$$

The integral vanishes at $k=0$ and its $k$-derivative is $a/(a^2+k^2)$, so it equals $\arctan(k/a)$. Taking the [distributional convergence](../../../distribution-theory.md#weak-convergence-of-distributions) limit gives

$$
\boxed{\mathcal F\!\left(\operatorname{PV}\frac1x\right)(k)=-i\pi\operatorname{sgn}k}.
$$

An ordinary improper integral of $1/x$ across zero is not a substitute for the specified [Cauchy principal value](../../../complex-analysis.md#cauchy-principal-value).

<h4 id="1/b/ii">ii</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/b/ii)

The locally integrable function $\log|x|$ defines a [tempered distribution](../../../fourier-analysis.md#tempered-distribution). Its [distributional derivative](../../../distribution-theory.md#distributional-derivative) is $\operatorname{PV}(1/x)$: perform [integration by parts](../../../calculus.md#integration-by-parts) outside $(-a,a)$, and observe that the boundary contribution $\log a[\varphi(a)-\varphi(-a)]$ tends to zero. By the [Fourier transform of a derivative](../../../fourier-analysis.md#fourier-transform-of-a-derivative) and the preceding result,

$$
ik\widehat{\log|x|}=-i\pi\operatorname{sgn}k.
$$

Division by $|k|$ needs a [finite-part inverse-absolute-value distribution](../../../distribution-theory.md#finite-part-inverse-absolute-value-distribution), since $1/|k|$ is not locally integrable at zero. One possible normalization is

$$
\left\langle\operatorname{Pf}\frac1{|k|},\varphi\right\rangle
=\int_{|k|<1}\frac{\varphi(k)-\varphi(0)}{|k|}\,dk
+\int_{|k|\ge1}\frac{\varphi(k)}{|k|}\,dk.
$$

It satisfies $k\operatorname{Pf}(1/|k|)=\operatorname{sgn}k$. The general solution of $kT=0$ is a multiple of the [Dirac delta distribution](../../../distribution-theory.md#dirac-delta-function): a [test function](../../../distribution-theory.md#test-function) vanishing at zero can be written $k\psi(k)$, so $T$ depends only on its value at zero. Consequently the [Fourier transform of the absolute logarithm](../../../fourier-analysis.md#fourier-transform-of-the-absolute-logarithm) is

$$
\boxed{\widehat{\log|x|}(k)=-\pi\operatorname{Pf}\frac1{|k|}+C\delta(k)}.
$$

Changing the finite-part normalization changes $C$. The printed reciprocal expression is meaningful with this interpretation, not as an ordinary function at $k=0$.

<h4 id="1/b/iii">iii</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#1/b/iii)

The barred integral in the PDF denotes a [Cauchy principal value](../../../complex-analysis.md#cauchy-principal-value). With $p(x)=\operatorname{PV}(1/x)$ its left side is the [convolution](../../../fourier-analysis.md#convolution) $p*f$, whose [Fourier transform](../../../analysis.md#fourier-transform) is $-i\pi\operatorname{sgn}(k)\widehat f(k)$. The right side is $-1$ on $(-1,1)$ and zero outside; either direct integration or the [Fourier transform](../../../analysis.md#fourier-transform) shift rule gives

$$
\widehat{H(x-1)-H(x+1)}=-\frac{2\sin k}{k}.
$$

Thus, away from the irrelevant single point $k=0$ in the $L^2$ formulation,

$$
\widehat f(k)=-\frac{2i}{\pi}\frac{\sin k}{|k|}.
$$

By the [Fourier transform of the absolute logarithm](../../../fourier-analysis.md#fourier-transform-of-the-absolute-logarithm), the difference $\log|x-1|-\log|x+1|$ has transform $2i\pi\sin k/|k|$; its two delta terms cancel. Therefore

$$
\boxed{f(x)=\frac1{\pi^2}\log\left|\frac{x+1}{x-1}\right|}.
$$

Its endpoint logarithms are locally square integrable, and $f(x)=2/(\pi^2x)+O(x^{-3})$ at infinity, so it belongs to [L2 space](../../../measure-theory.md#l2-space-is-a-hilbert-space). The [Hilbert transform](../../../analysis.md#hilbert-transform) multiplier is invertible almost everywhere on this space, proving uniqueness there. Without a decay or function-space condition, one may also add a constant under the symmetric principal-value convention. If the reversed step function were used to retain the printed sign in part (i), this answer would acquire the opposite sign.

<h4 id="1/b/iv">iv</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#1/b/iv)

Write $K_0(z)=-F(z)\log z+G(z)$ locally, with analytic $F,G$ and $F(0)=1$. The coefficient of $\log z$ in the [Modified Bessel differential equation](../../../analysis.md#modified-bessel-differential-equation) requires $z^2F''+zF'-z^2F=0$. If $F=\sum a_mz^m$, its recurrence is $m^2a_m=a_{m-2}$, with $a_1=0$. Hence

$$
F(z)=1+\frac{z^2}{4}+O(z^4),\qquad
K_0(|x|)=-\log|x|-\frac{x^2}{4}\log|x|+G(|x|)+O(x^4\log|x|).
$$

The analytic part is even: an odd-power term in $G$ would produce an uncancelled odd-power term under the same differential operator, and the recurrence removes all such terms. Insert a smooth even cutoff equal to one near zero. The smooth part and the exponentially decaying tails give no algebraic large-[wavenumber](../../../wave-equation.md#wavenumber) terms after repeated [integration by parts](../../../calculus.md#integration-by-parts). Therefore the [logarithmic singularities](../../../analysis.md#logarithmic-singularity) determine the requested terms. For $k\ne0$,

$$
\mathcal F(\log|x|)=-\frac\pi{|k|},\qquad
\mathcal F(x^2\log|x|)=-\frac{d^2}{dk^2}\left(-\frac\pi{|k|}\right)=\frac{2\pi}{|k|^3}.
$$

Thus the [Fourier transform of the modified Bessel function K0](../../../analysis.md#fourier-transform-of-the-modified-bessel-function-k0) has expansion

$$
\boxed{\widehat{K_0(|x|)}(k)=\frac\pi{|k|}-\frac\pi{2|k|^3}+O(|k|^{-5})}.
$$

An independent check follows from the [integral representation of the modified Bessel function of the second kind](../../../analysis.md#integral-representation-of-the-modified-bessel-function-of-the-second-kind). Integrating $e^{-|x|\cosh t}$ first and then setting $u=\sinh t$ gives $2\int_0^\infty du/(u^2+1+k^2)=\pi/\sqrt{1+k^2}$, with exactly these first two terms.

## 2

↑ **Parent:** [Paper 76](paper-76.md)

<h3 id="2/i">i</h3>

↑ **Parent:** [2](#2)

<h4 id="2/i/solution">Solution</h4>

↑ **Parent:** [I](#2/i)

Use the [Gaussian pole transition for a large gamma parameter](../../../analysis.md#gaussian-pole-transition-for-a-large-gamma-parameter). With $t=1+s/\sqrt n$ and $\lambda=n+i\mu\sqrt n+\nu+o(1)$, [Taylor expansion](../../../calculus.md#taylor-expansion) gives

$$
(n-1)\log t+\lambda(1-t)
=-\frac{s^2}{2}-i\mu s+\frac1{\sqrt n}\left(\frac{s^3}{3}-(1+\nu)s\right)+O(n^{-1}(1+|s|^4)),
\qquad \frac{dt}{1-t}=-\frac{ds}{s}.
$$

The upper semicircle is traversed from left to right, so $\int ds/s=-i\pi$ on the indentation. The minus sign in $dt/(1-t)$ therefore makes its contribution $+i\pi$. The remaining leading integral is

$$
I_0(\mu)=i\pi-\operatorname{PV}\int_{-\infty}^{\infty}\frac{e^{-s^2/2-i\mu s}}s\,ds.
$$

At $\mu=0$ its [Cauchy principal value](../../../complex-analysis.md#cauchy-principal-value) vanishes by oddness. Differentiating with respect to $\mu$ removes the [pole](../../../isolated-singularity.md#pole), leaving the [Fourier transform of a Gaussian](../../../fourier-analysis.md#fourier-transform-of-a-gaussian):

$$
I_0'(\mu)=i\sqrt{2\pi}e^{-\mu^2/2}.
$$

Integrating from zero gives

$$
\boxed{I(\lambda,n)=i\pi\left[1+\operatorname{erf}\left(\frac\mu{\sqrt2}\right)\right]+O(n^{-1/2})}.
$$

This is uniform for bounded real $\mu,\nu$ (and extends analytically over bounded complex values where the local contour is continued consistently). Contributions away from the saddle are exponentially small after localization. The bounded shift $\nu$ enters at the next order, not the leading [error function](../../../calculus.md#error-function). For example, retaining the displayed cubic correction gives $\sqrt{2\pi/n}e^{-\mu^2/2}[\nu+(2+\mu^2)/3]$ as the next term. This also checks the constant and contour sign.

<h3 id="2/ii">ii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#2/ii)

For positive integer $n$ and any positive integer $N$, the finite [geometric series](../../../real-analysis.md#geometric-series) identity

$$
\frac1{1-t}=\sum_{j=0}^{N-1}t^j+\frac{t^N}{1-t}
$$

gives an exact decomposition along the indented contour. The polynomial terms have no [pole](../../../isolated-singularity.md#pole) and may be returned to the positive real axis; their [Gamma function](../../../complex-analysis.md#gamma-function) integrals are

$$
I(\lambda,n)=e^\lambda\sum_{r=n}^{n+N-1}\frac{\Gamma(r)}{\lambda^r}+I(\lambda,n+N).
$$

Equivalently, expansion about the endpoint $t=0$ in the [Laplace transform](../../../analysis.md#laplace-transform) integral gives the same coefficients. The resulting formal [asymptotic expansion](../../../analysis.md#asymptotic-expansion) is

$$
\boxed{I(\lambda,n)\sim e^\lambda\sum_{r=n}^{\infty}\frac{\Gamma(r)}{\lambda^r}}.
$$

The ratio of consecutive terms is $r/\lambda$, so the infinite series is factorially divergent. It should be truncated, not treated as a convergent sum; the [pole](../../../isolated-singularity.md#pole) prescription controls the contribution beyond its algebraic orders. Although the source initially calls $n$ an integer, the ordinary lower endpoint integral requires $n>0$, as is already implicit in the large-positive-$n$ limit of part (i).

<h3 id="2/iii">iii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#2/iii)

By [Stirling's approximation](../../../real-analysis.md#stirling-formula), for fixed $a$,

$$
\frac{\Gamma(r+a)}{\Gamma(r)}=r^a[1+O(r^{-1})].
$$

Apply this with $a=1/6,5/6$ and use $\Gamma(r+1)=r\Gamma(r)$. Their exponents add to one, and hence

$$
\boxed{Y_r=\frac{\Gamma(r)}{2\pi\sigma^r}[1+O(r^{-1})]}.
$$

More explicitly, the ratio is $1-5/(36r)+O(r^{-2})$. The exact ratio of neighboring terms is

$$
\frac{Y_{r+1}}{Y_r}=\frac{(r+1/6)(r+5/6)}{\sigma(r+1)}\sim\frac r\sigma.
$$

Thus the [Airy function](../../../differential-equation.md#airy-function) expansion is factorially divergent, and [optimal truncation](../../../analysis.md#optimal-truncation) retains about $|\sigma|$ terms.

**The printed summation starts at $r=1$, but its leading $r=0$ term is missing.** The [Gamma reflection formula](../../../complex-analysis.md#gamma-reflection-formula) gives $\Gamma(1/6)\Gamma(5/6)=2\pi$, so $Y_0=1$. The correctly normalized dominant [Airy function](../../../differential-equation.md#airy-function) expansion starts at zero. This correction is essential for the exponentially small remainder in the next part; if the printed series is used literally, its remainder also contains the entire missing leading term.

<h3 id="2/iv">iv</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#2/iv)

Let $P(z)=1/(2\sqrt\pi z^{1/4})$, choose a consistent branch, and truncate the corrected series after $r=n-1$, with $n=|\sigma|+O(1)$. The leading factorial tail in part (iii) is represented by the same indented integral as in part (ii):

$$
R_n\sim\frac{P(z)e^{\sigma/2}}{2\pi}\sum_{r=n}^{\infty}\frac{\Gamma(r)}{\sigma^r}
\quad\longleftrightarrow\quad
\frac{P(z)e^{-\sigma/2}}{2\pi}I(\sigma,n).
$$

Here the divergent sum means its lateral [Borel summation](../../../analysis.md#borel-summation), not ordinary summation. To see why the [pole](../../../isolated-singularity.md#pole) approximation controls this remainder, write $a_r=\sigma^rY_r$ and insert $\Gamma(r)=\int_0^\infty e^{-v}v^{r-1}dv$ in the leading late terms. Summing the geometric tail creates $1/(1-v/\sigma)$; $v=\sigma t$ produces $I(\sigma,n)$. The relative $O(r^{-1})$ corrections to the late coefficients give lower-order contributions on its saddle scale. More concretely, the [Borel transform](../../../analysis.md#borel-transform-of-a-factorially-divergent-series) of the coefficient series is

$$
\sum_{r=1}^\infty\frac{a_r t^{r-1}}{\Gamma(r)}
=\frac d{dt}\,{}_2F_1\left(\frac16,\frac56;1;t\right)
=\frac1{2\pi(1-t)}+O(\log(1-t))\quad(t\to1).
$$

The [simple pole](../../../isolated-singularity.md#simple-pole) supplies the leading [Stokes phenomenon](../../../analysis.md#stokes-phenomenon); its weaker [logarithmic singularity](../../../analysis.md#logarithmic-singularity) supplies the smaller corrections. This is the integral justification for retaining the factorial tail.

For $\arg\sigma=\phi/\sqrt{|\sigma|}$, expand $\sigma=n+i\phi\sqrt n+O(1)$. Part (i), with $\mu=\phi$, now gives

$$
\boxed{R_n\sim\frac{i e^{-\sigma/2}}{4\sqrt\pi z^{1/4}}
\left[1+\operatorname{erf}\left(\frac\phi{\sqrt2}\right)\right]}.
$$

This formula uses the upper-pole prescription and the upper [Airy function](../../../differential-equation.md#airy-function) switching ray: near $\arg z=2\pi/3$, take $\arg\sigma=3\arg z/2-\pi$ near zero. The coefficient of the subdominant exponential changes smoothly from zero to $i$ across this ray and has value $i/2$ on it. The angular transition width is $O(|\sigma|^{-1/2})=O(|z|^{-3/4})$. The conjugate lower ray has the conjugate contour sign, rather than the same $+i$ on both rays. This is [error-function smoothing of a Stokes multiplier](../../../analysis.md#error-function-smoothing-of-a-stokes-multiplier), not a discontinuity of the analytic [Airy function](../../../differential-equation.md#airy-function). With the literal printed $r=1$ series, the missing $P(z)e^{\sigma/2}$ would invalidate this remainder formula.

## 3

↑ **Parent:** [Paper 76](paper-76.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

The [outer solution](../../../differential-equation.md#outer-expansion) satisfies $y(x)[x+y(x)]=0$, so on a connected interior interval the nonoscillatory branches are $y=0$ and $y=-x$. Both happen to solve the [differential equation](../../../differential-equation.md) exactly away from any endpoint mismatch. For a fixed positive endpoint coordinate $q$ ($q=a$ or $q=1$), introduce the inward distance $\xi=(x-a)/\sqrt\epsilon$ on the left or $\xi=(1-x)/\sqrt\epsilon$ on the right. The leading [nonlinear endpoint layer with a quadratic reaction](../../../differential-equation.md#nonlinear-endpoint-layer-with-a-quadratic-reaction) obeys

$$
Y''+qY+Y^2=0,\qquad
\frac12(Y')^2+\frac q2Y^2+\frac13Y^3=E.
$$

Matching to zero fixes $E=0$, so $(Y')^2=-qY^2-2Y^3/3$. It is negative for every sufficiently small nonzero $Y$. Thus no real nonconstant layer can approach zero: **the zero outer branch requires $\alpha=\beta=0$**, and then $y=0$ is an exact solution.

Matching to $-q$ fixes $E=q^3/6$. The [first integral](../../../differential-equation.md#first-integral) factors as

$$
\boxed{(Y')^2=\frac13(q-2Y)(Y+q)^2}.
$$

Consequently an endpoint value $\eta$ can match this branch only if $\eta\le q/2$. For $-q<\eta<q/2$, there are two choices: a direct approach to $-q$, and an initial excursion to $q/2$ followed by a return to $-q$. Both are translations of

$$
Y(\xi)=-q+\frac{3q}{2}\operatorname{sech}^2\left[\frac{\sqrt q}{2}(\xi-\xi_0)\right],\qquad
\xi_0=\pm\frac2{\sqrt q}\operatorname{arcosh}\sqrt{\frac{3q}{2(\eta+q)}}.
$$

The negative translation gives the direct layer; the positive translation gives the excursion. At $\eta=q/2$ the two coincide, with the maximum at the wall. For $\eta<-q$, the unique admissible direction is a monotone approach from below:

$$
Y(\xi)=-q-\frac{3q}{2}\operatorname{csch}^2\left[\frac{\sqrt q}{2}(\xi+\xi_0)\right],\qquad
\xi_0>0,
$$

where $\xi_0$ is fixed by $Y(0)=\eta$. At $\eta=-q$ only the constant leading layer matches at a finite inward coordinate; a pulse translated infinitely far from the wall is outside this endpoint-layer classification.

Thus the leading admissibility condition for the negative outer branch is **$\alpha\le a/2$ and $\beta\le1/2$**. Under strict inequalities, each endpoint has two choices when its datum lies between $-q$ and $q/2$, and one choice below $-q$. Their independent combinations give one, two or four formal matched profiles. In particular, for $\alpha=\beta=0$ there are four negative-bulk profiles in addition to the exact zero solution, so uniqueness certainly cannot be inferred from the outer equation. The endpoint equalities and the constant-layer cases are degenerate; higher-order endpoint matching is needed to decide exact finite-$\epsilon$ counts at these cutoffs. These conditions and counts concern leading families under the stated exclusion of interior layers and rapid oscillations.

A [matched asymptotic expansion](../../../differential-equation.md#matched-asymptotic-expansion) for the negative branch is

$$
y_{\rm comp}(x)=-x+[Y_L((x-a)/\sqrt\epsilon)+a]
+[Y_R((1-x)/\sqrt\epsilon)+1].
$$

The following sketch shows the four choices for zero endpoint data, together with the exact zero solution. It plots leading composite profiles, not numerical claims of exact finite-$\epsilon$ multiplicity.

<a id="3/image-four-leading-endpoint-layer-profiles-with-negative-outer-branch-and-the-exact-zero-solution"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-76-boundary-layers.png)

**[Figure 1](#3/image-four-leading-endpoint-layer-profiles-with-negative-outer-branch-and-the-exact-zero-solution). Four leading endpoint-layer profiles with negative outer branch, and the exact zero solution**.

Additional interior layers cannot be excluded merely by counting the outer roots. Freezing $x=q$ gives a [homoclinic orbit](../../../dynamical-systems.md#homoclinic-orbit) to $-q$ with the same hyperbolic-secant pulse. Its location would require a further matching or [solvability condition](../../../linear-operator-theory.md#solvability-condition); it is not an arbitrary parameter in the original variable-coefficient problem. Indeed, put $z=y+x$. The exact equation and an energy identity are

$$
\epsilon z''-xz+z^2=0,\qquad
\frac d{dx}\left[\frac\epsilon2(z')^2-\frac x2z^2+\frac13z^3\right]= -\frac12z^2.
$$

An isolated order-one pulse with exponentially small tails on both sides would decrease this energy by an algebraic amount, whereas its two tail energies would be exponentially small. This obstructs a freely standing isolated pulse well away from the walls. It does not by itself classify oscillatory solutions or pulse interactions with endpoint layers, so a complete global uniqueness claim would exceed this leading construction.

When $a=\alpha=0$, the two outer roots meet at the left endpoint. Let $x=\epsilon^pX$, $y=\epsilon^qY$. Balancing $xy$ with $y^2$ gives $p=q$, and balancing $\epsilon y''$ with them gives $1-q=2q$. The [one-third-power scaling at a nonlinear turning endpoint](../../../differential-equation.md#one-third-power-scaling-at-a-nonlinear-turning-endpoint) is therefore

$$
\boxed{x=\epsilon^{1/3}X,\quad y=\epsilon^{1/3}Y,\quad Y''+XY+Y^2=0}.
$$

Its left condition is $Y(0)=0$. Matching to the negative branch requires $Y(X)+X\to0$ and $Y'(X)+1\to0$ as $X\to\infty$; the right endpoint is then handled by the earlier $q=1$ layer. Write $Y=-X+u$. In the intermediate matching region a small correction satisfies $u''-Xu=0$, so $u=C\operatorname{Ai}(X)+D\operatorname{Bi}(X)$. The growing [Airy function](../../../differential-equation.md#airy-function) excludes $D$; the decaying [Airy function](../../../differential-equation.md#airy-function) supplies a permissible stable matching direction. In fact $Y=-X$ is an exact inner solution satisfying $Y(0)=0$, establishing existence of an inner match without solving a nonlinear shooting problem. Since $\operatorname{Ai}(0)\ne0$, the wall condition excludes an infinitesimal nonzero decaying correction about this solution; it does not prove absence of other finite-amplitude inner solutions. The right wall still requires $\beta\le1/2$ at leading order.

Matching instead to zero requires $Y\to0$. Its linearized equation is $Y''+XY=0$, with solutions $\operatorname{Ai}(-X)$ and $\operatorname{Bi}(-X)$. Their large-$X$ forms have envelope $X^{-1/4}$ and phase $2X^{3/2}/3$; although their values decay, they generate rapid spatial oscillations in the overlap region. The imposed nonoscillatory assumption removes these nonzero tails. The exact $Y=0$ remains, and a globally zero outer branch again requires $\beta=0$. The PDF's integration hint uses an inverse hyperbolic tangent; the converted TeX's inverse tangent would give a different and incorrect primitive.

## 4

↑ **Parent:** [Paper 76](paper-76.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/i">i</h4>

↑ **Parent:** [A](#4/a)

<h5 id="4/a/i/solution">Solution</h5>

↑ **Parent:** [I](#4/a/i)

Put $T=\epsilon t$ and use the [method of multiple scales](../../../differential-equation.md#method-of-multiple-scales) with $x=x_0(t,T)+\epsilon x_1+\cdots$. At leading order, $x_{0,tt}+x_0=k$, so write $x_0=k-r(T)\cos(t+\phi(T))$ with $r(0)=k$, $\phi(0)=0$. The order-$\epsilon$ equation is

$$
(\partial_t^2+1)x_1=-2\partial_t\partial_Tx_0-c(1-x_0^2)\partial_tx_0.
$$

Using $\cos^2 t\sin t=(\sin t+\sin3t)/4$, its fundamental sine coefficient is $-2r_T-c r(1-k^2-r^2/4)$, and its fundamental cosine coefficient forces $\phi_T=0$. Removing these resonant forcings is the [solvability condition in the method of multiple scales](../../../differential-equation.md#solvability-condition-in-the-method-of-multiple-scales). Thus the [shifted Van der Pol amplitude evolution](../../../differential-equation.md#shifted-van-der-pol-amplitude-evolution) is

$$
\boxed{r_T=\frac c2(k^2-1)r+\frac c8r^3,\qquad \phi_T=0}.
$$

With $a=k^2-1$ and $R=r^2$, solve $R_T=caR+cR^2/4$ by putting $W=1/R$. This gives

$$
\boxed{r^2(T)=\frac{k^2e^{caT}}{1-\dfrac{k^2}{4a}(e^{caT}-1)}}\quad(a\ne0),\qquad
\boxed{r(T)=(1-cT/4)^{-1/2}}\quad(k=1).
$$

The uniformly valid leading approximation is **$x(t)=k-r(\epsilon t)\cos t+O(\epsilon)$** on bounded slow-time intervals for which $r$ remains bounded. The exact initial [derivative](../../../calculus.md#derivative) is recovered by the first-order correction; the displayed leading expression already satisfies the leading initial data.

There is an important limitation to the source's unqualified time-range wording. Starting from $r(0)=k$, the [amplitude](../../../physics.md#wave-amplitude) decays for $k^2<4/5$, is constant at leading order for $k^2=4/5$, and grows for $k^2>4/5$. In the latter case the denominator vanishes at

$$
T_b=\frac{\log(5-4/k^2)}{c(k^2-1)},\qquad T_b=4/c\ \text{when }k=1.
$$

A bounded-amplitude [multiple-scale expansion](../../../differential-equation.md#method-of-multiple-scales) is uniform for $0\le T\le C<T_b$, not through its predicted large-amplitude breakdown. For the decaying case every fixed bounded slow-time interval is available; the leading unstable equilibrium at $k^2=4/5$ also has bounded [amplitude](../../../physics.md#wave-amplitude) over such intervals. The envelope singularity is a breakdown warning, not a proof that the exact original solution has precisely this blow-up time. The coefficient in the PDF is $\epsilon c$, correcting the converted TeX's duplicated $\epsilon$.

<h4 id="4/a/ii">ii</h4>

↑ **Parent:** [A](#4/a)

<h5 id="4/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#4/a/ii)

Again put $T=\epsilon t$. To leading order the oscillator has form $x_0=k-r(T)\cos(t+\phi(T))$, while the second variable has a slow part $Y(T)$. Averaging its equation over the fast period gives

$$
Y_T=1+k-Y,\qquad Y(0)=0,
\qquad \boxed{Y(T)=(1+k)(1-e^{-T})}.
$$

The oscillatory forcing of the second variable produces only an order-$\epsilon$ correction: its leading fast [derivative](../../../calculus.md#derivative) is $-r(T)\cos t$, whose bounded primitive is $-r(T)\sin t$. Thus it creates no [secular term](../../../differential-equation.md#secular-term).

The oscillator [solvability condition](../../../linear-operator-theory.md#solvability-condition) is the same as in part (i), with $c$ replaced by $Y(T)$:

$$
r_T=\frac Y2(k^2-1)r+\frac Y8r^3,\qquad\phi_T=0.
$$

Introduce accumulated [slow time](../../../differential-equation.md#slow-time)

$$
S(T)=\int_0^T Y(s)\,ds=(1+k)(T-1+e^{-T}).
$$

The [shifted Van der Pol amplitude evolution](../../../differential-equation.md#shifted-van-der-pol-amplitude-evolution) therefore gives, for $a=k^2-1$,

$$
r^2(T)=\frac{k^2e^{aS(T)}}{1-\dfrac{k^2}{4a}(e^{aS(T)}-1)}\quad(a\ne0),\qquad
r(T)=[1-S(T)/4]^{-1/2}\quad(k=1).
$$

Consequently

$$
\boxed{x(t)=k-r(\epsilon t)\cos t+O(\epsilon),\qquad
y(t)=(1+k)(1-e^{-\epsilon t})+O(\epsilon)}.
$$

As before, uniformity for $t=O(\epsilon^{-1})$ means a fixed bounded slow-time interval on which the envelope stays bounded. For $k^2>4/5$ it fails when $S(T)$ reaches $\log(5-4/k^2)/(k^2-1)$, with limiting value $4$ at $k=1$. There is no bounded leading approximation covering all such slow times for arbitrary positive $k$.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Use the [Burgers reduction of weakly nonlinear rightgoing acoustics](../../../fluid-mechanics.md#burgers-reduction-of-weakly-nonlinear-rightgoing-acoustics), with $\theta=t-x$, $X=Mx$, $\partial_t=\partial_\theta$ and $\partial_x=-\partial_\theta+M\partial_X$. The [equation of state](../../../thermodynamics.md#equation-of-state) expands as

$$
p=\rho+\frac M2(\gamma-1)\rho^2+O(M^2),\qquad
\rho_1=p_1-\frac{\gamma-1}{2}p_0^2.
$$

At order one, [mass conservation](../../../continuum-mechanics.md#mass-conservation) and [momentum conservation](../../../classical-mechanics.md#momentum-conservation) give $(\rho_0-u_0)_\theta=0$ and $(u_0-p_0)_\theta=0$. For the pure rightgoing [acoustic wave](../../../fluid-mechanics.md#acoustic-wave) with no independent leading mean density or velocity shift, $\rho_0=u_0=p_0$. This is the background choice implicit in the requested traveling-wave expansion; additional mean components would modify its phase convention. The source's duplicated phrase about expanding $p$ should refer to expanding $\rho$ as well as $u$.

At order $M$, the [mass conservation](../../../continuum-mechanics.md#mass-conservation) equation becomes

$$
(\rho_1-u_1)_\theta+p_{0,X}-(p_0^2)_\theta=0,
$$

whereas the [momentum conservation](../../../classical-mechanics.md#momentum-conservation) equation becomes

$$
(u_1-p_1)_\theta+p_{0,X}=0.
$$

In the latter equation, the two nonlinear products $\rho_0u_{0,\theta}$ and $-u_0u_{0,\theta}$ cancel. Substitute the [equation of state](../../../thermodynamics.md#equation-of-state) relation into the former equation and add the two equations to eliminate the first corrections. The result is

$$
\boxed{p_{0,X}-\frac{\gamma+1}{2}p_0p_{0,\theta}=0}.
$$

The same calculation gives $u_1-p_1=-(\gamma+1)p_0^2/4+C(X)$, so the first corrections may be chosen without an explicit secular factor of $\theta$. This is why the retarded-time description can remain uniform for $|\theta|=O(M^{-1})$, provided the leading profile and its relevant [derivatives](../../../calculus.md#derivative) remain bounded over that range and the slow propagation interval.

This [Inviscid Burgers equation](../../../partial-differential-equation.md#inviscid-burgers-equation) can develop a [shock](../../../partial-differential-equation.md#shock-wave), so the source's uniformity assertion needs a pre-shock qualification. If $p_0(\theta,0)=F(\theta)$ and $a=(\gamma+1)/2$, its [method of characteristics](../../../partial-differential-equation.md#method-of-characteristics) gives

$$
p_0=F(s),\qquad \theta=s-aF(s)X,\qquad
p_{0,\theta}=\frac{F'(s)}{1-aXF'(s)}.
$$

The smooth construction ends when this denominator vanishes; if $\max F'>0$, the first such distance is $X_s=[a\max F']^{-1}$.

For viscosity write $\beta=M\nu$ with bounded positive $\nu$. Since $u_{0,xx}=p_{0,\theta\theta}+O(M)$, the order-$M$ [momentum conservation](../../../classical-mechanics.md#momentum-conservation) equation instead reads $(u_1-p_1)_\theta+p_{0,X}=\nu p_{0,\theta\theta}$. Addition now yields the [viscous Burgers equation](../../../partial-differential-equation.md#viscous-burgers-equation)

$$
\boxed{p_{0,X}-\frac{\gamma+1}{2}p_0p_{0,\theta}
=\frac\nu2p_{0,\theta\theta}=\frac\beta{2M}p_{0,\theta\theta}}.
$$

Its positive [diffusion](../../../thermodynamics.md#diffusion) resolves the inviscid steepening rather than supporting an unqualified smooth inviscid expansion through [shock](../../../partial-differential-equation.md#shock-wave) formation.

## 5

↑ **Parent:** [Paper 76](paper-76.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/i">i</h4>

↑ **Parent:** [A](#5/a)

<h5 id="5/a/i/solution">Solution</h5>

↑ **Parent:** [I](#5/a/i)

Assume $\gamma>0$, the [positive diffusivity requirement for the forward heat kernel](../../../diffusion-equation.md#positive-diffusivity-requirement-for-the-forward-heat-kernel). A [normal mode](../../../wave-equation.md#normal-mode) $e^{ikx-i\omega t}$ of the [linear complex Ginzburg-Landau equation](../../../partial-differential-equation.md#linear-complex-ginzburg-landau-equation) gives

$$
D(k,\omega)=-i\omega+iUk-\mu+\gamma k^2=0,\qquad
\omega(k)=Uk+i(\mu-\gamma k^2).
$$

For real $k$, the maximum [temporal growth rate](../../../wave-equation.md#growth-rate) is $\mu$. The [Briggs-Bers criterion](../../../wave-equation.md#briggs-bers-criterion) starts the inverse time [Laplace transform](../../../analysis.md#laplace-transform) above the temporal growth spectrum and follows the two spatial roots as its frequency contour is lowered. A contributing [spatial pinch point](../../../wave-equation.md#spatial-pinch-point) occurs when roots continued from opposite sides of the spatial contour coalesce and prevent its deformation. An arbitrary algebraic saddle is not sufficient without this branch selection.

Here $D=D_k=0$ gives

$$
\boxed{k_0=-\frac{iU}{2\gamma},\qquad
\omega_0=i\left(\mu-\frac{U^2}{4\gamma}\right)}.
$$

To check the pinch, start at $\omega=i\Omega$ with $\Omega$ large. The roots are $k=-iU/(2\gamma)\pm i\sqrt{U^2+4\gamma(\Omega-\mu)}/(2\gamma)$ and initially lie in opposite half-planes. They meet at $\Omega=\mu-U^2/(4\gamma)$, giving the causal saddle. Positive imaginary [absolute frequency](../../../hydrodynamic-stability.md#absolute-frequency) means fixed-position exponential growth. Therefore

$$
\boxed{\text{absolute hydrodynamic instability: }\mu>\frac{U^2}{4\gamma}},\qquad
\boxed{\text{convective hydrodynamic instability: }0<\mu<\frac{U^2}{4\gamma}}.
$$

For $\mu\le0$ there is no positive temporal growth. At $\mu=U^2/(4\gamma)$ the fixed-position exponential rate is zero; its algebraic prefactor, derived below, decays. When $U=0$ the convective interval is empty.

The source specifies only real coefficients. For $\gamma<0$, temporal growth is unbounded at high real [wavenumber](../../../wave-equation.md#wavenumber), so the usual causal forward-diffusion construction is ill posed and the above criterion does not apply. For $\gamma=0$ the equation reduces to transport with amplification; its point impulse remains a moving delta, rather than a spreading [heat kernel](../../../diffusion-equation.md#heat-kernel). These cases cannot be included by division by $\gamma$.

<h4 id="5/a/ii">ii</h4>

↑ **Parent:** [A](#5/a)

<h5 id="5/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#5/a/ii)

Select the [causal Green function](../../../analysis.md#causal-green-function), zero for $t<0$; otherwise the impulse equation permits arbitrary homogeneous additions. Use the spatial [Fourier transform](../../../analysis.md#fourier-transform) convention $e^{-ikx}$ and the temporal [Laplace transform](../../../analysis.md#laplace-transform) boundary convention $e^{i\omega t}$. The transformed impulse equation is

$$
\widehat G(k,\omega)=\frac1{-i\omega+iUk-\mu+\gamma k^2}.
$$

If $\mu>0$, a literal real-frequency [Fourier transform](../../../analysis.md#fourier-transform) of the growing response need not exist. Its causal inverse instead starts on $\operatorname{Im}\omega=c>\max(\mu,0)$ and is continued from there. For $t>0$ close the frequency contour below; its clockwise orientation and the [pole](../../../isolated-singularity.md#pole) [residue](../../../analysis.md#residue) $1/(-i)=i$ give $e^{-i\omega(k)t}$. For $t<0$ the upper closure contains no [pole](../../../isolated-singularity.md#pole). The remaining inverse spatial transform is a [Gaussian integral](../../../calculus.md#gaussian-integral):

$$
G(x,t)=\frac{H(t)e^{\mu t}}{2\pi}\int_{\mathbb R}
 e^{-\gamma tk^2+ik(x-Ut)}\,dk
=\boxed{\frac{H(t)}{\sqrt{4\pi\gamma t}}
\exp\left[\mu t-\frac{(x-Ut)^2}{4\gamma t}\right]}.
$$

The unit-mass [Gaussian heat kernel](../../../diffusion-equation.md#gaussian-heat-kernel) tends to $\delta(x)$ at $t\downarrow0$, giving the required impulse normalization.

At the advected center $x=Ut$, its [amplitude](../../../physics.md#wave-amplitude) is $e^{\mu t}/\sqrt{4\pi\gamma t}$. At a fixed spatial point,

$$
G(x,t)=\frac{e^{Ux/(2\gamma)}}{\sqrt{4\pi\gamma t}}
\exp\left[\left(\mu-\frac{U^2}{4\gamma}\right)t-\frac{x^2}{4\gamma t}\right].
$$

Thus $\mu>0$ permits growth of the moving [wave packet](../../../wave-equation.md#wave-packet), but it is [convective hydrodynamic instability](../../../hydrodynamic-stability.md#convective-hydrodynamic-instability) if the fixed-position rate is negative. A positive fixed-position rate is [absolute hydrodynamic instability](../../../hydrodynamic-stability.md#absolute-hydrodynamic-instability). At its equality threshold the $t^{-1/2}$ factor decays, explaining the marginal exponential classification. This directly verifies the physically selected [Briggs-Bers criterion](../../../wave-equation.md#briggs-bers-criterion) saddle rather than assuming its accessibility.

<h4 id="5/a/iii">iii</h4>

↑ **Parent:** [A](#5/a)

<h5 id="5/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#5/a/iii)

Write $\boldsymbol c=(U,V)^T$ and $\Gamma=\begin{pmatrix}\gamma_{11}&\gamma_{12}\\\gamma_{12}&\gamma_{22}\end{pmatrix}$. A well-posed anisotropic [diffusion](../../../thermodynamics.md#diffusion) problem requires $\Gamma$ to be symmetric positive definite: $\gamma_{11}>0$ and $\Delta=\gamma_{11}\gamma_{22}-\gamma_{12}^2>0$. For the [normal mode](../../../wave-equation.md#normal-mode) in the source the [dispersion relation](../../../wave-equation.md#dispersion-relation) is

$$
\omega=Uk+Vl+i(\mu-\gamma_{11}k^2-2\gamma_{12}kl-\gamma_{22}l^2).
$$

The [group velocity](../../../wave-equation.md#group-velocity) vanishes when $\boldsymbol c-2i\Gamma\boldsymbol k=0$. Consequently

$$
\boldsymbol k_0=-\frac i2\Gamma^{-1}\boldsymbol c,\qquad
\omega_0=i\left(\mu-\frac14\boldsymbol c^T\Gamma^{-1}\boldsymbol c\right).
$$

The requested [anisotropic absolute-instability threshold for positive diffusion](../../../hydrodynamic-stability.md#anisotropic-absolute-instability-threshold-for-positive-diffusion) is

$$
\boxed{\mu>f(U,V),\qquad
f(U,V)=\frac{\gamma_{22}U^2-2\gamma_{12}UV+\gamma_{11}V^2}{4\Delta}}.
$$

For positive definite [diffusion](../../../thermodynamics.md#diffusion) this is also sufficient: the anisotropic [Gaussian heat kernel](../../../diffusion-equation.md#gaussian-heat-kernel) has exponential factor $\exp[\mu t-(\boldsymbol x-\boldsymbol c t)^T\Gamma^{-1}(\boldsymbol x-\boldsymbol c t)/(4t)]$ and a $t^{-1}$ prefactor, so its fixed-position [growth rate](../../../wave-equation.md#growth-rate) is precisely $\mu-f$.

Let the prescribed speed be $q$ and let $d_{\min}\le d_{\max}$ be the positive [eigenvalues](../../../linear-operator-theory.md#eigenvalue) of $\Gamma$. The [Rayleigh quotient](../../../linear-operator-theory.md#rayleigh-quotient) for $\Gamma^{-1}$ gives

$$
\min_{|\boldsymbol c|=q}f=\frac{q^2}{4d_{\max}},\qquad
\max_{|\boldsymbol c|=q}f=\frac{q^2}{4d_{\min}}.
$$

Absence of [absolute hydrodynamic instability](../../../hydrodynamic-stability.md#absolute-hydrodynamic-instability) for every direction therefore requires

$$
\boxed{\mu\le\frac{q^2}{4d_{\max}}}.
$$

**This is an upper bound on $\mu$, not a minimum required value.** The source's last sentence reverses this monotonicity: reducing the growth parameter always helps, so there is no finite lower threshold guaranteeing absence. If it had asked for instability in every direction, the corresponding condition would be $\mu>q^2/(4d_{\min})$. Without the positive-definite assumption, negative [diffusion](../../../thermodynamics.md#diffusion) directions make the forward problem ill posed; a singular [diffusion](../../../thermodynamics.md#diffusion) tensor requires a separate transport analysis and does not support the displayed inverse-matrix formula.

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

Assume again positive [diffusion](../../../thermodynamics.md#diffusion) $\gamma>0$. Remove the drift with $A(x,t)=e^{Ux/(2\gamma)-i\omega t}f(x)$. Differentiating explicitly cancels the first [derivative](../../../calculus.md#derivative) and gives

$$
\gamma f''+\left[\mu_0-\frac{U^2}{4\gamma}-\epsilon\lambda x+i\omega\right]f=0.
$$

Balance the second [derivative](../../../calculus.md#derivative) with the linear confinement by taking $x=O(\epsilon^{-1/3})$, so the requested exponent is **$\sigma=1/3$**. More precisely, put

$$
\xi=\left(\frac{\epsilon\lambda}{\gamma}\right)^{1/3}x,\qquad
\Lambda=(\epsilon^2\gamma\lambda^2)^{1/3},\qquad
c=\frac{\mu_0-U^2/(4\gamma)+i\omega}{\Lambda}.
$$

The [eigenvalue problem](../../../linear-operator-theory.md#eigenvalue-problem) reduces to $f_{\xi\xi}=(\xi-c)f$. Its two solutions are [Airy functions](../../../differential-equation.md#airy-function). The growing $\operatorname{Bi}(\xi-c)$ is excluded by the condition at infinity: its growth proportional to $e^{2\xi^{3/2}/3}$ dominates any linear-in-$x$ drift factor. The decaying $\operatorname{Ai}(\xi-c)$ remains admissible even after multiplication by $e^{Ux/(2\gamma)}$. The wall imposes $\operatorname{Ai}(-c)=0$, so $-c=z_n$, giving the [Airy global modes of a linearly confined Ginzburg-Landau equation](../../../partial-differential-equation.md#airy-global-modes-of-a-linearly-confined-ginzburg-landau-equation):

$$
\boxed{\omega_n=i\left[\mu_0-\frac{U^2}{4\gamma}+\Lambda z_n\right]},\qquad
A_n(x,t)=C_n e^{Ux/(2\gamma)-i\omega_nt}\operatorname{Ai}(\xi+z_n).
$$

The least negative zero, $z_1\simeq-2.338107$, gives the largest temporal [growth rate](../../../wave-equation.md#growth-rate). Hence

$$
\boxed{\text{global instability: }\mu_0>\frac{U^2}{4\gamma}+|z_1|(\epsilon^2\gamma\lambda^2)^{1/3}}.
$$

At equality the leading global [eigenmode](../../../wave-equation.md#normal-mode) is neutral, and below it all these [eigenmodes](../../../wave-equation.md#normal-mode) decay. In contrast, freezing the coefficients locally gives [absolute hydrodynamic instability](../../../hydrodynamic-stability.md#absolute-hydrodynamic-instability) wherever $\mu_0-\epsilon\lambda x>U^2/(4\gamma)$. Such a pocket exists iff $\mu_0>U^2/(4\gamma)$ and extends to $x_a=[\mu_0-U^2/(4\gamma)]/(\epsilon\lambda)$. Thus global instability implies a locally absolutely unstable pocket, while the converse fails: a pocket shorter than $|z_1|(\gamma/(\epsilon\lambda))^{1/3}$ does not overcome the wall and confinement losses. The additional threshold is order $\epsilon^{2/3}$, precisely the loss produced by the [Airy function](../../../differential-equation.md#airy-function) spatial scale.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2004](../../2004.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
