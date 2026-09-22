# Paper 203

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2024/Paper_203.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2024/Paper_203.pdf)

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
  - [d](#1/d)
    - [Solution](#1/d/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
  - [d](#2/d)
    - [Solution](#2/d/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
  - [d](#3/d)
    - [Solution](#3/d/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [Solution](#4/c/solution)
  - [d](#4/d)
    - [Solution](#4/d/solution)

## 1

↑ **Parent:** [Paper 203](paper-203.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

A [compact H-hull](../../../stochastic-process.md#compact-h-hull) is a bounded relatively closed set $A\subset\mathbb H$ for which $\mathbb H\setminus A$ is a [simply connected domain](../../../complex-analysis.md#simply-connected-domain). The [Riemann mapping theorem](../../../complex-analysis.md#riemann-mapping-theorem) and [hydrodynamic normalization at infinity](../../../stochastic-process.md#hydrodynamic-normalization-at-infinity) give a unique [mapping-out function of a compact H-hull](../../../stochastic-process.md#mapping-out-function-of-a-compact-h-hull) $g_A:\mathbb H\setminus A\to\mathbb H$ with

$$
g_A(z)=z+\frac{a}{z}+O(|z|^{-2}).
$$

The coefficient $a\geq0$ is the [half-plane capacity](../../../stochastic-process.md#half-plane-capacity) $\operatorname{hcap}(A)$.

For $\lambda>0$ and $x\in\mathbb R$, uniqueness of the normalized map gives

$$
g_{\lambda A+x}(z)=x+\lambda g_A\!\left(\frac{z-x}{\lambda}\right).
$$

Substituting the expansion of $g_A$ yields

$$
g_{\lambda A+x}(z)=z+\frac{\lambda^2a}{z-x}+O(|z|^{-2})=z+\frac{\lambda^2a}{z}+O(|z|^{-2}).
$$

Therefore the [scaling and translation of half-plane capacity](../../../stochastic-process.md#scaling-and-translation-of-half-plane-capacity) is

$$
\boxed{\operatorname{hcap}(\lambda A+x)=\lambda^2\operatorname{hcap}(A).}
$$

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/i">i</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/i/solution">Solution</h5>

↑ **Parent:** [I](#1/b/i)

Let $d=\operatorname{diam}(A)$. Unless $A$ is empty, its closure meets the real axis; otherwise a loop in $\mathbb H\setminus A$ surrounding $A$ could not contract, contrary to $\mathbb H\setminus A$ being a [simply connected domain](../../../complex-analysis.md#simply-connected-domain). Choose $x\in\overline A\cap\mathbb R$. Then $A\subseteq\{z\in\mathbb H:|z-x|\leq d\}$.

The unit half-disc is a compact H-hull with mapping-out function $z+z^{-1}$, so its [half-plane capacity](../../../stochastic-process.md#half-plane-capacity) is one. The [monotonicity of half-plane capacity](../../../stochastic-process.md#monotonicity-of-half-plane-capacity) and its scaling rule now give

$$
\operatorname{hcap}(A)\leq\operatorname{hcap}\{z\in\mathbb H:|z-x|\leq d\}=d^2.
$$

**Thus the assertion holds with the universal constant $c=1$ under this normalization.**

<h4 id="1/b/ii">ii</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/b/ii)

For $r\geq1$, let $R_r=[-r,r]\times(0,1]$. The [Brownian representation of half-plane capacity](../../../stochastic-process.md#brownian-representation-of-half-plane-capacity) gives

$$
\operatorname{hcap}(R_r)=\lim_{y\to\infty}y\,\mathbb E_{iy}[\operatorname{Im}B_\tau].
$$

On hitting $R_r$ the imaginary part is at most one, while the [harmonic measure](../../../brownian-motion.md#harmonic-measure) estimate supplied in the question shows that the probability of reaching a disc of radius $O(r)$ containing $R_r$ is $O(r/y)$. Hence $\operatorname{hcap}(R_r)\leq Cr$, the [half-plane capacity of a low rectangle](../../../stochastic-process.md#half-plane-capacity-of-a-low-rectangle) bound.

Set

$$
A_n=n^{-1}R_n=[-1,1]\times(0,n^{-1}].
$$

The [scaling and translation of half-plane capacity](../../../stochastic-process.md#scaling-and-translation-of-half-plane-capacity) gives

$$
\operatorname{hcap}(A_n)=n^{-2}\operatorname{hcap}(R_n)\leq Cn^{-1}\longrightarrow0,
$$

whereas $\operatorname{diam}(A_n)=\sqrt{4+n^{-2}}\to2$. This supplies the required sequence.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Let $S_r=\{se^{i\theta}:0<s\leq r\}$. Since $S_r=rS_1$, the [scaling and translation of half-plane capacity](../../../stochastic-process.md#scaling-and-translation-of-half-plane-capacity) gives

$$
\operatorname{hcap}(S_r)=r^2\operatorname{hcap}(S_1)=ar^2.
$$

The [half-plane-capacity parameterization](../../../stochastic-process.md#half-plane-capacity-parameterization) requires $ar(t)^2=2t$, so

$$
r(t)=\sqrt{\frac{2t}{a}},
\qquad
\gamma(t)=\sqrt{\frac{2t}{a}}e^{i\theta}.
$$

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

The parameterization in part (c) gives the exact self-similarity

$$
K_{\lambda^2t}=\lambda K_t
$$

for every $\lambda>0$. The [Loewner local growth property](../../../stochastic-process.md#loewner-local-growth-property) supplies a continuous [Loewner driving function](../../../stochastic-process.md#loewner-driving-function) $U$. Under this scaling of the hulls, the deterministic scaling rule for the [Chordal Loewner equation](../../../stochastic-process.md#chordal-loewner-equation) gives

$$
U_{\lambda^2t}=\lambda U_t.
$$

Taking $t=1$ and $\lambda=\sqrt t$ shows that

$$
U_t=U_1\sqrt t=c\sqrt t
$$

for the real constant $c=U_1$.

## 2

↑ **Parent:** [Paper 203](paper-203.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

For [Schramm–Loewner evolution](../../../stochastic-process.md#schramm-loewner-evolution) in $(\mathbb H,0,\infty)$, the [Scaling invariance of SLE](../../../stochastic-process.md#scaling-invariance-of-sle) states that, for every $a>0$,

$$
\widetilde K_t=a^{-1}K_{a^2t}
$$

has the same law as $K_t$. The scaled [Loewner driving function](../../../stochastic-process.md#loewner-driving-function) is $\widetilde U_t=a^{-1}U_{a^2t}$. Since $U_t=\sqrt\kappa B_t$, the [Brownian scaling](../../../brownian-motion.md#brownian-scaling) identity $a^{-1}B_{a^2t}\overset d=B_t$ proves the claim.

The [Conformal Markov property of SLE](../../../stochastic-process.md#conformal-markov-property-of-sle) states that, conditionally on the hull through time $t$, the future hull mapped by $g_t-U_t$ is an independent $\operatorname{SLE}_\kappa$ in $(\mathbb H,0,\infty)$. More precisely,

$$
\widetilde K_s=(g_t(K_{t+s}\setminus K_t)-U_t)^{\mathrm{fill}}
$$

has driving function $\widetilde U_s=U_{t+s}-U_t$. The [stationary increments](../../../stochastic-process.md#stationary-increments) and [independent increments](../../../stochastic-process.md#independent-increments) of [Brownian motion](../../../brownian-motion.md) show that $\widetilde U$ is independent of $\mathcal F_t$ and has the same law as $\sqrt\kappa B$. The deterministic correspondence between continuous drivers and [Loewner chains](../../../stochastic-process.md#loewner-chain) completes the proof.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Put $w=g_T^{-1}(U_T+z)$ and define

$$
f_s(z)=g_{T-s}(w)-U_T.
$$

Then $f_0(z)=z$. Differentiating with the [Chordal Loewner equation](../../../stochastic-process.md#chordal-loewner-equation) gives

$$
\partial_sf_s(z)=-\frac2{g_{T-s}(w)-U_{T-s}}=-\frac2{f_s(z)-(U_{T-s}-U_T)}.
$$

Uniqueness for this [ordinary differential equation](../../../differential-equation.md#ordinary-differential-equation) shows that $f_s=h_s$. At $s=T$,

$$
h_T(z)=w-U_T=g_T^{-1}(U_T+z)-U_T,
$$

which is the endpoint identity for the [Reverse Loewner flow](../../../stochastic-process.md#reverse-loewner-flow).

For $0<s<T$, the pathwise identity $h_s(z)=g_s^{-1}(U_s+z)-U_s$ is generally false. The left side is built from the reversed final driver segment $(U_{T-r}-U_T)_{0\leq r\leq s}$, whereas the right side is built from the initial segment $(U_r)_{0\leq r\leq s}$. By time reversal and symmetry of [Brownian motion](../../../brownian-motion.md) they have the same [probability distribution](../../../probability-theory.md#probability-distribution), but they are not equal for the given Brownian path.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

For $z=x+iy$ with $|x|\leq1$ and $0<y\leq1$, the given [Reverse SLE derivative martingale](../../../stochastic-process.md#reverse-sle-derivative-martingale) starts from

$$
M_0=\left(1+\frac{x^2}{y^2}\right)^{4/\kappa}\leq C_0y^{-8/\kappa}.
$$

It is a nonnegative local martingale and therefore a [supermartingale](../../../martingale.md#supermartingale). Since its second factor is at least one,

$$
\mathbb E|h_T'(x+iy)|^2\leq\mathbb E M_T\leq C_0y^{-8/\kappa}.
$$

Choose

$$
0<\alpha<\frac12\left(1-\frac8\kappa\right),
$$

which is possible exactly because $\kappa>8$. At height $y_n=2^{-n}$, take a horizontal grid of spacing comparable to $y_n$ in $[-1,1]$. The [Markov inequality](../../../probability-inequality.md#markov-inequality) gives, at each grid point,

$$
\mathbb P\bigl(|h_T'(z)|>y_n^{-1+\alpha}\bigr)\leq C y_n^{2-2\alpha-8/\kappa}.
$$

There are $O(y_n^{-1})$ grid points, so the probability that the bound fails anywhere on level $n$ is at most $Cy_n^{1-2\alpha-8/\kappa}$. These probabilities are summable. The [Borel-Cantelli lemmas](../../../probability-theory.md#borel-cantelli-lemmas) therefore give an almost surely finite random constant controlling every sufficiently fine grid, and enlarging it handles the finitely many remaining levels.

Every point of the half-rectangle lies within a fixed hyperbolic distance of one of these grid points at comparable height. The [Koebe distortion theorem](../../../complex-analysis.md#koebe-distortion-theorem) compares the two derivatives by a universal factor. Hence an almost surely finite random $C$ satisfies

$$
|h_T'(x+iy)|\leq Cy^{-1+\alpha}
$$

for all $x\in[-1,1]$ and $0<y\leq1$. This proves the [Reverse SLE derivative bound above the space-filling threshold](../../../stochastic-process.md#reverse-sle-derivative-bound-above-the-space-filling-threshold).

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

Apply the [derivative criterion for Hölder continuity up to a boundary](../../../sobolev-space.md#derivative-criterion-for-holder-continuity-up-to-a-boundary) to the estimate from part (c). For two points at distance $r$, move each vertically to height at least $r$, join them horizontally there, and move back. The two vertical integrals are bounded by

$$
C\int_0^ry^{-1+\alpha}dy=\frac C\alpha r^\alpha,
$$

and the horizontal integral is at most $Cr\,r^{-1+\alpha}=Cr^\alpha$. Thus $h_T$ extends continuously to the bottom edge and satisfies

$$
|h_T(z)-h_T(w)|\leq C'|z-w|^\alpha
$$

on the half-rectangle. In particular, it is almost surely a [Hölder continuous function](../../../sobolev-space.md#holder-condition) there.

## 3

↑ **Parent:** [Paper 203](paper-203.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Set $\kappa=4/(d-1)>4$. For chordal [Schramm–Loewner evolution](../../../stochastic-process.md#schramm-loewner-evolution), the centered image of a real boundary point, divided by $\sqrt\kappa$, follows the [Boundary-point Bessel flow for SLE](../../../stochastic-process.md#boundary-point-bessel-flow-for-sle); changing $B$ to $-B$ matches the sign convention in the question. Thus $\tau_x$ and $\tau_y$ are the times at which the marked boundary points $x$ and $y$ are swallowed, or equivalently disconnected from infinity, by the [Loewner chain](../../../stochastic-process.md#loewner-chain).

Consequently

$$
\{\tau_x>\tau_y\}=\{\text{the SLE trace reaches }(-\infty,y]\text{ before }[x,\infty)\}.
$$

It is the event that the negative marked point is swallowed before the positive marked point.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

For every $a>0$, define

$$
\widehat X_t=a^{-1}X_{a^2t},
\qquad
\widehat Y_t=a^{-1}Y_{a^2t},
\qquad
\widehat B_t=a^{-1}B_{a^2t}.
$$

The [Brownian scaling](../../../brownian-motion.md#brownian-scaling) theorem makes $\widehat B$ a standard Brownian motion, and substitution shows that $(\widehat X,\widehat Y)$ satisfies the same coupled [Bessel process](../../../brownian-motion.md#bessel-process) equations from initial values $(x/a,y/a)$. Both hitting times are divided by $a^2$, so their order is unchanged. Taking $a=x$ or comparing any two pairs with the same ratio proves that $\mathbb P(\tau_x>\tau_y)$ depends only on $x/y$.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

The [Strong Markov property](../../../markov-process.md#strong-markov-property) and part (b) show that, before $\tau=\tau_x\wedge\tau_y$,

$$
F(V_t)=\mathbb P(\tau_x>\tau_y\mid\mathcal F_t).
$$

Thus $F(V_{t\wedge\tau})$ is a bounded [martingale](../../../martingale.md). From the given stochastic differential equation,

$$
d[V]_t=\frac{(1-V_t)^2}{Y_t^2}dt.
$$

The [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) says that the drift of $F(V_t)$ is

$$
\frac1{2Y_t^2}\left[(1-v)^2F''(v)+\left(\frac{d-1}{v}+(3-d)v-2\right)F'(v)\right]_{v=V_t}dt.
$$

It must vanish. Dividing by $(1-v)^2/2$ and using the algebraic identity supplied in the question gives

$$
\boxed{F''(v)+\left(\frac{d-1}{v}+\frac{2d-4}{1-v}\right)F'(v)=0,
\qquad v<0.}
$$

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

Because $\widetilde F$ solves the differential equation from part (c), the [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) makes $\widetilde F(V_t)$ a [local martingale](../../../martingale.md#local-martingale) before $\tau$. The defining [improper integral](../../../real-analysis.md#improper-integral) converges at both endpoints: its integrand is asymptotic to $(-u)^{1-d}$ near zero and to $|u|^{d-3}$ at minus infinity. Since $1<d<2$, both exponents are integrable. Hence

$$
0\leq\widetilde F(v)\leq I:=\int_{-\infty}^0\frac{du}{(-u)^{d-1}(1-u)^{4-2d}}<\infty,
$$

so the stopped local martingale is a bounded martingale.

If $\tau_x<\tau_y$, then $V_t\to0$ and $\widetilde F(V_t)\to0$. If $\tau_y<\tau_x$, then $V_t\to-\infty$ and $\widetilde F(V_t)\to I$. The hitting times cannot coincide because $X_t-Y_t$ stays positive. The [optional sampling theorem for a supermartingale](../../../martingale.md#optional-sampling-theorem-for-a-supermartingale) and [bounded convergence theorem](../../../measure-theory.md#bounded-convergence-theorem) therefore give

$$
\widetilde F(v)=I\,\mathbb P(\tau_y<\tau_x)=I F(v).
$$

Consequently

$$
F(v)=c\widetilde F(v),
\qquad
c=I^{-1}>0,
$$

which is the [Two-sided SLE boundary swallowing probability](../../../stochastic-process.md#two-sided-sle-boundary-swallowing-probability).

## 4

↑ **Parent:** [Paper 203](paper-203.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

The [Zero-boundary Gaussian free field](../../../stochastic-process.md#zero-boundary-gaussian-free-field) on the unit disc is the centered [Gaussian process](../../../stochastic-process.md#gaussian-process) indexed by finite [Borel measures](../../../measure-theory.md#borel-measure) of finite [Green energy](../../../stochastic-process.md#green-energy), with [covariance](../../../variance.md#covariance)

$$
\mathbb E[(h,\rho)(h,\nu)]=\iint_{\mathbb D\times\mathbb D}G_{\mathbb D}(x,y)\rho(dx)\nu(dy).
$$

This covariance determines all its [finite-dimensional distributions](../../../stochastic-process.md#finite-dimensional-distribution).

The [Domain Markov property of the Gaussian free field](../../../stochastic-process.md#domain-markov-property-of-the-gaussian-free-field) says that for every suitable open $U\subset\mathbb D$ one can write

$$
h=h_U+h^{\mathbb D\setminus U},
$$

where $h_U$ is a zero-boundary Gaussian free field on $U$, independent of $h^{\mathbb D\setminus U}$, while $h^{\mathbb D\setminus U}$ is harmonic on $U$ and carries the information from the field outside $U$.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Take $U=B(0,e^{-t})$ in the [Domain Markov property of the Gaussian free field](../../../stochastic-process.md#domain-markov-property-of-the-gaussian-free-field). The field $h^{\mathbb D\setminus U}$ is a [harmonic function](../../../partial-differential-equation.md#harmonic-function) throughout $U$. If $s>t$, the circle $\partial B(0,e^{-s})$ lies inside $U$, so the [mean value property for harmonic functions](../../../partial-differential-equation.md#mean-value-property-for-harmonic-functions) gives

$$
\boxed{(h^{\mathbb D\setminus U},\rho_s)=h^{\mathbb D\setminus U}(0).}
$$

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

Write $h=h_U+h^{\mathbb D\setminus U}$ with $U=B(0,e^{-t})$. By part (b), the harmonic part contributes the same value $h^{\mathbb D\setminus U}(0)$ to every inner circle average. At radius $e^{-t}$ the zero-boundary part contributes zero; equivalently, take the limit from inner circles and use the assumed continuity. Hence

$$
X_s-X_t=(h_U,\rho_s).
$$

The field $h_U$ is independent of $h^{\mathbb D\setminus U}$, so the increment has the required independence.

The dilation $z\mapsto e^tz$ maps $U$ onto the unit disc and maps the circle of radius $e^{-s}$ onto the circle of radius $e^{-(s-t)}$. The [Conformal invariance of the two-dimensional Gaussian free field](../../../stochastic-process.md#conformal-invariance-of-the-two-dimensional-gaussian-free-field) therefore gives

$$
\boxed{X_s-X_t\overset d=X_{s-t}.}
$$

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

Part (c), iterated over disjoint nested annuli, gives [independent increments](../../../stochastic-process.md#independent-increments), and the law $X_s-X_t\overset d=X_{s-t}$ gives [stationary increments](../../../stochastic-process.md#stationary-increments). Every finite vector is jointly Gaussian by the definition of the [Zero-boundary Gaussian free field](../../../stochastic-process.md#zero-boundary-gaussian-free-field), and a continuous version was assumed. Moreover $X_0=0$, because the field has zero boundary values.

Thus $X$ is a continuous centered [Gaussian process](../../../stochastic-process.md#gaussian-process) with [stationary increments](../../../stochastic-process.md#stationary-increments) and [independent increments](../../../stochastic-process.md#independent-increments). Its [variance](../../../variance.md) is a [continuous additive function on the nonnegative real numbers](../../../analysis.md#continuous-additive-function-on-the-nonnegative-real-numbers), so $\operatorname{Var}(X_t)=\sigma^2t$ for some $\sigma^2\geq0$. The [Gaussian-process characterization of Brownian motion](../../../brownian-motion.md#gaussian-process-characterization-of-brownian-motion) now gives

$$
(X_t)_{t\geq0}\overset d=(\sigma B_t)_{t\geq0}
$$

for standard [Brownian motion](../../../brownian-motion.md) $B$. This is the [Circle-average process of the Gaussian free field is Brownian motion](../../../stochastic-process.md#circle-average-process-of-the-gaussian-free-field-is-brownian-motion).

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2024](../../2024.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
