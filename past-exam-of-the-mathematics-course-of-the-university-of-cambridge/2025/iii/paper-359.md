# Paper 359

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2025/III_Paper_359.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2025/III_Paper_359.pdf)

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
    - [iii](#1/c/iii)
      - [Solution](#1/c/iii/solution)
    - [iv](#1/c/iv)
      - [Solution](#1/c/iv/solution)
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
  - [c](#2/c)
    - [i](#2/c/i)
      - [Solution](#2/c/i/solution)
    - [ii](#2/c/ii)
      - [Solution](#2/c/ii/solution)

## 1

↑ **Parent:** [Paper 359](paper-359.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/i">i</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/i/solution">Solution</h5>

↑ **Parent:** [I](#1/a/i)

Expand $P_Nw$ in the orthonormal [Stokes operator](../../../viscous-fluid-flow.md#stokes-operator) eigenbasis:

$$
P_Nw=\sum_{k=1}^Nw_k\phi_k.
$$

The $H$ and $V$ norms satisfy

$$
|P_Nw|^2=\sum_{k=1}^N|w_k|^2,
\qquad
\|P_Nw\|^2=(AP_Nw,P_Nw)
=\sum_{k=1}^N\lambda_k|w_k|^2.
$$

Since $\lambda_k\leq\lambda_N$ on the projected space,

$$
\boxed{\|P_Nw\|\leq\lambda_N^{1/2}|P_Nw|}.
$$

This is the basic inverse estimate for a [spectral projection of the Stokes operator](../../../viscous-fluid-flow.md#spectral-projection-of-the-stokes-operator).

<h4 id="1/a/ii">ii</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/a/ii)

Interpolation between $L^2$ and $L^6$, followed by the three-dimensional [Sobolev inequality](../../../sobolev-space.md#sobolev-inequality), gives

$$
\|v\|_{L^3}
\leq\|v\|_{L^2}^{1/2}\|v\|_{L^6}^{1/2}
\leq c|v|^{1/2}\|v\|^{1/2}.
$$

Apply this with $v=P_Nw$ and use part i:

$$
\|P_Nw\|_{L^3}
\leq c|P_Nw|^{1/2}
\left(\lambda_N^{1/2}|P_Nw|\right)^{1/2}
=c\lambda_N^{1/4}|P_Nw|.
$$

Orthogonal projection is contractive in $H$, so

$$
\boxed{\|P_Nw\|_{L^3}
\leq c\lambda_N^{1/4}|w|}.
$$

The Sobolev constant is dimensionless after using the periodic-domain normalization, so the estimate is scale invariant.

<h4 id="1/a/iii">iii</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#1/a/iii)

By the [Holder inequality](../../../functional-analysis.md#holder-inequality) with exponents $3,2,6$,

$$
\begin{aligned}
|\langle B(P_Nu,v),w\rangle|
&=\left|\int_\Omega
((P_Nu)\mathbin\cdot\nabla v)\mathbin\cdot w\,dx\right|\\
&\leq\|P_Nu\|_{L^3}\|\nabla v\|_{L^2}\|w\|_{L^6}.
\end{aligned}
$$

Part ii and the Sobolev embedding $H^1\hookrightarrow L^6$ yield

$$
\boxed{
|\langle B(P_Nu,v),w\rangle|
\leq c\lambda_N^{1/4}|u|\,\|v\|\,\|w\|}.
$$

Equivalently,

$$
\|B(P_Nu,v)\|_{V'}
\leq c\lambda_N^{1/4}|u|\,\|v\|.
$$

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/i">i</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/i/solution">Solution</h5>

↑ **Parent:** [I](#1/b/i)

On the finite-dimensional space $H_m$, the Galerkin equation is an autonomous system of ordinary differential equations whose right-hand side is a quadratic polynomial in the coefficients of $u_m$. It is locally Lipschitz, so the [Picard-Lindelöf theorem](../../../differential-equation.md#picard-lindelof-theorem) gives a unique maximal local solution.

Taking the $H$ inner product with $u_m$ gives

$$
\frac12\frac d{dt}|u_m|^2+\nu\|u_m\|^2
+\langle B(P_Nu_m,u_m),u_m\rangle=0.
$$

The advecting field $P_Nu_m$ is divergence free. Periodicity and the [skew-symmetry of incompressible transport](../../../viscous-fluid-flow.md#skew-symmetry-of-incompressible-transport) therefore make the nonlinear term zero. Hence

$$
|u_m(t)|\leq|P_mu_0|\leq|u_0|.
$$

A finite-dimensional solution can cease to exist only if its norm diverges. This uniform bound prevents such blow-up, so the solution extends uniquely through every interval $[0,T]$.

<h4 id="1/b/ii">ii</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/b/ii)

Integrating the exact Galerkin energy identity gives

$$
\frac12|u_m(t)|^2
+\nu\int_0^t\|u_m(\tau)\|^2\,d\tau
=\frac12|P_mu_0|^2
\leq\frac12|u_0|^2.
$$

Thus one may take

$$
\boxed{
K_0(T)=|u_0|,
\qquad
K_1(T)=\frac{|u_0|}{\sqrt{2\nu}}}
$$

for the first two requested bounds; these constants happen not to grow with $T$.

The Galerkin equation and contractivity of $P_m$ on $V'$ give

$$
\left\|\frac{du_m}{dt}\right\|_{V'}
\leq\nu\|Au_m\|_{V'}
+\|B(P_Nu_m,u_m)\|_{V'}.
$$

Since $\|Au_m\|_{V'}=\|u_m\|$, part a gives

$$
\left\|\frac{du_m}{dt}\right\|_{V'}
\leq
\left(\nu+c\lambda_N^{1/4}|u_m|\right)\|u_m\|
\leq
\left(\nu+c\lambda_N^{1/4}|u_0|\right)\|u_m\|.
$$

Consequently

$$
\boxed{
\left\|\frac{du_m}{dt}\right\|_{L^2(0,T;V')}
\leq
K_0'(T)
:=
\left(\nu+c\lambda_N^{1/4}|u_0|\right)
\frac{|u_0|}{\sqrt{2\nu}}}.
$$

All three constants are independent of $m$.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/i">i</h4>

↑ **Parent:** [C](#1/c)

<h5 id="1/c/i/solution">Solution</h5>

↑ **Parent:** [I](#1/c/i)

The estimates from part b make $(u_m)$ bounded in

$$
L^\infty(0,T;H)\cap L^2(0,T;V),
$$

and $(\partial_tu_m)$ bounded in $L^2(0,T;V')$. Since the periodic embedding $V\Subset H$ is compact, the [Aubin-Lions lemma](../../../partial-differential-equation.md#aubin-lions-lemma) supplies a subsequence such that

$$
u_m\rightharpoonup^*u
\quad\hbox{in }L^\infty(0,T;H),
$$



$$
u_m\rightharpoonup u
\quad\hbox{in }L^2(0,T;V),
\qquad
u_m\to u
\quad\hbox{in }L^2(0,T;H).
$$

The derivatives converge weakly in $L^2(0,T;V')$ to $\partial_tu$.

Because $P_NH$ is fixed and finite dimensional, strong convergence in $H$ implies

$$
P_Nu_m\to P_Nu
\quad\hbox{strongly in }L^2(0,T;V).
$$

Combining this with the uniform $L^\infty H$ and $L^2V$ bounds in the estimate from part a identifies the weak limit

$$
B(P_Nu_m,u_m)\rightharpoonup B(P_Nu,u)
\quad\hbox{in }L^2(0,T;V').
$$

Passing to the limit in the Galerkin identity gives

$$
\boxed{
\frac{du}{dt}+\nu Au+B(P_Nu,u)=0
\quad\hbox{in }L^2(0,T;V')}.
$$

The projected initial data converge to $u_0$ in $H$, so $u(0)=u_0$.

The [weak continuity from evolution-space bounds](../../../partial-differential-equation.md#weak-continuity-from-evolution-space-bounds) gives

$$
\boxed{
u\in C([0,T];H_{\rm weak})
\cap L^\infty(0,T;H)
\cap L^2(0,T;V),
\qquad
u_t\in L^2(0,T;V')}.
$$

Since $T$ was arbitrary, this is a global weak solution of the [Navier-Stokes equation with spectrally truncated advection](../../../viscous-fluid-flow.md#navier-stokes-equation-with-spectrally-truncated-advection).

<h4 id="1/c/ii">ii</h4>

↑ **Parent:** [C](#1/c)

<h5 id="1/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/c/ii)

The evolution-space regularity permits pairing the equation with $u(t)$ and gives

$$
\frac12\frac d{dt}|u|^2
+\nu\|u\|^2
+\langle B(P_Nu,u),u\rangle=0
$$

for almost every $t$. Since $P_Nu$ is divergence free, periodic integration by parts gives

$$
\langle B(P_Nu,u),u\rangle=0.
$$

Integration in time, using $u(0)=u_0$, yields the exact energy balance

$$
\boxed{
\frac12|u(t)|^2
+\nu\int_0^t\|u(\tau)\|^2\,d\tau
=\frac12|u_0|^2}
$$

for every $t\in[0,T]$. Unlike the usual three-dimensional Leray construction, the improved $L^2(0,T;V')$ control of the truncated nonlinearity permits an equality rather than only an inequality.

<h4 id="1/c/iii">iii</h4>

↑ **Parent:** [C](#1/c)

<h5 id="1/c/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#1/c/iii)

The energy equality shows that

$$
t\longmapsto |u(t)|^2
=|u_0|^2-2\nu\int_0^t\|u(\tau)\|^2\,d\tau
$$

is continuous. Part i gives weak continuity in $H$. In a Hilbert space, weak convergence together with convergence of norms implies strong convergence. Applying this whenever $t_n\to t$ proves the [strong continuity from weak continuity and an energy equality](../../../partial-differential-equation.md#strong-continuity-from-weak-continuity-and-an-energy-equality):

$$
\boxed{u\in C([0,T];H)}.
$$

<h4 id="1/c/iv">iv</h4>

↑ **Parent:** [C](#1/c)

<h5 id="1/c/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#1/c/iv)

Let $u$ and $v$ be two weak solutions with the same initial value, and put $w=u-v$. Bilinearity gives

$$
w_t+\nu Aw+B(P_Nu,w)+B(P_Nw,v)=0.
$$

Pair with $w$. The first transport term vanishes because $P_Nu$ is divergence free. Part a and the [Young inequality](../../../nonlinear-analysis.md#young-s-inequality-for-products) give

$$
\begin{aligned}
|\langle B(P_Nw,v),w\rangle|
&\leq c\lambda_N^{1/4}|w|\,\|v\|\,\|w\|\\
&\leq\frac\nu2\|w\|^2
+\frac{c^2\lambda_N^{1/2}}{2\nu}
\|v\|^2|w|^2.
\end{aligned}
$$

Therefore

$$
\frac d{dt}|w|^2+\nu\|w\|^2
\leq\frac{c^2\lambda_N^{1/2}}{\nu}
\|v\|^2|w|^2.
$$

The coefficient is integrable because $v\in L^2(0,T;V)$. Since $w(0)=0$, the [Gronwall inequality](../../../probability-and-statistics.md#gronwall-inequality) gives $w=0$ on $[0,T]$. The global weak solution is unique.

## 2

↑ **Parent:** [Paper 359](paper-359.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/i">i</h4>

↑ **Parent:** [A](#2/a)

<h5 id="2/a/i/solution">Solution</h5>

↑ **Parent:** [I](#2/a/i)

For smooth periodic fields, the [Holder inequality](../../../functional-analysis.md#holder-inequality) and $H^1\hookrightarrow L^6$ give

$$
\left|\int_\Omega
(u\mathbin\cdot\nabla v)\mathbin\cdot w\,dx\right|
\leq\|u\|_{L^3}\|\nabla v\|_{L^2}\|w\|_{L^6}
\leq c|u|^{1/2}\|u\|^{1/2}\|v\|\|w\|.
$$

Similarly,

$$
\left|\int_\Omega
(\nabla\mathbin\cdot u)(v\mathbin\cdot w)\,dx\right|
\leq\|\nabla u\|_{L^2}\|v\|_{L^3}\|w\|_{L^6}
\leq c\|u\||v|^{1/2}\|v\|^{1/2}\|w\|.
$$

Adding the bounds proves that the [skew-symmetrized transport form](../../../viscous-fluid-flow.md#skew-symmetrized-transport-form) extends continuously from smooth fields to $\widetilde V^3$ and

$$
\boxed{
|\langle\widetilde B(u,v),w\rangle|
\leq c\left(
|u|^{1/2}\|u\|^{1/2}\|v\|
+|v|^{1/2}\|v\|^{1/2}\|u\|
\right)\|w\|}.
$$

The periodic [Poincaré inequality](../../../sobolev-space.md#poincare-inequality) gives

$$
|u|\leq\mu_1^{-1/2}\|u\|,
\qquad
|v|\leq\mu_1^{-1/2}\|v\|.
$$

Hence

$$
\boxed{
|\langle\widetilde B(u,v),w\rangle|
\leq c\mu_1^{-1/4}\|u\|\|v\|\|w\|}.
$$

<h4 id="2/a/ii">ii</h4>

↑ **Parent:** [A](#2/a)

<h5 id="2/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/a/ii)

Periodic integration by parts gives

$$
\int_\Omega(u\mathbin\cdot\nabla v)\mathbin\cdot w\,dx
=
-\int_\Omega(u\mathbin\cdot\nabla w)\mathbin\cdot v\,dx
-\int_\Omega(\nabla\mathbin\cdot u)(v\mathbin\cdot w)\,dx.
$$

Adding one half of the divergence term to both transport forms yields

$$
\boxed{
\langle\widetilde B(u,v),w\rangle
=-\langle\widetilde B(u,w),v\rangle}.
$$

Density extends the identity from smooth fields to all $u,v,w\in\widetilde V$. In particular,

$$
\boxed{\langle\widetilde B(u,v),v\rangle=0}
$$

without requiring $\nabla\mathbin\cdot u=0$.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/i">i</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/i/solution">Solution</h5>

↑ **Parent:** [I](#2/b/i)

Take the $\widetilde H$ inner product of the finite-dimensional equation with $u_m$. Part a gives exact cancellation of the nonlinear term:

$$
\nu\|u_m\|^2=(f,u_m).
$$

By the [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) and the Poincare inequality,

$$
(f,u_m)\leq|f|\,|u_m|
\leq\mu_1^{-1/2}|f|\,\|u_m\|.
$$

Thus every solution satisfies

$$
\boxed{
\|u_m\|\leq R,
\qquad
R=\frac{|f|}{\nu\mu_1^{1/2}}}.
$$

The bound is independent of $m$.

<h4 id="2/b/ii">ii</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/b/ii)

On $\widetilde H_m$, use the inner product

$$
(v,w)_{\widetilde V}=(\widetilde Av,w)_{\widetilde H}.
$$

The map in the question is continuous, and part a gives

$$
\begin{aligned}
(\Phi_m(v),v)_{\widetilde V}
&=-\|v\|^2
-\frac1\nu\langle\widetilde B(v,v),v\rangle
+\frac1\nu(f,v)\\
&=-\|v\|^2+\frac1\nu(f,v).
\end{aligned}
$$

On the sphere $\|v\|=\rho$ with any $\rho>R$,

$$
(\Phi_m(v),v)_{\widetilde V}
\leq-\rho^2+\frac{|f|}{\nu\mu_1^{1/2}}\rho<0.
$$

The [Brouwer inward-pointing zero lemma](../../../topological-analysis.md#brouwer-inward-pointing-zero-lemma) therefore supplies $v^*$ in the ball with $\Phi_m(v^*)=0$. Multiplication by $\nu\widetilde A$ shows that this zero satisfies

$$
\nu\widetilde Av^*
+\widetilde P_m\widetilde B(v^*,v^*)
=\widetilde P_mf.
$$

**Thus every Galerkin system has at least one solution.**

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/i">i</h4>

↑ **Parent:** [C](#2/c)

<h5 id="2/c/i/solution">Solution</h5>

↑ **Parent:** [I](#2/c/i)

The uniform estimate gives a subsequence

$$
u_m\rightharpoonup u
\quad\hbox{weakly in }\widetilde V,
\qquad
\|u\|\leq R.
$$

The compact periodic embedding $\widetilde V\Subset\widetilde H$ improves this to

$$
u_m\to u
\quad\hbox{strongly in }\widetilde H.
$$

One may also take strong convergence in $L^3$ by the [Rellich-Kondrachov compactness theorem](../../../sobolev-space.md#rellich-kondrachov-theorem). Combining this with weak convergence of the gradients and using the skew form when derivatives must be moved to a test function gives

$$
\widetilde B(u_m,u_m)
\rightharpoonup\widetilde B(u,u)
\quad\hbox{in }\widetilde V'.
$$

For any test function in a fixed finite-dimensional subspace, the Galerkin equation therefore passes to the limit. Density then gives

$$
\boxed{
\nu\widetilde Au+\widetilde B(u,u)=f
\quad\hbox{in }\widetilde V',
\qquad
\|u\|\leq R}.
$$

This is a weak solution of the [steady skew-symmetrized Navier-Stokes equation](../../../viscous-fluid-flow.md#steady-skew-symmetrized-navier-stokes-equation).

<h4 id="2/c/ii">ii</h4>

↑ **Parent:** [C](#2/c)

<h5 id="2/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/c/ii)

Initially $u\in H^1(\Omega)$, so in three dimensions

$$
u\in L^6,\qquad \nabla u\in L^2.
$$

Both terms in

$$
\widetilde B(u,u)
=(u\mathbin\cdot\nabla)u
+\frac12(\nabla\mathbin\cdot u)u
$$

therefore belong to $L^{3/2}$. The equation becomes

$$
-\nu\Delta u=f-\widetilde B(u,u)
\quad\hbox{with right-hand side in }L^{3/2}.
$$

Periodic [elliptic regularity](../../../distribution-theory.md#elliptic-regularity) gives

$$
u\in W^{2,3/2}.
$$

The Sobolev embedding then yields

$$
u\in W^{1,3}\cap L^6.
$$

Consequently each product in $\widetilde B(u,u)$ belongs to $L^2$, because

$$
L^6\cdot L^3\subset L^2.
$$

A second application of [elliptic regularity](../../../distribution-theory.md#elliptic-regularity) now gives

$$
u\in H^2_{\rm per}(\Omega)=D(\widetilde A).
$$

Every term in the equation belongs to $\widetilde H$, and hence

$$
\boxed{
u\in D(\widetilde A),
\qquad
\nu\widetilde Au+\widetilde B(u,u)=f
\quad\hbox{in }\widetilde H}.
$$

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2025](../../2025.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
