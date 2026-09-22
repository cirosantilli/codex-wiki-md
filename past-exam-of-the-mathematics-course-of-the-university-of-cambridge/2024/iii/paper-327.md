# Paper 327

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2024/Paper_327.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2024/Paper_327.pdf)

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
    - [v](#1/b/v)
      - [Solution](#1/b/v/solution)
    - [vi](#1/b/vi)
      - [Solution](#1/b/vi/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
    - [i](#3/a/i)
      - [Solution](#3/a/i/solution)
    - [ii](#3/a/ii)
      - [Solution](#3/a/ii/solution)
    - [iii](#3/a/iii)
      - [Solution](#3/a/iii/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)

## 1

↑ **Parent:** [Paper 327](paper-327.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/i">i</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/i/solution">Solution</h5>

↑ **Parent:** [I](#1/a/i)

The [Schwartz space](../../../fourier-analysis.md#schwartz-space) on the [real line](../../../real-analysis.md#real-line) is

$$
\mathcal S(\mathbb R)
=\left\{\varphi\in C^\infty(\mathbb R):
p_{m,n}(\varphi)<\infty\text{ for every }m,n\in\mathbb N_0\right\},
\qquad
p_{m,n}(\varphi)=\sup_{x\in\mathbb R}|x^m\varphi^{(n)}(x)|.
$$

These [seminorms](../../../topological-vector-space.md#seminorm) define its [Fréchet space](../../../topological-vector-space.md#frechet-space) topology. The space of [tempered distributions](../../../fourier-analysis.md#tempered-distribution) is its [continuous dual space](../../../continuous-dual-space.md),

$$
\mathcal S'(\mathbb R)=\mathcal S(\mathbb R)^*.
$$

With the angular-frequency convention, the [Fourier transform](../../../analysis.md#fourier-transform) of a [Schwartz function](../../../fourier-analysis.md#schwartz-function) is

$$
\widehat\varphi(\lambda)
=\int_{\mathbb R}e^{-i\lambda x}\varphi(x)\,dx.
$$

It maps $\mathcal S$ continuously to itself. The transform of $u\in\mathcal S'$ is defined through the [dual pairing](../../../continuous-dual-space.md#dual-pairing):

$$
\boxed{\langle\widehat u,\varphi\rangle
=\langle u,\widehat\varphi\rangle},
$$

up to the fixed reflection and $2\pi$ factor if the inverse-transform convention is used for the test function.

<h4 id="1/a/ii">ii</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/a/ii)

For $f\in L^1(\mathbb R)$, its regular [tempered distribution](../../../fourier-analysis.md#tempered-distribution) acts by integration, and the distributional transform agrees with the function

$$
\widehat f(\lambda)=\int_{\mathbb R}f(x)e^{-i\lambda x}\,dx.
$$

The [triangle inequality](../../../topological-analysis.md#triangle-inequality) gives the uniform bound

$$
|\widehat f(\lambda)|\leq\int_{\mathbb R}|f(x)|\,dx=\|f\|_1.
$$

If $\lambda_j\to\lambda$, then $f(x)e^{-i\lambda_jx}\to f(x)e^{-i\lambda x}$ pointwise and every integrand is bounded in absolute value by the [Lebesgue integrable function](../../../measure-theory.md#lebesgue-integrable-function) $|f|$. The [Dominated convergence theorem](../../../measure-theory.md#dominated-convergence-theorem) therefore proves that $\widehat f$ is [continuous](../../../calculus.md#continuous-function). In fact the [Riemann-Lebesgue lemma](../../../fourier-analysis.md#riemann-lebesgue-lemma) also gives $\widehat f(\lambda)\to0$ as $|\lambda|\to\infty$.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/i">i</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/i/solution">Solution</h5>

↑ **Parent:** [I](#1/b/i)

Let

$$
v(\lambda)=-i\int_1^\infty\frac{e^{-i\lambda x}}{x^2}\,dx.
$$

The integral is [absolutely convergent](../../../real-analysis.md#absolute-convergence). For a [Schwartz function](../../../fourier-analysis.md#schwartz-function) $\varphi$, [Fubini's theorem](../../../measure-theory.md#fubini-s-theorem) and [integration by parts](../../../calculus.md#integration-by-parts) in $\lambda$ give

$$
\begin{aligned}
\int_{\mathbb R}\varphi'(\lambda)v(\lambda)\,d\lambda
&=-i\int_1^\infty\frac1{x^2}
\left(\int_{\mathbb R}\varphi'(\lambda)e^{-i\lambda x}\,d\lambda\right)dx\\
&=-\int_1^\infty\frac1x
\left(\int_{\mathbb R}\varphi(\lambda)e^{-i\lambda x}\,d\lambda\right)dx\\
&=\langle\widehat u,\varphi\rangle.
\end{aligned}
$$

Equivalently, $v'=-\widehat u$ as a [distributional derivative](../../../distribution-theory.md#distributional-derivative), and hence

$$
\boxed{\langle\widehat u,\varphi\rangle
=\int_{\mathbb R}\varphi'(\lambda)v(\lambda)\,d\lambda}.
$$

<h4 id="1/b/ii">ii</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/b/ii)

Because $x^{-2}$ is [integrable](../../../measure-theory.md#lebesgue-integrable-function) on $[1,\infty)$, the [Dominated convergence theorem](../../../measure-theory.md#dominated-convergence-theorem) applied to the defining integral proves that $v$ is [continuous](../../../calculus.md#continuous-function) on $\mathbb R$.

For $\lambda>0$, the [change of variables formula](../../../calculus.md#change-of-variables-formula) $t=\lambda x$ gives

$$
v(\lambda)=-i\lambda\int_\lambda^\infty\frac{e^{-it}}{t^2}\,dt,
$$

and for $\lambda<0$ the analogous formula is obtained with $e^{it}$. On either open half-line the lower endpoint stays away from zero locally, so repeated [differentiation under the integral sign](../../../analysis.md#differentiation-under-the-integral-sign) proves smoothness. Thus

$$
\boxed{v\in C(\mathbb R)\cap C^\infty(\mathbb R\setminus\{0\})}.
$$

<h4 id="1/b/iii">iii</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#1/b/iii)

For $0<\lambda<1$, the preceding change of variables and one [integration by parts](../../../calculus.md#integration-by-parts) give

$$
v(\lambda)
=-ie^{-i\lambda}-\lambda\int_\lambda^\infty\frac{e^{-ix}}x\,dx.
$$

Split the last [improper integral](../../../real-analysis.md#improper-integral) at one and add and subtract one on $(\lambda,1)$. Since $\int_\lambda^1dx/x=-\log\lambda$,

$$
\boxed{
v(\lambda)=\lambda\log|\lambda|-ie^{-i\lambda}
-\lambda\left[
\int_\lambda^1\frac{e^{-ix}-1}{x}\,dx
+\int_1^\infty\frac{e^{-ix}}x\,dx
\right]}.
$$

The definition also gives the [complex conjugate](../../../complex-analysis.md#complex-conjugate) relation

$$
v(-\lambda)=-\overline{v(\lambda)}.
$$

Consequently, for $-1<\lambda<0$,

$$
\boxed{
v(\lambda)=\lambda\log|\lambda|-ie^{-i\lambda}
-\lambda\left[
\int_{|\lambda|}^1\frac{e^{ix}-1}{x}\,dx
+\int_1^\infty\frac{e^{ix}}x\,dx
\right]}.
$$

<h4 id="1/b/iv">iv</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#1/b/iv)

On either open half-line, part (i) says $\widehat u=-v'$. Differentiating the formula in part (iii) makes all elementary terms cancel except the [logarithm](../../../calculus.md#logarithm) and the bracket. Therefore

$$
\widehat u(\lambda)=-\log|\lambda|+f_+(\lambda),
\qquad \lambda>0,
$$

where

$$
f_+(\lambda)=
\int_\lambda^1\frac{e^{-ix}-1}{x}\,dx
+\int_1^\infty\frac{e^{-ix}}x\,dx,
$$

and

$$
\widehat u(\lambda)=-\log|\lambda|+f_-(\lambda),
\qquad \lambda<0,
$$

where

$$
f_-(\lambda)=
\int_{|\lambda|}^1\frac{e^{ix}-1}{x}\,dx
+\int_1^\infty\frac{e^{ix}}x\,dx.
$$

Both functions are [smooth](../../../analysis.md#smooth-function) on their respective half-lines, proving the required assertion.

<h4 id="1/b/v">v</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/v/solution">Solution</h5>

↑ **Parent:** [V](#1/b/v)

For $\lambda>0$, subtracting the two formulas from part (iv) yields

$$
f_+(\lambda)-f_-(-\lambda)
=\int_\lambda^\infty
\frac{e^{-ix}-e^{ix}}x\,dx
=-2i\int_\lambda^\infty\frac{\sin x}{x}\,dx.
$$

Using the stated [Dirichlet integral](../../../fourier-analysis.md#dirichlet-integral) and taking the [one-sided limit](../../../calculus.md#one-sided-limit) gives

$$
\boxed{
\lim_{\lambda\downarrow0}
\bigl[f_+(\lambda)-f_-(-\lambda)\bigr]
=-2i\frac\pi2=-i\pi}.
$$

<h4 id="1/b/vi">vi</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/vi/solution">Solution</h5>

↑ **Parent:** [Vi](#1/b/vi)

Remove the two reciprocal tails by setting

$$
r(x)=w(x)-c_+u(x)+c_-u(-x).
$$

The assumed $O(x^{-2})$ remainder at each end and [local integrability](../../../distribution-theory.md#locally-integrable-function) on bounded intervals imply $r\in L^1(\mathbb R)$. Its [Fourier transform](../../../analysis.md#fourier-transform) $\widehat r$ is therefore [continuous](../../../calculus.md#continuous-function) at zero. Since $\widehat{u(-\mathord\cdot)}(\lambda)=\widehat u(-\lambda)$,

$$
\widehat w(\lambda)
=c_+\widehat u(\lambda)-c_-\widehat u(-\lambda)+\widehat r(\lambda).
$$

Parts (iv) and (v) show that both requested one-sided limits exist. If $L_+$ denotes the limit from positive frequencies and $L_-$ the limit from negative frequencies, then the common value $\widehat r(0)$ cancels and

$$
\begin{aligned}
L_+-L_-
&=(c_++c_-)
\lim_{\lambda\downarrow0}
\bigl[f_+(\lambda)-f_-(-\lambda)\bigr]\\
&=\boxed{-i\pi(c_++c_-)}.
\end{aligned}
$$

This is the [universal jump caused by reciprocal tails](../../../analysis.md#fourier-transform-of-a-function-with-reciprocal-tails).

## 2

↑ **Parent:** [Paper 327](paper-327.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

The [space of test functions](../../../distribution-theory.md#space-of-test-functions) is

$$
\mathcal D(\mathbb R^n)=C_c^\infty(\mathbb R^n).
$$

A sequence $\varphi_j$ converges to $\varphi$ in $\mathcal D$ when all supports lie eventually in one [compact set](../../../topology.md#compact-space) $K$ and

$$
\sup_{x\in K}|D^\alpha(\varphi_j-\varphi)(x)|\longrightarrow0
$$

for every [multi-index](../../../distribution-theory.md#multi-index-notation) $\alpha$. A [distribution](../../../distribution-theory.md#distribution-mathematical-analysis) is a [linear functional](../../../linear-algebra.md#linear-functional) $u:\mathcal D\to\mathbb C$ such that, for every compact $K$, there are $C_K>0$ and $m_K\in\mathbb N_0$ with

$$
|\langle u,\varphi\rangle|
\leq C_K\max_{|\alpha|\leq m_K}
\sup_{x\in K}|D^\alpha\varphi(x)|
$$

whenever $\operatorname{supp}\varphi\subseteq K$. Convergence in $\mathcal D'$ is [pointwise convergence on test functions](../../../distribution-theory.md#weak-convergence-of-distributions).

Continuity plainly implies sequential continuity. Conversely, suppose the linear form is sequentially continuous but the displayed estimate fails for some compact $K$. For every $j$, choose $\varphi_j$ supported in $K$ such that

$$
\max_{|\alpha|\leq j}\sup_K|D^\alpha\varphi_j|\leq\frac1j,
\qquad
|\langle u,\varphi_j\rangle|\geq1.
$$

Then $\varphi_j\to0$ in $\mathcal D$, while $u(\varphi_j)\not\to0$, a contradiction. Hence the seminorm estimate holds on every compact set and $u\in\mathcal D'$.

For a [translation vector](../../../vector-space.md#vector) $h$ and a [multi-index](../../../distribution-theory.md#multi-index-notation) $\alpha$, define

$$
\langle\tau_hu,\varphi\rangle
=\langle u,\varphi(\mathord\cdot+h)\rangle,
\qquad
\langle D^\alpha u,\varphi\rangle
=(-1)^{|\alpha|}\langle u,D^\alpha\varphi\rangle.
$$

These definitions extend ordinary [translation](../../../distribution-theory.md#translation-of-a-distribution) and [differentiation](../../../calculus.md#derivative) to distributions.

If $\tau_{te_i}u=u$ for every $t$, differentiating its pairing at $t=0$ gives $\partial_i u=0$. Conversely, if $\partial_i u=0$, then for every test function

$$
\frac d{dt}\langle\tau_{te_i}u,\varphi\rangle
=\langle u,\partial_i\varphi(\mathord\cdot+te_i)\rangle
=-\langle\partial_i u,\varphi(\mathord\cdot+te_i)\rangle=0.
$$

The pairing is constant in $t$, hence $\tau_{te_i}u=u$. This proves both directions of [translation invariance and vanishing distributional derivative](../../../distribution-theory.md#translation-invariance-and-vanishing-distributional-derivative).

Finally, the [distributional differentiation](../../../distribution-theory.md#distributional-derivative) obeys the linear [chain rule](../../../calculus.md#chain-rule) under the linear coordinates $s=x-y$ and $t=x+y$. Thus

$$
\partial_x^2 f(x-y)=f''(x-y)=\partial_y^2 f(x-y)
$$

and likewise

$$
\partial_x^2 g(x+y)=g''(x+y)=\partial_y^2 g(x+y)
$$

as distributions. Adding the two identities gives

$$
\boxed{u_{xx}-u_{yy}=0},
$$

the [one-dimensional wave equation](../../../wave-equation.md#one-dimensional-wave-equation); this is the low-regularity form of the travelling waves in the [D'Alembert formula](../../../wave-equation.md#d-alembert-s-formula).

## 3

↑ **Parent:** [Paper 327](paper-327.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

A [phase function](../../../distribution-theory.md#phase-function) is a real [smooth function](../../../analysis.md#smooth-function) $\Phi$ on $X\times(\mathbb R^k\setminus\{0\})$ that is [positively homogeneous](../../../real-analysis.md#positively-homogeneous-function-degree-one) of degree one in $\theta$ and has nonzero total differential $d_{x,\theta}\Phi$. The [symbol class](../../../distribution-theory.md#symbol-class)

$$
\operatorname{Sym}(X,\mathbb R^k;N)
$$

consists of smooth amplitudes for which, for every compact $K\subset X$ and all [multi-indices](../../../distribution-theory.md#multi-index-notation) $\alpha,\beta$,

$$
|D_x^\alpha D_\theta^\beta a(x,\theta)|
\leq C_{K,\alpha,\beta}\langle\theta\rangle^{N-|\beta|}.
$$

Choose a [smooth cutoff function](../../../analysis.md#smooth-cutoff-function) $\chi$ equal to one near zero. The associated [oscillatory integral](../../../distribution-theory.md#oscillatory-integral) is defined on a [test function](../../../distribution-theory.md#test-function) $f$ by

$$
\langle I_\Phi(a),f\rangle
=\lim_{\varepsilon\downarrow0}
\int_X\int_{\mathbb R^k}
e^{i\Phi(x,\theta)}a(x,\theta)f(x)
\chi(\varepsilon\theta)\,d\theta\,dx.
$$

On the compact $x$-support of $f$, use an integration-by-parts operator $L$ satisfying $Le^{i\Phi}=e^{i\Phi}$. Repeated application of its formal adjoint lowers the effective symbol order until the integral is absolutely convergent. The resulting bounds involve only finitely many derivatives of $f$, prove that the limit is independent of $\chi$, and give the seminorm estimate required for

$$
\boxed{I_\Phi(a)\in\mathcal D'(X)}.
$$

<h4 id="3/a/i">i</h4>

↑ **Parent:** [A](#3/a)

<h5 id="3/a/i/solution">Solution</h5>

↑ **Parent:** [I](#3/a/i)

Applying $D_x^\alpha$ changes only the constants in the defining symbol estimates, while every $D_\theta$ lowers the power of $\langle\theta\rangle$ by one. Hence

$$
\boxed{D_x^\alpha D_\theta^\beta a
\in\operatorname{Sym}(X,\mathbb R^k;N-|\beta|)}.
$$

<h4 id="3/a/ii">ii</h4>

↑ **Parent:** [A](#3/a)

<h5 id="3/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/a/ii)

The [Leibniz rule](../../../calculus.md#leibniz-rule) writes every derivative of $a_1a_2$ as a finite sum of products of derivatives of the two factors. Multiplying the corresponding symbol estimates adds their orders, so

$$
\boxed{a_1a_2\in
\operatorname{Sym}(X,\mathbb R^k;N_1+N_2)}.
$$

<h4 id="3/a/iii">iii</h4>

↑ **Parent:** [A](#3/a)

<h5 id="3/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#3/a/iii)

If $b$ is [positively homogeneous](../../../real-analysis.md#positively-homogeneous-function-degree-one) of degree $M$ for large $|\theta|$, then $D_\theta^\beta b$ is positively homogeneous of degree $M-|\beta|$, while $x$-derivatives preserve the degree. These derivatives are uniformly bounded on the [unit sphere](../../../topology.md#unit-sphere) when $x$ ranges over a compact subset of $X$. Rescaling $\theta$ gives

$$
|D_x^\alpha D_\theta^\beta b(x,\theta)|
\leq C_{K,\alpha,\beta}
\langle\theta\rangle^{M-|\beta|}
$$

at large frequency, and smoothness controls the remaining compact region. Therefore

$$
\boxed{b\in\operatorname{Sym}(X,\mathbb R^k;M)}.
$$

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

For a [test function](../../../distribution-theory.md#test-function) $f\in\mathcal D(\mathbb R)$, define the proposed integral by reversing the order of integration:

$$
\langle I,f\rangle
=\int_{\mathbb R}
\left(\int_{\mathbb R}f(x)e^{ix\sqrt{\theta^2+1}}\,dx\right)d\theta
=\int_{\mathbb R}
\widehat f\bigl(-\sqrt{\theta^2+1}\bigr)\,d\theta.
$$

The [Fourier transform](../../../analysis.md#fourier-transform) of a test function is a [Schwartz function](../../../fourier-analysis.md#schwartz-function), while $\sqrt{\theta^2+1}\asymp1+|\theta|$. The final integral is consequently [absolutely convergent](../../../real-analysis.md#absolute-convergence). Repeated [integration by parts](../../../calculus.md#integration-by-parts) in $x$ bounds it by finitely many [seminorms](../../../topological-vector-space.md#seminorm) of the test function, so it defines a [continuous linear functional](../../../continuous-dual-space.md) on $\mathcal D(\mathbb R)$.

Equivalently, put $\lambda=\sqrt{\theta^2+1}$ on the two half-lines. Then

$$
\langle I,f\rangle
=2\int_1^\infty
\widehat f(-\lambda)
\frac{\lambda}{\sqrt{\lambda^2-1}}\,d\lambda.
$$

The density has only an integrable inverse-square-root singularity at one and is bounded at infinity, so it is a regular [tempered distribution](../../../fourier-analysis.md#tempered-distribution). Its inverse [Fourier transform](../../../analysis.md#fourier-transform) is exactly the proposed oscillatory integral. Thus

$$
\boxed{\int_{\mathbb R}e^{ix\sqrt{\theta^2+1}}\,d\theta
\in\mathcal D'(\mathbb R)}.
$$

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2024](../../2024.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
