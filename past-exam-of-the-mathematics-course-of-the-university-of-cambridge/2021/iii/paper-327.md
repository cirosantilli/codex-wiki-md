# Paper 327

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2021/paper_327.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2021/paper_327.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
  - [i](#2/i)
    - [Solution](#2/i/solution)
  - [ii](#2/ii)
    - [Solution](#2/ii/solution)
- [3](#3)
  - [Solution](#3/solution)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
  - [d](#3/d)
    - [Solution](#3/d/solution)

## 1

↑ **Parent:** [Paper 327](paper-327.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

The [space of test functions](../../../distribution-theory.md#space-of-test-functions) is

$$
\mathcal D(\mathbb R)=C_c^\infty(\mathbb R).
$$

A sequence $\varphi_m$ converges to $\varphi$ in $\mathcal D(\mathbb R)$ when all supports lie in one [compact set](../../../topology.md#compact-space) $K$ and

$$
\sup_{x\in K}|\varphi_m^{(j)}(x)-\varphi^{(j)}(x)|\longrightarrow0
$$

for every [nonnegative integer](../../../arithmetic.md#natural-number) $j$. The [distribution](../../../distribution-theory.md#distribution-mathematical-analysis) space $\mathcal D'(\mathbb R)$ is the [continuous dual space](../../../continuous-dual-space.md) of $\mathcal D(\mathbb R)$, and $u_m\to u$ in $\mathcal D'$ means

$$
\langle u_m,\varphi\rangle\longrightarrow\langle u,\varphi\rangle
$$

for every test function $\varphi$.

If a linear form $u$ is continuous, it clearly maps every [null sequence](../../../real-analysis.md#null-sequence) to a scalar sequence tending to zero. Conversely, suppose it has this sequential property. For each compact $K$, its restriction to the [Fréchet space](../../../topological-vector-space.md#frechet-space) $\mathcal D_K$ must be continuous: otherwise, for every $m$ one could choose $\varphi_m\in\mathcal D_K$ such that

$$
\max_{0\leq j\leq m}\|\varphi_m^{(j)}\|_\infty\leq\frac1m,
\qquad
|\langle u,\varphi_m\rangle|\geq1.
$$

Then $\varphi_m\to0$ in $\mathcal D$ but its images do not tend to zero, a contradiction. Continuity on every $\mathcal D_K$ is precisely continuity for the [strict inductive limit topology](../../../topological-vector-space.md#strict-inductive-limit-topology) of $\mathcal D$, so $u\in\mathcal D'$.

Use the convention $\tau_h\varphi(x)=\varphi(x-h)$. Translation and the [distributional derivative](../../../distribution-theory.md#distributional-derivative) are defined by

$$
\langle\tau_hu,\varphi\rangle
=\langle u,\tau_{-h}\varphi\rangle,
\qquad
\langle u',\varphi\rangle=-\langle u,\varphi'\rangle.
$$

Translation, differentiation, and multiplication by $-1$ are continuous maps on $\mathcal D$, so these formulas define continuous linear functionals and hence distributions.

For fixed $\varphi$, the [difference quotient](../../../calculus.md#difference-quotient) satisfies

$$
\frac{\tau_h\varphi-\varphi}{h}\longrightarrow-\varphi'
\quad\text{in }\mathcal D.
$$

Therefore

$$
\left\langle\frac{\tau_{-h}u-u}{h},\varphi\right\rangle
=\left\langle u,\frac{\tau_h\varphi-\varphi}{h}\right\rangle
\longrightarrow-\langle u,\varphi'\rangle
=\langle u',\varphi\rangle,
$$

which proves $u'=\lim_{h\to0}(\tau_{-h}u-u)/h$ in $\mathcal D'$.

For $-1<\lambda<0$, integration by parts after subtracting the value at zero gives

$$
\boxed{
\langle(x_+^\lambda)',\varphi\rangle
=\int_0^\infty[\varphi(x)-\varphi(0)]\lambda x^{\lambda-1}\,dx}.
$$

The subtraction makes the integrand locally integrable at zero, and $x^\lambda\to0$ handles the other boundary.

The analogous [Hadamard finite-part integral](../../../distribution-theory.md#hadamard-finite-part-integral) is

$$
\boxed{
\langle(\log x_+)',\varphi\rangle
=\int_0^1\frac{\varphi(x)-\varphi(0)}x\,dx
+\int_1^\infty\frac{\varphi(x)}x\,dx}.
$$

Indeed, integrating from $\varepsilon$ and combining the boundary term $\varphi(\varepsilon)\log\varepsilon$ with the divergent constant part of the integral gives this limit.

Because $x_+^\lambda$ is a [locally integrable function](../../../distribution-theory.md#locally-integrable-function), its first distributional derivative has order at most one. It is not of order zero. Choose $\psi\in\mathcal D((0,1))$ with $\int_0^1\lambda t^{\lambda-1}\psi(t)\,dt\ne0$ and put $\psi_\varepsilon(x)=\psi(x/\varepsilon)$. The sup norms stay bounded while

$$
\langle(x_+^\lambda)',\psi_\varepsilon\rangle
=\varepsilon^\lambda
\int_0^1\lambda t^{\lambda-1}\psi(t)\,dt
$$

is unbounded as $\varepsilon\downarrow0$. This contradicts the local sup-norm estimate required of an [order-zero distribution](../../../distribution-theory.md#order-zero-distribution). Hence $(x_+^\lambda)'$ has order exactly $\boxed{1}$.

## 2

↑ **Parent:** [Paper 327](paper-327.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

A [phase function](../../../distribution-theory.md#phase-function) is a real smooth function

$$
\Phi:X\times(\mathbb R^k\setminus\{0\})\to\mathbb R
$$

that is [positively homogeneous](../../../real-analysis.md#positively-homogeneous-function-degree-one) of degree one in $\theta$ and has no critical point in all variables:

$$
\Phi(x,t\theta)=t\Phi(x,\theta),
\qquad
\nabla_{x,\theta}\Phi(x,\theta)\ne0.
$$

The [symbol class](../../../distribution-theory.md#symbol-class) $\operatorname{Sym}(X,\mathbb R^k;N)$ consists of all $a\in C^\infty(X\times\mathbb R^k)$ such that, for every compact $K\Subset X$ and [multi-indices](../../../distribution-theory.md#multi-index-notation) $\alpha,\beta$,

$$
|D_x^\alpha D_\theta^\beta a(x,\theta)|
\leq C_{K,\alpha,\beta}(1+|\theta|)^{N-|\beta|}.
$$

For a cutoff $\chi\in C_c^\infty(\mathbb R^k)$ equal to one near zero, define the [oscillatory integral](../../../distribution-theory.md#oscillatory-integral) by

$$
\boxed{
\langle I_\Phi(a),\psi\rangle
=\lim_{\varepsilon\downarrow0}
\int_X\int_{\mathbb R^k}
e^{i\Phi(x,\theta)}a(x,\theta)\psi(x)\chi(\varepsilon\theta)
\,d\theta\,dx}.
$$

Repeated [integration by parts](../../../calculus.md#integration-by-parts) makes the limit meaningful and independent of the cutoff.

The [singular support](../../../distribution-theory.md#singular-support) is the complement of the largest open set on which the distribution is represented by a [smooth function](../../../analysis.md#smooth-function). Suppose $x_0$ does not belong to

$$
C_\Phi=\{x:\nabla_\theta\Phi(x,\theta)=0
\text{ for some }\theta\ne0\}.
$$

On a sufficiently small neighborhood of $x_0$, homogeneity and compactness of the unit sphere give a lower bound for $|\nabla_\theta\Phi|$. The differential operator

$$
L=\frac{\nabla_\theta\Phi\mathbin\cdot\nabla_\theta}
{i|\nabla_\theta\Phi|^2}
$$

satisfies $Le^{i\Phi}=e^{i\Phi}$. Repeatedly transferring $L$ to the amplitude lowers its symbol order until the integral and all its $x$-derivatives converge absolutely. Hence $I_\Phi(a)$ is smooth near $x_0$, proving

$$
\boxed{\operatorname{sing\,supp}I_\Phi(a)\subseteq C_\Phi}.
$$

For the stated distribution on $\mathbb R^3$, rotational symmetry lets us align the polar axis with $x$ and write $\rho=|x|$. The angular integral is

$$
\int_0^{2\pi}\int_0^\pi
e^{ir\rho\cos\theta}\sin\theta\,d\theta\,d\phi
=4\pi\frac{\sin(r\rho)}{r\rho}.
$$

Therefore, for $\rho>0$,

$$
\begin{aligned}
u(x)
&=\frac1{2\pi}\frac{4\pi}{\rho}
\int_0^\infty\frac{r\sin(r\rho)}{1+r^2}\,dr\\
&=\boxed{\frac{\pi e^{-\rho}}{\rho}}.
\end{aligned}
$$

The original amplitude is not [Lebesgue integrable](../../../measure-theory.md#lebesgue-integrable-function) in $k$, so this computation illustrates how oscillation assigns a distribution to a divergent ordinary integral. The result is smooth away from the origin and has singular support $\{0\}$. It is a constant multiple of the three-dimensional [Yukawa potential](../../../electromagnetism.md#yukawa-potential), satisfying $(-\Delta+1)u=4\pi^2\delta_0$ with the normalization used in the question.

<h3 id="2/i">i</h3>

↑ **Parent:** [2](#2)

<h4 id="2/i/solution">Solution</h4>

↑ **Parent:** [I](#2/i)

Differentiation in $x$ does not change the allowed growth order in $\theta$, while every $\theta$-derivative lowers it by one. More precisely, for further multi-indices $\gamma,\delta$,

$$
|D_x^\gamma D_\theta^\delta(D_x^\alpha D_\theta^\beta a)|
=|D_x^{\alpha+\gamma}D_\theta^{\beta+\delta}a|
\leq C(1+|\theta|)^{N-|\beta|-|\delta|}.
$$

Thus

$$
\boxed{D_x^\alpha D_\theta^\beta a
\in\operatorname{Sym}(X,\mathbb R^k;N-|\beta|)}.
$$

<h3 id="2/ii">ii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#2/ii)

The multivariable [Leibniz rule](../../../calculus.md#leibniz-rule) writes each derivative of $a_1a_2$ as a finite sum of products

$$
(D_x^{\alpha_1}D_\theta^{\beta_1}a_1)
(D_x^{\alpha_2}D_\theta^{\beta_2}a_2),
\qquad
\beta_1+\beta_2=\beta.
$$

Each term is bounded by a constant times

$$
(1+|\theta|)^{N_1-|\beta_1|}
(1+|\theta|)^{N_2-|\beta_2|}
=(1+|\theta|)^{N_1+N_2-|\beta|}.
$$

Hence

$$
\boxed{a_1a_2\in\operatorname{Sym}(X,\mathbb R^k;N_1+N_2)}.
$$

## 3

↑ **Parent:** [Paper 327](paper-327.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

Using [multi-index notation](../../../distribution-theory.md#multi-index-notation), the [Schwartz space](../../../fourier-analysis.md#schwartz-space) is

$$
\mathcal S(\mathbb R^n)
=\left\{\varphi\in C^\infty:
p_{\alpha,\beta}(\varphi)
=\sup_x|x^\alpha D^\beta\varphi(x)|<\infty
\text{ for all }\alpha,\beta\right\}.
$$

Its topology is generated by the displayed [seminorms](../../../topological-vector-space.md#seminorm). The [tempered distribution](../../../fourier-analysis.md#tempered-distribution) $\mathcal S'(\mathbb R^n)$ is its continuous dual, with weak convergence defined by convergence of every pairing with a Schwartz function.

For the convention

$$
\widehat\varphi(\lambda)
=\int_{\mathbb R^n}e^{-i\lambda\cdot x}\varphi(x)\,dx,
$$

differentiation under the integral and [integration by parts](../../../calculus.md#integration-by-parts) give

$$
D_\lambda^\alpha\widehat\varphi
=\widehat{(-ix)^\alpha\varphi},
\qquad
\lambda^\beta\widehat\varphi
=\widehat{(-iD_x)^\beta\varphi}.
$$

These identities bound every Schwartz seminorm of $\widehat\varphi$ by finitely many seminorms of $\varphi$, proving continuity. The [Fourier inversion theorem](../../../fourier-analysis.md#fourier-inversion-theorem) gives the continuous inverse

$$
\varphi(x)=\frac1{(2\pi)^n}
\int e^{i\lambda\cdot x}\widehat\varphi(\lambda)\,d\lambda,
$$

so the [Fourier transform](../../../analysis.md#fourier-transform) is a continuous isomorphism of $\mathcal S$. By duality,

$$
\langle\widehat u,\varphi\rangle
=\langle u,\widehat\varphi\rangle
$$

defines a continuous isomorphism of $\mathcal S'$.

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

For $\omega\ne0$, insert the Gaussian damping factor $e^{-\varepsilon x^2/2}$ and use the [Gaussian integral](../../../calculus.md#gaussian-integral):

$$
\int_{\mathbb R}
e^{-(\varepsilon-i\omega)x^2/2-i\lambda x}\,dx
=\sqrt{\frac{2\pi}{\varepsilon-i\omega}}
\exp\left[-\frac{\lambda^2}{2(\varepsilon-i\omega)}\right].
$$

Taking $\varepsilon\downarrow0$ in $\mathcal S'$ with the continuous square-root branch gives the [Fresnel integral](../../../analysis.md#fresnel-integral)

$$
\boxed{
\mathcal F\left[e^{i\omega x^2/2}\right](\lambda)
=\sqrt{\frac{2\pi}{|\omega|}}
e^{i\pi\operatorname{sgn}(\omega)/4}
e^{-i\lambda^2/(2\omega)}}.
$$

For $\omega=0$, the function is constant and its Fourier transform is $\boxed{2\pi\delta_0}$.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

For a locally integrable $u$, the [change of variables formula](../../../calculus.md#change-of-variables-formula) $y=Ax$ gives

$$
\int_{\mathbb R^n}u(Ax)\varphi(x)\,dx
=\frac1{|\det A|}
\int_{\mathbb R^n}u(y)\varphi(A^{-1}y)\,dy.
$$

This motivates

$$
\boxed{
\langle A^*u,\varphi\rangle
=\frac1{|\det A|}
\langle u,(A^{-1})^*\varphi\rangle}.
$$

Because pullback by an invertible linear map acts continuously on the [Schwartz space](../../../fourier-analysis.md#schwartz-space), the right side is a continuous linear functional of $\varphi$. It therefore defines a [tempered distribution](../../../fourier-analysis.md#tempered-distribution) and agrees with ordinary pullback when $u$ is a function.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

For every $\varphi\in\mathcal S$, the [change of variables formula](../../../calculus.md#change-of-variables-formula) gives the identity

$$
\widehat{(A^t)^*\varphi}(x)
=\frac1{|\det A|}\widehat\varphi(A^{-1}x).
$$

Using this, the distributional Fourier transform, and the pullback formula from part b,

$$
\begin{aligned}
\langle\widehat{A^*u},\varphi\rangle
&=\frac1{|\det A|}
\langle u,(A^{-1})^*\widehat\varphi\rangle\\
&=\langle u,\widehat{(A^t)^*\varphi}\rangle
=\langle\widehat u,(A^t)^*\varphi\rangle\\
&=\left\langle
\frac{((A^t)^{-1})^*\widehat u}{|\det A|},
\varphi\right\rangle.
\end{aligned}
$$

Therefore

$$
\boxed{\widehat{A^*u}
=\frac{((A^t)^{-1})^*\widehat u}{|\det A|}}.
$$

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

By the [spectral theorem for real symmetric matrices](../../../linear-algebra.md#spectral-theorem-for-real-symmetric-matrices), write $A=O^tDO$ with $O$ [orthogonal](../../../linear-algebra.md#orthogonal-matrix) and $D=\operatorname{diag}(\xi_1,\ldots,\xi_n)$. Part a and the tensor-product property of the [Fourier transform](../../../analysis.md#fourier-transform) give

$$
\mathcal F\left[e^{iDx\cdot x/2}\right](\lambda)
=\prod_{j=1}^n
\left(
\sqrt{\frac{2\pi}{|\xi_j|}}
e^{i\pi\operatorname{sgn}(\xi_j)/4}
e^{-i\lambda_j^2/(2\xi_j)}
\right).
$$

Thus

$$
\mathcal F\left[e^{iDx\cdot x/2}\right](\lambda)
=\sqrt{\frac{(2\pi)^n}{|\det D|}}
\exp\left[
\frac{i\pi}{4}\operatorname{sgn}(D)
-\frac i2D^{-1}\lambda\cdot\lambda
\right].
$$

Applying the pullback rule from part c to the orthogonal change of variables, for which $|\det O|=1$, replaces $D$ by $A$ and $D^{-1}$ by $A^{-1}$. Since determinant and [signature](../../../linear-algebra.md#signature-of-a-quadratic-form) are invariant under orthogonal conjugation,

$$
\boxed{
\left[e^{iAx\cdot x/2}\right]^{\widehat{}}(\lambda)
=\sqrt{\frac{(2\pi)^n}{|\det A|}}
\exp\left[
\frac{i\pi}{4}\operatorname{sgn}(A)
-\frac i2(A^{-1}\lambda)\cdot\lambda
\right]}.
$$

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2021](../../2021.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
