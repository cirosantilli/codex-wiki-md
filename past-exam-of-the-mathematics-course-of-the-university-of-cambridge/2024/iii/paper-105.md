# Paper 105

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2024/Paper_105.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2024/Paper_105.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [i](#1/a/i)
      - [Solution](#1/a/i/solution)
    - [ii](#1/a/ii)
      - [Solution](#1/a/ii/solution)
    - [iii](#1/a/iii)
      - [Solution](#1/a/iii/solution)
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
  - [d](#1/d)
    - [i](#1/d/i)
      - [Solution](#1/d/i/solution)
    - [ii](#1/d/ii)
      - [Solution](#1/d/ii/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [i](#2/c/i)
      - [Solution](#2/c/i/solution)
    - [ii](#2/c/ii)
      - [Solution](#2/c/ii/solution)
    - [iii](#2/c/iii)
      - [Solution](#2/c/iii/solution)
    - [iv](#2/c/iv)
      - [Solution](#2/c/iv/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
  - [d](#3/d)
    - [Solution](#3/d/solution)

## 1

↑ **Parent:** [Paper 105](paper-105.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/i">i</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/i/solution">Solution</h5>

↑ **Parent:** [I](#1/a/i)

The [principal symbol](../../../partial-differential-equation.md#principal-symbol-of-a-partial-differential-equation) of the equation is

$$
P(t,x;\tau,\xi)=tx\tau^2-\xi^2.
$$

In the standard notation $Au_{tt}+2Bu_{tx}+Cu_{xx}$, we have $A=tx$, $B=0$, and $C=-1$, so

$$
B^2-AC=tx.
$$

A second-order equation is a [hyperbolic partial differential equation](../../../partial-differential-equation.md#hyperbolic-partial-differential-equation) exactly where this discriminant is positive. Hence the hyperbolic set is

$$
\boxed{\{(t,x):tx>0\}},
$$

the union of the first and third open quadrants.

<h4 id="1/a/ii">ii</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/a/ii)

A [characteristic hypersurface](../../../partial-differential-equation.md#characteristic-hypersurface) of the form $\phi(t,x)=p(t)\pm q(x)$ must satisfy

$$
tx\,p'(t)^2-q'(x)^2=0.
$$

On either connected component of $tx>0$, separation gives

$$
tp'(t)^2=\frac{q'(x)^2}{x}=\operatorname{sgn}(t)=\operatorname{sgn}(x).
$$

One choice valid on both components is

$$
p(t)=2\operatorname{sgn}(t)\sqrt{|t|},
\qquad
q(x)=\frac23\operatorname{sgn}(x)|x|^{3/2}.
$$

Indeed, $p'(t)=|t|^{-1/2}$ and $q'(x)=|x|^{1/2}$ away from the axes, so $txp'^2=q'^2$. Thus

$$
\boxed{p(t)+q(x)=\text{constant},\qquad p(t)-q(x)=\text{constant}}
$$

are the two families of characteristics, and $p\pm q$ are [characteristic coordinates](../../../partial-differential-equation.md#characteristic-coordinate).

<h4 id="1/a/iii">iii</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#1/a/iii)

The initial line is $t=t_0$, whose conormal is $dt$. Evaluating the [principal symbol](../../../partial-differential-equation.md#principal-symbol-of-a-partial-differential-equation) on it gives

$$
P(t_0,x_0;1,0)=t_0x_0.
$$

It is therefore a [non-characteristic hypersurface](../../../partial-differential-equation.md#non-characteristic-hypersurface) at $(t_0,x_0)$ exactly when $t_0x_0\ne0$. At such a point the equation can be written

$$
u_{tt}=\frac{u_{xx}-u_t^2}{tx},
$$

whose right-hand side is [real analytic](../../../analysis.md#real-analytic-function) locally, and the prescribed [Cauchy data](../../../partial-differential-equation.md#cauchy-data) are also real analytic. The [Cauchy-Kovalevskaya theorem](../../../partial-differential-equation.md#cauchy-kovalevskaya-theorem) consequently gives a unique local analytic solution exactly at the points

$$
\boxed{t_0x_0\ne0}.
$$

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/i">i</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/i/solution">Solution</h5>

↑ **Parent:** [I](#1/b/i)

For $u\in L^1_{\mathrm{loc}}(\mathbb R)$, a function $g\in L^1_{\mathrm{loc}}(\mathbb R)$ is its [weak derivative](../../../distribution-theory.md#weak-derivative) when

$$
\int_{\mathbb R}u(x)\varphi'(x)\,dx
=-\int_{\mathbb R}g(x)\varphi(x)\,dx
$$

for every [test function](../../../distribution-theory.md#test-function) $\varphi\in C_c^\infty(\mathbb R)$. Equivalently, the [distributional derivative](../../../distribution-theory.md#distributional-derivative) of $u$ is represented by the locally integrable function $g$.

<h4 id="1/b/ii">ii</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/b/ii)

For $u(x)=\sin|x|$, the ordinary derivative away from zero is

$$
g(x)=
\begin{cases}
-\cos x,&-\pi<x<0,\\
\cos x,&0<x<\pi.
\end{cases}
$$

This bounded function is locally integrable. For a [test function](../../../distribution-theory.md#test-function) $\varphi$, [integration by parts](../../../calculus.md#integration-by-parts) on $(-\pi,0)$ and $(0,\pi)$ produces boundary terms at zero which cancel because $u$ is continuous there and $u(0)=0$. Hence

$$
\int_{-\pi}^{\pi}u\varphi'=-\int_{-\pi}^{\pi}g\varphi.
$$

Therefore $u$ has the [weak derivative](../../../distribution-theory.md#weak-derivative)

$$
\boxed{u'(x)=\operatorname{sgn}(x)\cos|x|\quad\text{for almost every }x.}
$$

The jump in the ordinary derivative creates no [Dirac delta function](../../../distribution-theory.md#dirac-delta-function); such a term would arise from a jump in the function itself.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/i">i</h4>

↑ **Parent:** [C](#1/c)

<h5 id="1/c/i/solution">Solution</h5>

↑ **Parent:** [I](#1/c/i)

For $1\leq p<n$, define the [Sobolev conjugate exponent](../../../sobolev-space.md#sobolev-conjugate-exponent)

$$
p^*=\frac{np}{n-p},
\qquad
\frac1{p^*}=\frac1p-\frac1n.
$$

The [Sobolev inequality](../../../sobolev-space.md#sobolev-inequality), also called the Gagliardo--Nirenberg--Sobolev inequality, states that there is a constant $C=C(n,p)$ such that

$$
\boxed{\|u\|_{L^{p^*}(\mathbb R^n)}\leq C\|Du\|_{L^p(\mathbb R^n)}}
$$

for every $u\in C_c^\infty(\mathbb R^n)$, and hence by completion for every $u\in W^{1,p}(\mathbb R^n)$ for which the right formulation applies.

<h4 id="1/c/ii">ii</h4>

↑ **Parent:** [C](#1/c)

<h5 id="1/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/c/ii)

Take $u\in W_0^{1,p}(U)$ and extend it by zero outside $U$. The [zero extension of W01](../../../sobolev-space.md#zero-extension-of-w01) belongs to $W^{1,p}(\mathbb R^n)$ and the [Sobolev inequality](../../../sobolev-space.md#sobolev-inequality) gives

$$
\|u\|_{L^{p^*}(U)}\leq C_S\|Du\|_{L^p(U)}.
$$

Because $U$ has finite measure, the [Holder inequality](../../../functional-analysis.md#holder-inequality) gives

$$
\|u\|_{L^p(U)}
\leq |U|^{1/p-1/p^*}\|u\|_{L^{p^*}(U)}
\leq C\|Du\|_{L^p(U)}.
$$

Thus

$$
\|u\|_{W^{1,p}(U)}
\leq C'\|Du\|_{L^p(U)}.
$$

The reverse estimate follows directly from $\|Du\|_{L^p}\leq\|u\|_{W^{1,p}}$. After adjusting constants,

$$
\boxed{C\|Du\|_{L^p(U)}\leq\|u\|_{W^{1,p}(U)}\leq C'\|Du\|_{L^p(U)}}.
$$

This is the [Poincaré inequality](../../../sobolev-space.md#poincare-inequality) on $W_0^{1,p}(U)$.

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/i">i</h4>

↑ **Parent:** [D](#1/d)

<h5 id="1/d/i/solution">Solution</h5>

↑ **Parent:** [I](#1/d/i)

The [Fredholm alternative for an elliptic Dirichlet problem](../../../elliptic-boundary-value-problem.md#fredholm-alternative-for-an-elliptic-dirichlet-problem) says that either the homogeneous adjoint problem has only the zero solution, in which case $Lu=f$ has a unique solution for every admissible $f$, or the homogeneous kernels are nontrivial and finite-dimensional. In the latter case,

$$
Lu=f
$$

is solvable exactly when

$$
\langle f,v\rangle=0
\qquad\text{for every }v\in\ker L^*,
$$

and any two solutions differ by an element of $\ker L$. Moreover $\dim\ker L=\dim\ker L^*$.

<h4 id="1/d/ii">ii</h4>

↑ **Parent:** [D](#1/d)

<h5 id="1/d/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/d/ii)

For $L=d^2/dx^2+1$ with homogeneous [Dirichlet data](../../../differential-equation.md#dirichlet-boundary-condition) at $0$ and $2\pi$, [integration by parts](../../../calculus.md#integration-by-parts) shows that $L^*=L$. Its homogeneous kernel is

$$
\ker L=\operatorname{span}\{\sin x\},
$$

because $A\cos x+B\sin x$ vanishes at both endpoints exactly when $A=0$.

The forcing obeys the [orthogonality](../../../linear-algebra.md#orthogonal-vectors) condition

$$
\int_0^{2\pi}\cos x\sin x\,dx=0.
$$

The [Fredholm alternative for an elliptic Dirichlet problem](../../../elliptic-boundary-value-problem.md#fredholm-alternative-for-an-elliptic-dirichlet-problem) therefore says that solutions exist, though they are not unique. Indeed,

$$
\boxed{u(x)=\frac{x}{2}\sin x+C\sin x}
$$

satisfies $u''+u=\cos x$ and both boundary conditions for every constant $C$.

## 2

↑ **Parent:** [Paper 105](paper-105.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Set

$$
\phi(x)=\int_0^xu(t)\,dt,
\qquad
Au(x)=\frac{\phi(x)}x.
$$

The [Holder inequality](../../../functional-analysis.md#holder-inequality) gives

$$
|\phi(x)|^p x^{1-p}
\leq\int_0^x|u(t)|^p\,dt\longrightarrow0
\quad(x\downarrow0).
$$

Using $x^{-p}\,dx=-(p-1)^{-1}d(x^{1-p})$ and [integration by parts](../../../calculus.md#integration-by-parts), while discarding the nonpositive boundary term at $x=1$, yields

$$
\begin{aligned}
\|Au\|_p^p
&=\int_0^1|\phi|^px^{-p}\,dx\\
&\leq\frac p{p-1}\int_0^1|\phi|^{p-1}x^{1-p}|u|\,dx\\
&=\frac p{p-1}\int_0^1|Au|^{p-1}|u|\,dx.
\end{aligned}
$$

Another application of [Hölder's inequality](../../../functional-analysis.md#holder-inequality) gives

$$
\|Au\|_p^p
\leq\frac p{p-1}\|Au\|_p^{p-1}\|u\|_p.
$$

After cancellation, with the zero case immediate,

$$
\boxed{\|Au\|_{L^p(0,1)}\leq\frac p{p-1}\|u\|_{L^p(0,1)}}.
$$

This is the [Hardy averaging inequality](../../../sobolev-space.md#hardy-averaging-inequality).

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

The [one-dimensional Sobolev representative](../../../sobolev-space.md#one-dimensional-sobolev-representative) of $u$ is absolutely continuous, and its zero [trace](../../../sobolev-space.md#sobolev-trace-theorem) gives

$$
u(x)=\int_0^xu'(t)\,dt.
$$

Consequently $u(x)/x=A(u')(x)$ for the [Hardy operator](../../../sobolev-space.md#hardy-operator). Applying the [Hardy averaging inequality](../../../sobolev-space.md#hardy-averaging-inequality) to $u'$ gives the [Hardy inequality on an interval](../../../sobolev-space.md#hardy-inequality-on-an-interval):

$$
\boxed{\left\|\frac ux\right\|_{L^p(0,1)}
\leq\frac p{p-1}\|u'\|_{L^p(0,1)}}.
$$

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/i">i</h4>

↑ **Parent:** [C](#2/c)

<h5 id="2/c/i/solution">Solution</h5>

↑ **Parent:** [I](#2/c/i)

The [Sobolev trace theorem](../../../sobolev-space.md#sobolev-trace-theorem) makes evaluation at zero a continuous linear map $T_0:H^1(0,1)\to\mathbb R$. Hence

$$
H=\ker T_0
$$

is a [closed vector subspace](../../../vector-space.md#closed-vector-subspace) of the [Hilbert space](../../../hilbert-space.md) $H^1(0,1)$. Every closed vector subspace of a Hilbert space is complete with the restricted inner product, so $H$ is a Hilbert space with the standard $H^1$ inner product.

<h4 id="2/c/ii">ii</h4>

↑ **Parent:** [C](#2/c)

<h5 id="2/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/c/ii)

For $u\in H$, the trace $u(0)$ vanishes. Apply the [Hardy inequality on an interval](../../../sobolev-space.md#hardy-inequality-on-an-interval) with $p=2$ to obtain

$$
\boxed{\left\|\frac ux\right\|_{L^2(0,1)}\leq2\|u'\|_{L^2(0,1)}}.
$$

**Thus $u/x\in L^2(0,1)$.**

<h4 id="2/c/iii">iii</h4>

↑ **Parent:** [C](#2/c)

<h5 id="2/c/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#2/c/iii)

Multiply the differential equation by $v\in H$ and integrate. The [Hardy inequality on an interval](../../../sobolev-space.md#hardy-inequality-on-an-interval) makes the terms containing $u/x$ and $v/x$ integrable. For smooth $v$, [integration by parts](../../../calculus.md#integration-by-parts) gives

$$
-\int_0^1u''v
=\int_0^1u'v'-[u'v]_0^1
=\int_0^1u'v',
$$

because $v(0)=0$ and the [Neumann boundary condition](../../../differential-equation.md#neumann-boundary-condition) is $u'(1)=0$. Therefore

$$
\boxed{
\int_0^1u'v'
+\int_0^1\frac{uv}{x^2}
-\int_0^1u'v
=\int_0^1\frac{fv}{x^2}.}
$$

The [density of smooth functions in a Sobolev space](../../../sobolev-space.md#density-of-smooth-functions-in-a-sobolev-space) and continuity of all four terms extend this [weak formulation](../../../partial-differential-equation.md#weak-formulation) to every $v\in H$.

<h4 id="2/c/iv">iv</h4>

↑ **Parent:** [C](#2/c)

<h5 id="2/c/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#2/c/iv)

Define on $H$ the [bilinear form](../../../linear-algebra.md#bilinear-form)

$$
a(u,v)=\int_0^1u'v'+\int_0^1\frac{uv}{x^2}-\int_0^1u'v
$$

and the linear functional

$$
\ell(v)=\int_0^1\frac fx\frac vx.
$$

The [Hardy inequality on an interval](../../../sobolev-space.md#hardy-inequality-on-an-interval), [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality), and the one-sided [Poincaré inequality](../../../sobolev-space.md#poincare-inequality) show that $a$ is a [bounded bilinear form](../../../linear-algebra.md#bounded-bilinear-form) and that

$$
|\ell(v)|\leq2\|f/x\|_2\|v'\|_2\leq C\|f/x\|_2\|v\|_{H^1}.
$$

For $v\in H$, $v(x)=\int_0^xv'(t)\,dt$, so [Cauchy--Schwarz](../../../probability-and-statistics.md#cauchy-schwarz-inequality) and [Fubini's theorem](../../../measure-theory.md#fubini-s-theorem) give

$$
\|v\|_2^2\leq\frac12\|v'\|_2^2.
$$

Hence

$$
\begin{aligned}
a(v,v)
&=\|v'\|_2^2+\|v/x\|_2^2-\int_0^1v'v\\
&\geq\left(1-\frac1{\sqrt2}\right)\|v'\|_2^2\\
&\geq c\|v\|_{H^1}^2.
\end{aligned}
$$

Thus $a$ is a [coercive bilinear form](../../../linear-algebra.md#coercive-bilinear-form). The [Lax-Milgram theorem](../../../functional-analysis.md#lax-milgram-theorem) supplies a unique $u\in H$ satisfying $a(u,v)=\ell(v)$ for every $v\in H$. This is precisely the unique weak solution described by the [weak boundary value problem with an inverse-square potential](../../../functional-analysis.md#weak-boundary-value-problem-with-an-inverse-square-potential).

## 3

↑ **Parent:** [Paper 105](paper-105.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

The condition $\sum_{i=1}^n1/p_i=1$ and positivity imply $p_i\geq1$. We prove the [Generalized Holder inequality](../../../functional-analysis.md#generalized-holder-inequality) by induction on $n$. The case $n=2$ is the usual [Holder inequality](../../../functional-analysis.md#holder-inequality). For the induction step, set

$$
\frac1q=\sum_{i=1}^{n-1}\frac1{p_i}=1-\frac1{p_n}.
$$

The exponents $q$ and $p_n$ are conjugate, so Hölder followed by the induction hypothesis gives

$$
\begin{aligned}
\left\|\prod_{i=1}^nf_i\right\|_1
&\leq\left\|\prod_{i=1}^{n-1}f_i\right\|_q\|f_n\|_{p_n}\\
&\leq\prod_{i=1}^n\|f_i\|_{p_i}.
\end{aligned}
$$

This proves the claim.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Since $U\subset\mathbb R^3$ is bounded and smooth, the [Sobolev embedding theorem](../../../sobolev-space.md#sobolev-embedding-theorem) gives continuous embeddings $H^1(U)\hookrightarrow L^4(U)$ and $H^1(U)\hookrightarrow L^6(U)$. Because $|\sin s|\leq1$,

$$
\|w(t)^2\sin w(t)\|_{L^2(U)}
\leq\|w(t)\|_{L^4(U)}^2
\leq C\|w(t)\|_{H^1(U)}^2.
$$

Taking the $L^2$ norm in time gives

$$
\boxed{\|w^2\sin w\|_{L^2(U_T)}
\leq\beta T^{1/2}\|w\|_{L_t^\infty H_x^1}^2}.
$$

For $F(s)=s^2\sin s$, the [mean value theorem](../../../calculus.md#mean-value-theorem) and $|F'(s)|\leq2|s|+s^2$ imply

$$
|F(r)-F(s)|
\leq C|r-s|\bigl(|r|+|s|+|r|^2+|s|^2\bigr).
$$

Apply the [Generalized Holder inequality](../../../functional-analysis.md#generalized-holder-inequality) in space, using $L^4$ for the quadratic products and $L^6\cdot L^3$ for the cubic products, and then use the two Sobolev embeddings. Pointwise in time this yields

$$
\|F(w)-F(\widetilde w)\|_2
\leq C\|w-\widetilde w\|_{H^1}
\left(\|w\|_{H^1}+\|w\|_{H^1}^2
+\|\widetilde w\|_{H^1}+\|\widetilde w\|_{H^1}^2\right).
$$

Taking the $L^2$ norm in time proves the required estimate with the factor $\gamma T^{1/2}$.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Put

$$
D=\|\psi_0\|_{H^1(U)}+\|\psi_1\|_{L^2(U)}.
$$

The assumed [energy estimate](../../../partial-differential-equation.md#energy-estimate) for the linear [wave equation](../../../wave-equation.md) and the first nonlinear estimate give, for $w\in X_{b,\tau}$,

$$
\|Aw\|_{X_\tau}
\leq C_0\left(D+\beta\tau^{1/2}b^2\right).
$$

Choose $b\geq2C_0D$ and then choose $\tau>0$ so small that $C_0\beta\tau^{1/2}b^2\leq b/2$. Then $A$ maps the closed ball $X_{b,\tau}$ into itself.

For $w,\widetilde w\in X_{b,\tau}$, the difference $Aw-A\widetilde w$ solves the linear equation with zero [Cauchy data](../../../partial-differential-equation.md#cauchy-data) and forcing $F(w)-F(\widetilde w)$. The second nonlinear estimate therefore gives

$$
\|Aw-A\widetilde w\|_{X_\tau}
\leq2C_0\gamma\tau^{1/2}(b+b^2)
\|w-\widetilde w\|_{X_\tau}.
$$

Shrinking $\tau$ once more makes the coefficient strictly smaller than one. Since $X_\tau$ is a [Banach space](../../../banach-space.md) and its closed ball is complete, $A$ is a contraction on $X_{b,\tau}$.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

By the [contraction mapping theorem](../../../analysis.md#contraction-mapping-theorem), the contraction $A:X_{b,\tau}\to X_{b,\tau}$ has a unique fixed point $u$. The identity $Au=u$ says exactly that $u$ is the weak solution of the linear initial boundary value problem whose forcing is $u^2\sin u$. Consequently $u\in X_\tau$ satisfies

$$
u_{tt}-\Delta u=u^2\sin u
$$

with the prescribed initial and homogeneous Dirichlet data. Thus a sufficiently small $\tau>0$ gives a local [weak solution](../../../partial-differential-equation.md#weak-solution) of the [semilinear wave equation](../../../wave-equation.md#semilinear-wave-equation), as summarized by the [local weak solution by contraction for a semilinear wave equation](../../../wave-equation.md#local-weak-solution-by-contraction-for-a-semilinear-wave-equation).

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2024](../../2024.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
