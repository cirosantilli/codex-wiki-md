# Paper 105

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2021/Paper_105.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2021/Paper_105.pdf)

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
- [2](#2)
  - [a](#2/a)
    - [i](#2/a/i)
      - [Solution](#2/a/i/solution)
    - [ii](#2/a/ii)
      - [Solution](#2/a/ii/solution)
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

## 1

↑ **Parent:** [Paper 105](paper-105.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Write $S=x_1+\cdots+x_n$. The [Taylor series](../../../calculus.md#taylor-series) of the [cosine](../../../geometry-and-topology.md#cosine) is

$$
\cos S=\sum_{k=0}^{\infty}\frac{(-1)^kS^{2k}}{(2k)!}.
$$

After expanding each power by the [multinomial theorem](../../../combinatorics.md#multinomial-theorem), the coefficient of $x^\alpha$ has absolute value $1/\alpha!$ when $|\alpha|$ is [even](../../../calculus.md#even-function) and is zero when $|\alpha|$ is [odd](../../../calculus.md#odd-function). The [hyperbolic cosine](../../../calculus.md#hyperbolic-cosine)

$$
g(x)=\cosh(x_1+\cdots+x_n)
=\sum_{k=0}^{\infty}\frac{(x_1+\cdots+x_n)^{2k}}{(2k)!}
$$

therefore has exactly the absolute values of the coefficients of $f$. Thus $g$ is an entire [majorant series](../../../real-analysis.md#majorant-series) for $f$.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/i">i</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/i/solution">Solution</h5>

↑ **Parent:** [I](#1/b/i)

The [principal symbol](../../../partial-differential-equation.md#principal-symbol-of-a-partial-differential-equation) of

$$
u_t-(x^2-1)u_{xx}=u_t+(1-x^2)u_{xx}=0
$$

is $p(x,t;\xi,\tau)=(1-x^2)\xi^2$. For a regular curve $s\mapsto(x(s),t(s))$, the [characteristic curve](../../../partial-differential-equation.md#characteristic-curve) equation is

$$
(1-x^2)\dot t^{,2}=0.
$$

Away from $x=\pm1$ this gives $t=\text{constant}$. The two degenerate lines $x=1$ and $x=-1$ are also characteristic. These are the characteristic curves, apart from reparametrization and pieces joined at the degenerate lines.

<h4 id="1/b/ii">ii</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/b/ii)

Along $x=\sin s$ and $t=s^2$, the characteristic expression is

$$
(1-\sin^2s)(2s)^2=4s^2\cos^2s.
$$

It vanishes exactly when

$$
\boxed{s=0\quad\hbox{or}\quad s=\frac\pi2+k\pi\quad(k\in\mathbb Z).}
$$

<h4 id="1/b/iii">iii</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#1/b/iii)

The initial line $x=0$ has conormal $dx$, and the [principal symbol](../../../partial-differential-equation.md#principal-symbol-of-a-partial-differential-equation) on this conormal is $1$. It is therefore a [non-characteristic hypersurface](../../../partial-differential-equation.md#non-characteristic-hypersurface) at every $(0,t_0)$. The equation's coefficients and the prescribed [Cauchy data](../../../partial-differential-equation.md#cauchy-data) $u(0,t)=\cos t$ and $u_x(0,t)=0$ are [real analytic functions](../../../analysis.md#real-analytic-function). The [Cauchy-Kovalevskaya theorem](../../../partial-differential-equation.md#cauchy-kovalevskaya-theorem) consequently gives a unique analytic solution in a neighbourhood of $(0,t_0)$ for every

$$
\boxed{t_0\in\mathbb R.}
$$

## 2

↑ **Parent:** [Paper 105](paper-105.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/i">i</h4>

↑ **Parent:** [A](#2/a)

<h5 id="2/a/i/solution">Solution</h5>

↑ **Parent:** [I](#2/a/i)

In [polar coordinates](../../../calculus.md#polar-coordinates), set

$$
u(x,y)=\left(\log\frac1{\sqrt{x^2+y^2}}\right)^{1/4}
$$

away from the origin, assigning any value at the origin. This is unbounded as $r=\sqrt{x^2+y^2}\downarrow0$. It belongs to $L^2(U)$ because

$$
\int_0^{1/2}r\left(\log\frac1r\right)^{1/2},dr<\infty.
$$

Moreover

$$
|\nabla u|^2=\frac1{16r^2}\left(\log\frac1r\right)^{-3/2},
$$

and hence

$$
\int_U|\nabla u|^2
=\frac{\pi}{8}\int_0^{1/2}\frac{dr}{r(\log(1/r))^{3/2}}<\infty.
$$

**Thus $u\in H^1(U)$ but $u\notin L^\infty(U)$, exhibiting the [failure of first-order Sobolev embedding into Linfinity in two dimensions](../../../sobolev-space.md#failure-of-first-order-sobolev-embedding-into-linfinity-in-two-dimensions).**

<h4 id="2/a/ii">ii</h4>

↑ **Parent:** [A](#2/a)

<h5 id="2/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/a/ii)

The boundedness in the [Sobolev space](../../../sobolev-space.md) $H^1(U)$ and the [weak sequential compactness of bounded sequences in a reflexive Banach space](../../../functional-analysis.md#weak-sequential-compactness-of-bounded-sequences-in-a-reflexive-banach-space) give a subsequence converging weakly to some $u\in H^1(U)$. For each integer $m\geq2$, the [Rellich-Kondrachov compactness theorem](../../../sobolev-space.md#rellich-kondrachov-theorem) makes $H^1(U)\hookrightarrow L^m(U)$ compact because the dimension is two. Repeated extraction followed by the [diagonal argument](../../../foundations-of-mathematics.md#diagonal-argument) gives one subsequence $u_{n_k}$ converging strongly to $u$ in every $L^m(U)$ with integral $m\geq2$.

For any finite real $p\geq1$, choose an integer $m\geq\max\{2,p\}$. Since $U$ has finite measure, the [Lp inclusion on a finite measure space](../../../measure-theory.md#lp-inclusion-on-a-finite-measure-space) gives

$$
\|u_{n_k}-u\|_{L^p(U)}
\leq |U|^{1/p-1/m}\|u_{n_k}-u\|_{L^m(U)}\longrightarrow0.
$$

The same subsequence therefore works for every finite $p$.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/i">i</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/i/solution">Solution</h5>

↑ **Parent:** [I](#2/b/i)

The [Holder inequality](../../../functional-analysis.md#holder-inequality) interpolates between $L^2(U)$ and $L^6(U)$:

$$
\|v\|_{L^3}^3
=\int_U|v|^{3/2}|v|^{3/2}
\leq\|v\|_{L^2}^{3/2}\|v\|_{L^6}^{3/2}.
$$

Taking cube roots and applying the three-dimensional [Sobolev inequality](../../../sobolev-space.md#sobolev-inequality) $H^1(U)\hookrightarrow L^6(U)$ gives

$$
\|v\|_{L^3(U)}
\leq C\|v\|_{L^2(U)}^{1/2}\|v\|_{H^1(U)}^{1/2}.
$$

This is the [H1 L3 interpolation inequality in three dimensions](../../../sobolev-space.md#h1-l3-interpolation-inequality-in-three-dimensions).

<h4 id="2/b/ii">ii</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/b/ii)

Linearity in $u$ follows from linearity of the [weak derivative](../../../distribution-theory.md#weak-derivative) and [Lebesgue integration](../../../calculus.md#lebesgue-integration). By the [Holder inequality](../../../functional-analysis.md#holder-inequality), the three-dimensional [Sobolev inequality](../../../sobolev-space.md#sobolev-inequality), and the preceding $L^3$ interpolation estimate,

$$
|\Phi(u)|
\leq\sqrt3\,\|\nabla u\|_2\|vw\|_2
\leq\sqrt3\,\|\nabla u\|_2\|v\|_6\|w\|_3
\leq C\|v\|_{H^1}\|w\|_{H^1}\|u\|_{H^1}.
$$

**Thus $\Phi$ is a [linear functional](../../../linear-algebra.md#linear-functional) and a [continuous linear map](../../../topological-vector-space.md#continuous-linear-operator) on $H^1(U)$.**

<h4 id="2/b/iii">iii</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#2/b/iii)

After passing to a subsequence, weak compactness and the [Rellich-Kondrachov compactness theorem](../../../sobolev-space.md#rellich-kondrachov-theorem) give

$$
u_{n_k}\rightharpoonup u\quad\hbox{in }H^1(U),
\qquad
u_{n_k}\longrightarrow u\quad\hbox{in }L^3(U).
$$

For fixed $w\in H^1(U)$, the [Sobolev inequality](../../../sobolev-space.md#sobolev-inequality) gives $w\in L^6(U)$, so

$$
u_{n_k}w\longrightarrow uw\quad\hbox{in }L^2(U).
$$

Meanwhile $\partial_j u_{n_k}\rightharpoonup\partial_j u$ in $L^2(U)$. Pairing this weak convergence with the strong convergence of the products, or equivalently using the [weak-strong product convergence lemma](../../../functional-analysis.md#weak-strong-product-convergence-lemma), yields

$$
\boxed{\int_U(\partial_xu_{n_k}+\partial_yu_{n_k}+\partial_zu_{n_k})u_{n_k}w
\longrightarrow
\int_U(\partial_xu+\partial_yu+\partial_zu)uw.}
$$

## 3

↑ **Parent:** [Paper 105](paper-105.md)

<h3 id="3/i">i</h3>

↑ **Parent:** [3](#3)

<h4 id="3/i/solution">Solution</h4>

↑ **Parent:** [I](#3/i)

In three dimensions the [Sobolev embedding theorem](../../../sobolev-space.md#sobolev-embedding-theorem) gives

$$
H^2(U)\hookrightarrow L^\infty(U),
\qquad
H^2(U)\hookrightarrow W^{1,4}(U).
$$

Consequently, for $w\in H^2(U)\cap H_0^1(U)$,

$$
\||Dw|^2w\|_{L^2}
\leq\|Dw\|_{L^4}^2\|w\|_{L^\infty}
\leq C\|w\|_{H^2}^3.
$$

Thus $f+|Dw|^2w\in L^2(U)$. The [Dirichlet Poisson regularity theorem](../../../distribution-theory.md#dirichlet-poisson-regularity-theorem) on a bounded $C^2$ domain says that

$$
-\Delta v=f+|Dw|^2w,qquad v|_{\partial U}=0,
$$

has a unique $v\in H^2(U)\cap H_0^1(U)$ and

$$
\|v\|_{H^2}\leq C\bigl(\|f\|_2+\||Dw|^2w\|_2\bigr).
$$

**Hence $\Phi(w)=v$ is well defined.**

<h3 id="3/ii">ii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#3/ii)

The preceding estimate gives constants $A,B>0$ such that, whenever $\|w\|_{H^2}\leq R$,

$$
\|\Phi(w)\|_{H^2}\leq A\|f\|_2+BR^3.
$$

Choose $R>0$ so that $BR^2\leq1/2$, and then choose $r>0$ so that $Ar\leq R/2$. If $\|f\|_2\leq r$, the closed ball $B_R(0)$ is mapped into itself.

For $w,z\in B_R(0)$, factor the [cubic gradient nonlinearity](../../../elliptic-boundary-value-problem.md#cubic-gradient-nonlinearity) as

$$
|Dw|^2w-|Dz|^2z
=|Dw|^2(w-z)+(Dw+Dz)\mathbin\cdot D(w-z),z.
$$

The same [Sobolev embedding theorem](../../../sobolev-space.md#sobolev-embedding-theorem) and the [Holder inequality](../../../functional-analysis.md#holder-inequality) imply

$$
\||Dw|^2w-|Dz|^2z\|_2
\leq CR^2\|w-z\|_{H^2}.
$$

The elliptic estimate therefore yields

$$
\|\Phi(w)-\Phi(z)\|_{H^2}
\leq C'R^2\|w-z\|_{H^2}.
$$

Shrinking $R$ further makes $C'R^2<1$, so $\Phi$ is a [contraction mapping](../../../analysis.md#contraction-mapping) of the closed ball. This ball is complete because $H^2(U)\cap H_0^1(U)$ is a [Banach space](../../../banach-space.md). The [contraction mapping theorem](../../../analysis.md#contraction-mapping-theorem) gives a fixed point $u=\Phi(u)$, and its defining equation is

$$
-\Delta u-|Du|^2u=f,qquad u|_{\partial U}=0.
$$

**Thus the nonlinear [elliptic boundary value problem](../../../elliptic-boundary-value-problem.md) has a solution for sufficiently small $\|f\|_2$.**

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2021](../../2021.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
