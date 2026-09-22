# Paper 327

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2025/III_Paper_327.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2025/III_Paper_327.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [i](#1/b/i)
      - [Solution](#1/b/i/solution)
    - [ii](#1/b/ii)
      - [Solution](#1/b/ii/solution)
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
    - [v](#2/b/v)
      - [Solution](#2/b/v/solution)
    - [vi](#2/b/vi)
      - [Solution](#2/b/vi/solution)
    - [vii](#2/b/vii)
      - [Solution](#2/b/vii/solution)
    - [viii](#2/b/viii)
      - [Solution](#2/b/viii/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
  - [d](#2/d)
    - [Solution](#2/d/solution)
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
    - [i](#3/b/i)
      - [Solution](#3/b/i/solution)
    - [ii](#3/b/ii)
      - [Solution](#3/b/ii/solution)

## 1

↑ **Parent:** [Paper 327](paper-327.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

For a compact convex set $K\subset\mathbb R^n$, let

$$
H_K(\eta)=\sup_{x\in K}x\mathbin\cdot\eta.
$$

The [Paley–Wiener–Schwartz theorem](../../../distribution-theory.md#paley-wiener-schwartz-theorem) says that if $u$ is a [compactly supported distribution](../../../distribution-theory.md#compactly-supported-distribution) with support in $K$, its Fourier--Laplace transform

$$
\widehat u(z)=\langle u(x),e^{-ix\cdot z}\rangle
$$

is entire and, for some $C,N$,

$$
|\widehat u(z)|\leq C(1+|z|)^N
e^{H_K(\operatorname{Im}z)}.
$$

Conversely, every entire function satisfying such an estimate is the transform of a distribution supported in $K$.

For the forward direction, compact support lets $u$ act on the exponential after insertion of a cutoff equal to one near $K$. Differentiation in $z$ may be passed under the pairing, proving entire analyticity. The finite-order estimate for $u$ bounds derivatives of the exponential on $K$ by a polynomial in $|z|$ times $e^{H_K(\operatorname{Im}z)}$.

Conversely, restrict the entire function $F$ to $\mathbb R^n$. Its polynomial growth defines a [tempered distribution](../../../fourier-analysis.md#tempered-distribution) $u$ by inverse [Fourier transform](../../../analysis.md#fourier-transform). If a test function is supported outside $K$, separate its compact support from $K$ by a real vector $\eta$. Shifting the Fourier inversion contour from $\mathbb R^n$ to $\mathbb R^n+i t\eta$ is allowed by entire analyticity. The exponential gained from the test function beats the bound $e^{tH_K(\eta)}$ as $t\to\infty$, so the pairing vanishes. Hence $\operatorname{supp}u\subset K$, completing the converse.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/i">i</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/i/solution">Solution</h5>

↑ **Parent:** [I](#1/b/i)

If $u\in\mathcal E'(\mathbb R)$ solves $P(D)u=v$, Fourier transformation gives

$$
P(z)\widehat u(z)=\widehat v(z).
$$

The [Paley–Wiener–Schwartz theorem](../../../distribution-theory.md#paley-wiener-schwartz-theorem) makes $\widehat u$ entire, so $\widehat v/P$ is entire.

Conversely, suppose $F(z)=\widehat v(z)/P(z)$ is entire. Polynomial division estimates away from the finitely many zeros of $P$, together with the maximum principle on fixed disks around those zeros, show that $F$ retains a Paley--Wiener--Schwartz bound, with only the polynomial exponent changed. The converse theorem therefore gives $u\in\mathcal E'(\mathbb R)$ with $\widehat u=F$. Then $P(D)u=v$. Thus

$$
\boxed{\exists u\in\mathcal E':P(D)u=v
\iff \widehat v/P\text{ is entire}}.
$$

<h4 id="1/b/ii">ii</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/b/ii)

**No.** Non-entireness rules out a compactly supported solution, but the [Malgrange–Ehrenpreis theorem](../../../distribution-theory.md#malgrange-ehrenpreis-theorem) gives a distributional [fundamental solution of a linear differential operator](../../../distribution-theory.md#fundamental-solution-of-a-linear-differential-operator) $E$ with $P(D)E=\delta$. Since $v$ has compact support, the convolution $u=E*v$ is defined and satisfies

$$
P(D)u=(P(D)E)*v=v.
$$

One may choose a tempered fundamental solution for a constant-coefficient operator, so $u\in\mathcal S'(\mathbb R)$.

## 2

↑ **Parent:** [Paper 327](paper-327.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

The [Sobolev space](../../../sobolev-space.md) $H^s(\mathbb R^n)$ consists of $u\in\mathcal S'(\mathbb R^n)$ for which

$$
\int_{\mathbb R^n}\langle\xi\rangle^{2s}
|\widehat u(\xi)|^2\,d\xi<\infty,
\qquad
\langle\xi\rangle=(1+|\xi|^2)^{1/2}.
$$

The [Local Sobolev space](../../../sobolev-space.md#local-sobolev-space) $H^s_{\rm loc}(X)$ consists of distributions $u$ such that $\chi u\in H^s(\mathbb R^n)$ for every $\chi\in C_c^\infty(X)$.

If $P$ has degree $m$ and principal homogeneous part $P_m$, then $P(D)$ is an [elliptic differential operator](../../../distribution-theory.md#elliptic-differential-operator) when

$$
P_m(\xi)\ne0\qquad(\xi\in\mathbb R^n\setminus\{0\}).
$$

Equivalently, $|P(\xi)|\geq c|\xi|^m$ for all sufficiently large real $\xi$.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/i">i</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/i/solution">Solution</h5>

↑ **Parent:** [I](#2/b/i)

**True.** Multiplication by a [Schwartz function](../../../fourier-analysis.md#schwartz-function) is a bounded map $H^s(\mathbb R^n)\to H^s(\mathbb R^n)$ for every real $s$.

<h4 id="2/b/ii">ii</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/b/ii)

**True.** If $s>t$, then $\langle\xi\rangle^{2t}\leq\langle\xi\rangle^{2s}$, so $H^s(\mathbb R^n)\subset H^t(\mathbb R^n)$ continuously.

<h4 id="2/b/iii">iii</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#2/b/iii)

**False.** Ellipticity concerns the principal part and large frequencies; lower-order terms may create nonzero real roots. For example, $P(\xi)=\xi^2-1$ is elliptic in one dimension but vanishes at $\xi=\pm1$.

<h4 id="2/b/iv">iv</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#2/b/iv)

**True.** Repeated use of the [Leibniz rule](../../../calculus.md#leibniz-rule) and the polynomial Taylor formula gives

$$
\boxed{P(D)(fg)=\sum_\alpha\frac1{\alpha!}
(D^\alpha f)\,P^{(\alpha)}(D)g.}
$$

<h4 id="2/b/v">v</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/v/solution">Solution</h5>

↑ **Parent:** [V](#2/b/v)

**True.** The [Sobolev embedding theorem](../../../sobolev-space.md#sobolev-embedding-theorem) gives $H^s(\mathbb R^n)\hookrightarrow C^0(\mathbb R^n)$ when $s>n/2$.

<h4 id="2/b/vi">vi</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/vi/solution">Solution</h5>

↑ **Parent:** [Vi](#2/b/vi)

**False.** The constant distribution $u=1$ is tempered, but its Fourier transform is a multiple of the [Dirac delta function](../../../distribution-theory.md#dirac-delta-function), which is not an $L^2$ function after multiplication by any Sobolev weight. Thus $1\notin H^t(\mathbb R^n)$ for every $t$.

<h4 id="2/b/vii">vii</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/vii/solution">Solution</h5>

↑ **Parent:** [Vii](#2/b/vii)

**True.** The Fourier transform of a [compactly supported distribution](../../../distribution-theory.md#compactly-supported-distribution) is a smooth function of at most polynomial growth. A sufficiently negative Sobolev weight makes its square integrable, so every $u\in\mathcal E'(\mathbb R^n)$ belongs to $H^t(\mathbb R^n)$ for some $t$.

<h4 id="2/b/viii">viii</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/viii/solution">Solution</h5>

↑ **Parent:** [Viii](#2/b/viii)

**True.** Fourier transformation turns $D^\alpha$ into multiplication by $\xi^\alpha$, and

$$
\langle\xi\rangle^{s-|\alpha|}|\xi^\alpha|
\leq\langle\xi\rangle^s.
$$

**Hence $D^\alpha:H^s\to H^{s-|\alpha|}$ is bounded.**

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

The derivative hypothesis implies that $1/Q(\xi)$ is a symbol of order $-\delta N$ at high frequency. Choose cutoffs $\chi\prec\psi$ in $X$ and a high-frequency cutoff in $\xi$. The corresponding Fourier multiplier is a [parametrix](../../../distribution-theory.md#parametrix) for $Q(D)$, and the [symbol calculus](../../../distribution-theory.md#symbol-calculus), together with the product formula from part (b), gives the localized estimate

$$
\|\chi u\|_{H^{s+\delta N}}
\leq C\left(\|\psi Q(D)u\|_{H^s}
+\|\psi u\|_{H^t}\right)
$$

for some sufficiently negative $t$. The commutator terms contain derivatives $Q^{(\alpha)}$; the assumed factor $|\xi|^{-\delta|\alpha|}$ lowers their order and lets them be absorbed inductively. Therefore

$$
\boxed{Q(D)u\in H^s_{\rm loc}(X)
\Longrightarrow u\in H^{s+\delta N}_{\rm loc}(X)}.
$$

If $Q(D)u$ is smooth, it belongs locally to $H^s$ for every $s$. Starting from the fact that every compactly supported distribution has some negative Sobolev order and repeatedly applying the gain $\delta N>0$ places $u$ in every local Sobolev space. The [Sobolev embedding theorem](../../../sobolev-space.md#sobolev-embedding-theorem) then gives $u\in C^\infty(X)$. Thus $Q(D)$ is a [hypoelliptic differential operator](../../../distribution-theory.md#hypoelliptic-operator).

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

The heat operator

$$
\partial_t-\Delta_x
$$

is hypoelliptic: its symbol $i\tau+|\xi|^2$ satisfies the derivative estimates that yield local regularity by the argument in part (c). It is not elliptic as an operator of total order two, because its principal symbol is $|\xi|^2$, which vanishes at every nonzero covector $(\tau,0)$ with $\tau\ne0$. Hence it is a [hypoelliptic differential operator](../../../distribution-theory.md#hypoelliptic-operator) that is not an [elliptic differential operator](../../../distribution-theory.md#elliptic-differential-operator).

## 3

↑ **Parent:** [Paper 327](paper-327.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

A [phase function](../../../distribution-theory.md#phase-function) is a real smooth function $\Phi$ on $X\times(\mathbb R^k\setminus\{0\})$, positively homogeneous of degree one in $\theta$, with $d_{x,\theta}\Phi\ne0$. The [symbol class](../../../distribution-theory.md#symbol-class)

$$
\operatorname{Sym}(X,\mathbb R^k;N)
$$

consists of smooth amplitudes satisfying, on each compact $K\subset X$,

$$
|D_x^\alpha D_\theta^\beta a(x,\theta)|
\leq C_{K,\alpha,\beta}\langle\theta\rangle^{N-|\beta|}.
$$

To define the [oscillatory integral](../../../distribution-theory.md#oscillatory-integral), insert a cutoff $\chi(\varepsilon\theta)$ equal to one near zero and set

$$
\langle I_\Phi(a),f\rangle
=\lim_{\varepsilon\downarrow0}
\int_X\int_{\mathbb R^k}
e^{i\Phi(x,\theta)}a(x,\theta)f(x)
\chi(\varepsilon\theta)\,d\theta\,dx.
$$

Repeated integration by parts with an operator $L$ satisfying $Le^{i\Phi}=e^{i\Phi}$ makes the integral absolutely convergent after enough iterations and shows that the limit defines a distribution.

<h4 id="3/a/i">i</h4>

↑ **Parent:** [A](#3/a)

<h5 id="3/a/i/solution">Solution</h5>

↑ **Parent:** [I](#3/a/i)

Applying $D_x^\alpha$ changes only the constants in the defining estimates, while each $D_\theta$ lowers the power of $\langle\theta\rangle$ by one. Hence

$$
\boxed{D_x^\alpha D_\theta^\beta a
\in\operatorname{Sym}(X,\mathbb R^k;N-|\beta|)}.
$$

<h4 id="3/a/ii">ii</h4>

↑ **Parent:** [A](#3/a)

<h5 id="3/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/a/ii)

The [Leibniz rule](../../../calculus.md#leibniz-rule) writes every derivative of $a_1a_2$ as a finite sum of products of derivatives of the factors. Multiplying their symbol bounds adds the orders, so

$$
\boxed{a_1a_2\in
\operatorname{Sym}(X,\mathbb R^k;N_1+N_2)}.
$$

<h4 id="3/a/iii">iii</h4>

↑ **Parent:** [A](#3/a)

<h5 id="3/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#3/a/iii)

Differentiating a function positively homogeneous of degree $M$ in $\theta$ makes $D_\theta^\beta b$ homogeneous of degree $M-|\beta|$, while $x$-derivatives preserve the degree. On the unit sphere these derivatives are bounded uniformly over compact subsets of $X$. Scaling then gives

$$
|D_x^\alpha D_\theta^\beta b|
\leq C\langle\theta\rangle^{M-|\beta|}
$$

for large $\theta$; smoothness controls the remaining compact frequency region. Thus

$$
\boxed{b\in\operatorname{Sym}(X,\mathbb R^k;M)}.
$$

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

The [singular support](../../../distribution-theory.md#singular-support) of $u\in\mathcal D'(X)$ is the complement of the largest open subset of $X$ on which $u$ is represented by a smooth function.

<h4 id="3/b/i">i</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/i/solution">Solution</h5>

↑ **Parent:** [I](#3/b/i)

Suppose $x_0$ has a neighborhood on which $\nabla_\theta\Phi(x,\theta)\ne0$ for every $\theta\ne0$. There one may integrate by parts repeatedly with

$$
L=\frac{\nabla_\theta\Phi}
{i|\nabla_\theta\Phi|^2}\mathbin\cdot\nabla_\theta,
\qquad
Le^{i\Phi}=e^{i\Phi}.
$$

Each adjoint application lowers the effective symbol order. After enough repetitions, the integral and all its $x$-derivatives converge absolutely and define a smooth function near $x_0$. Therefore

$$
\boxed{
\operatorname{sing\,supp}I_\Phi(a)
\subset
\{x:\nabla_\theta\Phi(x,\theta)=0
\text{ for some }\theta\ne0\}}.
$$

<h4 id="3/b/ii">ii</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/b/ii)

**The claim is false** because vanishing of the amplitude at one spatial point need not control its derivatives nearby. Take $X=\mathbb R$, $k=1$,

$$
\Phi(x,\theta)=x\theta,
\qquad
a(x,\theta)=x\theta.
$$

Then $0\in Z(a)$, but distributionally

$$
I_\Phi(a)
=x\int_{\mathbb R}e^{ix\theta}\theta\,d\theta
=-2\pi i\,x\delta'(x)
=2\pi i\,\delta(x)
$$

up to the Fourier-transform sign convention. Thus $0$ lies in the [singular support](../../../distribution-theory.md#singular-support) of $I_\Phi(a)$ despite belonging to $Z(a)$.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2025](../../2025.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
