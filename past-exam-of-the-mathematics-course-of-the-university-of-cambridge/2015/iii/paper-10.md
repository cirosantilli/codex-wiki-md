# Paper 10

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2015/paper_10.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2015/paper_10.pdf)

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
- [2](#2)
  - [1](#2/1)
    - [Solution](#2/1/solution)
  - [2](#2/2)
    - [Solution](#2/2/solution)
- [3](#3)
  - [1](#3/1)
    - [Solution](#3/1/solution)
  - [2](#3/2)
    - [Solution](#3/2/solution)
  - [3](#3/3)
    - [Solution](#3/3/solution)
- [4](#4)
  - [1](#4/1)
    - [Solution](#4/1/solution)
  - [2](#4/2)
    - [Solution](#4/2/solution)
  - [3](#4/3)
    - [Solution](#4/3/solution)
  - [4](#4/4)
    - [Solution](#4/4/solution)
  - [5](#4/5)
    - [Solution](#4/5/solution)
  - [6](#4/6)
    - [Solution](#4/6/solution)
  - [7](#4/7)
    - [Solution](#4/7/solution)

## 1

↑ **Parent:** [Paper 10](paper-10.md)

<h3 id="1/1">1</h3>

↑ **Parent:** [1](#1)

<h4 id="1/1/solution">Solution</h4>

↑ **Parent:** [1](#1/1)

For the [wave equation](../../../wave-equation.md) with [d'Alembert operator](../../../wave-equation.md#d-alembert-operator) $\Box=-\partial_t^2+\Delta$, the [wave speed](../../../wave-equation.md#wave-speed) is one. **The [domain of dependence](../../../partial-differential-equation.md#domain-of-dependence) of $(t,x)$ is the initial ball $\overline B(x,t)$.** More precisely, two solutions whose [Cauchy data](../../../partial-differential-equation.md#cauchy-data) agree on a neighbourhood of that ball have the same value at $(t,x)$. Thus, if both [Cauchy data](../../../partial-differential-equation.md#cauchy-data) have [support](../../../function.md#support) in $K$, [finite propagation speed](../../../wave-equation.md#finite-propagation-speed) gives

$$
\operatorname{supp}\phi(t,\cdot)\subseteq\{x:\operatorname{dist}(x,K)\leq t\},\qquad t\geq0.
$$

The [Strong Huygens principle](../../../wave-equation.md#strong-huygens-principle) is sharper in three spatial dimensions: **only the initial data on the sphere $|y-x|=t$ contribute**, including the first spatial derivatives of the initial displacement there. The [Kirchhoff formula](../../../wave-equation.md#kirchhoff-formula) makes this precise:

$$
\phi(t,x)=\partial_t\left(\frac{t}{4\pi}\int_{S^2}\phi_0(x+t\omega)\,d\omega\right)
+\frac{t}{4\pi}\int_{S^2}\phi_1(x+t\omega)\,d\omega.
$$

In particular, if the [Cauchy data](../../../partial-differential-equation.md#cauchy-data) have [compact support](../../../function.md#compact-support) in $\overline B(0,R)$, then

$$
\boxed{\phi(t,x)=0\quad\text{whenever}\quad \bigl||x|-t\bigr|>R.}
$$

For $t>R$, the solution therefore vanishes behind the inward edge $|x|=t-R$ as well as outside $|x|=t+R$. The absence of an interior tail is the additional content of the [Strong Huygens principle](../../../wave-equation.md#strong-huygens-principle).

<h3 id="1/2">2</h3>

↑ **Parent:** [1](#1)

<h4 id="1/2/solution">Solution</h4>

↑ **Parent:** [2](#1/2)

We prove [finite propagation speed](../../../wave-equation.md#finite-propagation-speed) using a [shrinking cone energy argument](../../../wave-equation.md#shrinking-cone-energy-argument). Fix $T>0$ and $x_*$, and suppose the [Cauchy data](../../../partial-differential-equation.md#cauchy-data) vanish on $B(x_*,T)$. For $0\leq s<T$, define the local [wave energy](../../../wave-equation.md#wave-energy)

$$
e=\frac12\bigl(\phi_t^2+|\nabla\phi|^2\bigr),\qquad
E(s)=\int_{B(x_*,T-s)}e(s,x)\,dx.
$$

The homogeneous [wave equation](../../../wave-equation.md) gives the local [conservation law](../../../physics.md#conservation-law)

$$
\partial_t e=\nabla\cdot(\phi_t\nabla\phi).
$$

Differentiate the integral over the moving ball. Its boundary moves inward with speed one, so the [divergence theorem](../../../calculus.md#divergence-theorem) gives

$$
E'(s)=\int_{\partial B(x_*,T-s)}\bigl(\phi_t\partial_n\phi-e\bigr)\,dS
=-\frac12\int_{\partial B(x_*,T-s)}
\left((\phi_t-\partial_n\phi)^2+|\nabla_{\mathrm{tan}}\phi|^2\right)\,dS\leq0.
$$

Here $n$ is the outward [unit normal](../../../differential-geometry.md#unit-normal), $\partial_n$ the [normal derivative](../../../differential-geometry.md#normal-derivative), and $\nabla_{\mathrm{tan}}$ the component of the [gradient](../../../calculus.md#gradient) tangent to the boundary. Since $E(0)=0$ and $e\geq0$, we have $E(s)=0$. Hence both $\phi_t$ and $\nabla\phi$ vanish inside the backward [light cone](../../../special-relativity.md#light-cone). Integrating $\phi_t(s,x_*)=0$ from the zero initial displacement gives $\phi(s,x_*)=0$; [continuity](../../../calculus.md#continuous-function) then gives $\phi(T,x_*)=0$.

Applying the same [energy estimate](../../../partial-differential-equation.md#energy-estimate) to the difference of two solutions proves the [domain of dependence](../../../partial-differential-equation.md#domain-of-dependence) assertion. If $\operatorname{dist}(x_*,K)>T$, the initial ball misses $K$, and the preceding argument proves the stated [support](../../../function.md#support) bound. **No disturbance propagates faster than one.**

<h3 id="1/3">3</h3>

↑ **Parent:** [1](#1)

<h4 id="1/3/solution">Solution</h4>

↑ **Parent:** [3](#1/3)

For a [radial function](../../../partial-differential-equation.md#radial-function), the [Laplacian](../../../calculus.md#laplacian) is $\Delta\phi=\phi_{rr}+2\phi_r/r$. Introduce the [retarded and advanced null coordinates](../../../special-relativity.md#retarded-and-advanced-null-coordinates) and the [radial reduction of the three-dimensional wave equation](../../../wave-equation.md#radial-reduction-of-the-three-dimensional-wave-equation):

$$
u=t-r,\qquad v=t+r,\qquad r=\frac{v-u}{2},\qquad w=r\phi.
$$

The [chain rule](../../../calculus.md#chain-rule) gives $\partial_t=\partial_u+\partial_v$ and $\partial_r=-\partial_u+\partial_v$. Consequently the inhomogeneous [wave equation](../../../wave-equation.md) is

$$
\boxed{-4\phi_{uv}+\frac{4}{v-u}(\phi_v-\phi_u)=F.}
$$

Multiplying the radial [wave equation](../../../wave-equation.md) by $r$ removes its first-order radial derivative:

$$
-w_{tt}+w_{rr}=rF.
$$

Thus the particularly useful [retarded and advanced null coordinates](../../../special-relativity.md#retarded-and-advanced-null-coordinates) form is

$$
\boxed{-4w_{uv}=rF,\qquad
\partial_u\partial_v\bigl((v-u)\phi\bigr)=-\frac{v-u}{4}F.}
$$

These formulas hold for $r>0$. At the axis, smooth [spherical symmetry](../../../geometry-and-topology.md#spherical-symmetry) imposes $\phi_r(t,0)=0$ and $w(t,0)=0$; equivalently $w$ has a smooth [odd extension](../../../calculus.md#odd-extension) across $r=0$.

<h3 id="1/4">4</h3>

↑ **Parent:** [1](#1)

<h4 id="1/4/solution">Solution</h4>

↑ **Parent:** [4](#1/4)

Use the [radial reduction of the three-dimensional wave equation](../../../wave-equation.md#radial-reduction-of-the-three-dimensional-wave-equation) $w=r\phi$ and extend $w$ oddly in $r$. Write $w=w_h+w_F$, where $w_h$ is the homogeneous [wave equation](../../../wave-equation.md) solution with the prescribed [Cauchy data](../../../partial-differential-equation.md#cauchy-data), and $w_F$ has zero [Cauchy data](../../../partial-differential-equation.md#cauchy-data). With $w_0(r)=r\phi_0(r)$ and $w_1(r)=r\phi_1(r)$, the [D'Alembert formula](../../../wave-equation.md#d-alembert-s-formula) gives

$$
w_h(t,r)=\frac{w_0(r-t)+w_0(r+t)}2+\frac12\int_{r-t}^{r+t}w_1(\rho)\,d\rho.
$$

Both odd initial profiles have [compact support](../../../function.md#compact-support), so

$$
|w_h(t,r)|\leq A,\qquad A=\|w_0\|_\infty+\frac12\|w_1\|_1.
$$

The [Duhamel principle](../../../diffusion-equation.md#duhamel-s-principle), applied to $w_{tt}-w_{rr}=-rF$, gives

$$
w_F(t,r)=-\frac12\int_0^t\int_{r-(t-s)}^{r+(t-s)}\rho F(s,\rho)\,d\rho\,ds.
$$

Now write $r=t+a$ with $1/2\leq a\leq1$. The lower integration limit is $s+a>0$, so this [domain of dependence](../../../partial-differential-equation.md#domain-of-dependence) never crosses the axis. Intersecting its integration interval with the [support](../../../function.md#support) of the source leaves a subset of $[s+a,s+1]$, of length at most one. On this interval,

$$
\rho |F(s,\rho)|\leq\frac{s+1}{(1+s)^2}=\frac1{1+s}.
$$

The [outgoing shell source estimate for a radial wave](../../../wave-equation.md#outgoing-shell-source-estimate-for-a-radial-wave) therefore yields

$$
|w_F(t,t+a)|\leq\frac12\int_0^t\frac{ds}{1+s}=\frac12\log(1+t).
$$

Finally $r\geq t+1/2\geq(1+t)/2$, and thus

$$
|\phi(t,t+a)|\leq\frac{2A+\log(1+t)}{1+t}
\leq\boxed{\frac{C\log(2+t)}{1+t}},\qquad C=1+\frac{2A}{\log2}.
$$

This constant depends only on the [Cauchy data](../../../partial-differential-equation.md#cauchy-data) and the fixed unit bound for the source. The logarithm comes from integrating the shell's accumulated forcing, whereas the factor $(1+t)^{-1}$ comes from division by $r$.

<h2 id="2">2</h2>

↑ **Parent:** [Paper 10](paper-10.md)

<h3 id="2/1">1</h3>

↑ **Parent:** [2](#2)

<h4 id="2/1/solution">Solution</h4>

↑ **Parent:** [1](#2/1)

One version of the [Klainerman-Sobolev inequality](../../../wave-equation.md#klainerman-sobolev-inequality), for a sufficiently decaying [smooth function](../../../analysis.md#smooth-function) $\psi$ on $\mathbb R^{1+3}$, is

$$
\boxed{|\psi(t,x)|\leq
\frac{C}{(1+t+|x|)(1+|t-|x||)^{1/2}}
\sum_{|I|\leq2}\|Z^I\psi(t,\cdot)\|_{L^2(\mathbb R^3)}},\qquad t\geq0.
$$

Here $I$ denotes a word of length $|I|$ in the following eleven [commutation vector fields for the wave equation](../../../wave-equation.md#commutation-vector-field-for-the-wave-equation):

$$
\begin{aligned}
&\partial_t,\ \partial_1,\ \partial_2,\ \partial_3, &&\text{spacetime translations},\\
&\Omega_{ij}=x_i\partial_j-x_j\partial_i\quad(1\leq i<j\leq3), &&\text{spatial rotations},\\
&L_i=t\partial_i+x_i\partial_t\quad(1\leq i\leq3), &&\text{Lorentz boosts},\\
&S=t\partial_t+\sum_{i=1}^3x_i\partial_i, &&\text{scaling}.
\end{aligned}
$$

The first four are [spacetime translation vector fields](../../../wave-equation.md#spacetime-translation-vector-field); the next three are [spatial rotation vector fields](../../../wave-equation.md#spatial-rotation-vector-field); the next three are [Lorentz boost vector fields](../../../wave-equation.md#lorentz-boost-vector-field); and $S$ is the [scaling vector field](../../../wave-equation.md#scaling-vector-field). The [vector field method for wave equations](../../../wave-equation.md#vector-field-method-for-wave-equations) uses these [vector fields](../../../calculus.md#vector-field) because their [commutators](../../../lie-algebra.md#commutator) with the [d'Alembert operator](../../../wave-equation.md#d-alembert-operator) obey

$$
[\Box,Z]=0\quad(Z\ne S),\qquad [\Box,S]=2\Box.
$$

In particular the [Klainerman-Sobolev inequality](../../../wave-equation.md#klainerman-sobolev-inequality) implies

$$
\|\psi(t,\cdot)\|_\infty\leq\frac{C}{1+t}\sum_{|I|\leq2}\|Z^I\psi(t,\cdot)\|_2.
$$

The displayed [L2 norms](../../../real-analysis.md#l2-norm) are spatial norms at fixed time; the spacetime [vector fields](../../../calculus.md#vector-field) can contain time derivatives. No [wave equation](../../../wave-equation.md) assumption is needed for the [Klainerman-Sobolev inequality](../../../wave-equation.md#klainerman-sobolev-inequality) itself.

<h3 id="2/2">2</h3>

↑ **Parent:** [2](#2)

<h4 id="2/2/solution">Solution</h4>

↑ **Parent:** [2](#2/2)

We establish a quantitative [almost global existence for wave equations](../../../wave-equation.md#almost-global-existence-for-wave-equations) estimate. Take $0<\varepsilon\leq1$, fix an integer $m\geq6$, and use the [commutation vector fields for the wave equation](../../../wave-equation.md#commutation-vector-field-for-the-wave-equation) from the preceding part. Put $\partial=(\partial_t,\nabla)$ and define the [commuted wave energy](../../../wave-equation.md#commuted-wave-energy)

$$
A_m(t)=\sum_{|I|\leq m}\|\partial Z^I\phi(t)\|_2.
$$

All these [L2 norms](../../../real-analysis.md#l2-norm) are finite on any smooth existence interval by [finite propagation speed](../../../wave-equation.md#finite-propagation-speed). At $t=0$, the polynomial coefficients of the [vector fields](../../../calculus.md#vector-field) are bounded on the fixed [compact support](../../../function.md#compact-support) of the [Cauchy data](../../../partial-differential-equation.md#cauchy-data). Whenever a higher time derivative occurs, use $\phi_{tt}=\Delta\phi-\phi_t^2$ and its differentiated versions to express it in terms of initial spatial derivatives. Every term contains at least one factor of $\varepsilon$; consequently

$$
A_m(0)\leq C_0\varepsilon
$$

for a constant depending only on finitely many derivatives and the [support](../../../function.md#support) radius of $\phi_0,\phi_1$.

The [commutators](../../../lie-algebra.md#commutator) $[Z,\partial_\mu]$ are constant linear combinations of translations. Together with $[\Box,S]=2\Box$ and the [Leibniz rule](../../../calculus.md#leibniz-rule), this shows that each commuted source is a finite linear combination of products

$$
\partial_\mu Z^J\phi\,\partial_\nu Z^K\phi,\qquad |J|+|K|\leq |I|.
$$

This statement includes the extra copies of the original source produced by the [scaling vector field](../../../wave-equation.md#scaling-vector-field). In each product put the factor with fewer commutations in the [Lp norm](../../../real-analysis.md#lp-norm) $L^\infty$ and the other in the [L2 norm](../../../real-analysis.md#l2-norm). The lower order is at most $\lfloor m/2\rfloor$. Applying the [Klainerman-Sobolev inequality](../../../wave-equation.md#klainerman-sobolev-inequality) to $\partial_\mu Z^J\phi$ costs at most two additional commutations; commuting those past $\partial_\mu$ introduces only lower-order translations. Since $\lfloor m/2\rfloor+2\leq m$,

$$
\sum_{|I|\leq m}\|\Box Z^I\phi(t)\|_2\leq\frac{C_m}{1+t}A_m(t)^2.
$$

The inhomogeneous [wave energy estimate](../../../partial-differential-equation.md#wave-energy-estimate) now gives

$$
A_m(t)\leq C_0\varepsilon+C_m\int_0^t\frac{A_m(s)^2}{1+s}\,ds.
$$

Let $T_\varepsilon=\varepsilon^{-N}$. Use a [bootstrap argument](../../../partial-differential-equation.md#bootstrap-argument) with $A_m(t)\leq2C_0\varepsilon$ up to the smaller of $T_\varepsilon$ and the maximal existence time. The [energy estimate](../../../partial-differential-equation.md#energy-estimate) improves this to

$$
A_m(t)\leq C_0\varepsilon+4C_mC_0^2\varepsilon^2\log(1+T_\varepsilon).
$$

For each fixed $N$,

$$
\varepsilon\log(1+\varepsilon^{-N})\longrightarrow0\quad\text{as}\quad\varepsilon\downarrow0.
$$

Choose $\varepsilon_N\leq1$ so that $4C_mC_0\varepsilon\log(1+\varepsilon^{-N})\leq1/2$ for every $0<\varepsilon\leq\varepsilon_N$. Then $A_m(t)\leq(3/2)C_0\varepsilon$, a strict improvement. A [continuity](../../../calculus.md#continuous-function) argument closes the [bootstrap argument](../../../partial-differential-equation.md#bootstrap-argument).

Finally, the translation terms in $A_m$ control ordinary spatial [Sobolev norms](../../../sobolev-space.md#sobolev-norm) of $\partial\phi$. The missing [L2 norm](../../../real-analysis.md#l2-norm) of $\phi$ satisfies

$$
\|\phi(t)\|_2\leq\varepsilon\|\phi_0\|_2+\int_0^t\|\phi_t(s)\|_2\,ds.
$$

Thus the full local-existence [Sobolev norms](../../../sobolev-space.md#sobolev-norm) remain bounded on this finite interval. The [smooth continuation criterion for semilinear wave equations](../../../wave-equation.md#smooth-continuation-criterion-for-semilinear-wave-equations) extends the solution past any finite endpoint before $T_\varepsilon$. To see smooth persistence explicitly, the [tame Sobolev product estimate](../../../sobolev-space.md#tame-sobolev-product-estimate) gives $\|\phi_t^2\|_{H^k}\leq C_k\|\phi_t\|_\infty\|\phi_t\|_{H^k}$. Ordinary differentiated [wave energy estimates](../../../partial-differential-equation.md#wave-energy-estimate) therefore bound each higher derivative energy by its initial value times $\exp(C_k\int_0^t\|\phi_t(s)\|_\infty\,ds)$. This is finite on the interval already controlled by the base [commuted wave energy](../../../wave-equation.md#commuted-wave-energy); no separate $\varepsilon_N$ is needed for each derivative order. Therefore

$$
\boxed{\text{the solution is smooth on }[0,\varepsilon^{-N}]\text{ for }0<\varepsilon\leq\varepsilon_N.}
$$

For $\varepsilon=0$ the zero solution is global. The same [energy estimate](../../../partial-differential-equation.md#energy-estimate) in fact permits an exponential lower bound for the lifespan, which is stronger than any fixed inverse power.

<h2 id="3">3</h2>

↑ **Parent:** [Paper 10](paper-10.md)

<h3 id="3/1">1</h3>

↑ **Parent:** [3](#3)

<h4 id="3/1/solution">Solution</h4>

↑ **Parent:** [1](#3/1)

The sign convention makes this a [defocusing semilinear wave equation](../../../wave-equation.md#defocusing-semilinear-wave-equation):

$$
\phi_{tt}-\Delta\phi+\phi^3=0.
$$

Its [wave energy](../../../wave-equation.md#wave-energy) includes a nonnegative potential term:

$$
\boxed{E(t)=\int_{\mathbb R^3}\left(\frac12\phi_t^2+\frac12|\nabla\phi|^2+\frac14\phi^4\right)\,dx=E(0).}
$$

For a [smooth function](../../../analysis.md#smooth-function) solution, [finite propagation speed](../../../wave-equation.md#finite-propagation-speed) preserves [compact support](../../../function.md#compact-support) on finite time intervals. Differentiate under the integral and use [integration by parts](../../../calculus.md#integration-by-parts):

$$
\frac{dE}{dt}=\int_{\mathbb R^3}\phi_t\bigl(\phi_{tt}-\Delta\phi+\phi^3\bigr)\,dx=0.
$$

Equivalently the local [conservation law](../../../physics.md#conservation-law) has density $e=\phi_t^2/2+|\nabla\phi|^2/2+\phi^4/4$ and flux $-\phi_t\nabla\phi$. All three terms are nonnegative, and $E=0$ forces both [Cauchy data](../../../partial-differential-equation.md#cauchy-data) to vanish. Hence this is a positive conserved [energy](../../../classical-mechanics.md#energy), rather than the indefinite energy associated with the opposite sign.

<h3 id="3/2">2</h3>

↑ **Parent:** [3](#3)

<h4 id="3/2/solution">Solution</h4>

↑ **Parent:** [2](#3/2)

We use the homogeneous version of the [Sobolev embedding theorem](../../../sobolev-space.md#sobolev-embedding-theorem) in three dimensions:

$$
\|h\|_{L^6(\mathbb R^3)}\leq C_S\|\nabla h\|_{L^2(\mathbb R^3)},\qquad h\in\dot H^1(\mathbb R^3).
$$

Here [homogeneous Sobolev space](../../../sobolev-space.md#homogeneous-sobolev-space) $\dot H^1$ is the completion of compactly supported [smooth functions](../../../analysis.md#smooth-function) in the [L2 norm](../../../real-analysis.md#l2-norm) of the [gradient](../../../calculus.md#gradient), identified with its $L^6$ representative. Apply this [Sobolev inequality](../../../sobolev-space.md#sobolev-inequality) both to $\phi$ and to its [spatial derivatives](../../../calculus.md#spatial-derivative).

Let

$$
B(t)=\left(\sum_{i=1}^3\|\partial_i\phi_t(t)\|_2^2+
\sum_{i,j=1}^3\|\partial_i\partial_j\phi(t)\|_2^2\right)^{1/2}.
$$

The [Plancherel theorem](../../../fourier-analysis.md#plancherel-theorem) identifies the [L2 norm](../../../real-analysis.md#l2-norm) of the [Hessian matrix](../../../calculus.md#hessian-matrix) with $\|\phi\|_{\dot H^2}$, because $\sum_{i,j}\xi_i^2\xi_j^2=|\xi|^4$. In particular,

$$
\|\phi\|_{\dot H^2}+\|\phi_t\|_{\dot H^1}\leq\sqrt2 B(t),\qquad B(0)\leq D.
$$

Differentiating the [defocusing semilinear wave equation](../../../wave-equation.md#defocusing-semilinear-wave-equation) gives $\Box(\partial_i\phi)=3\phi^2\partial_i\phi$. By the [Holder inequality](../../../functional-analysis.md#holder-inequality) with exponents $3$ and $6$, the preceding [Sobolev inequality](../../../sobolev-space.md#sobolev-inequality), and conservation of the positive [wave energy](../../../wave-equation.md#wave-energy),

$$
\begin{aligned}
\|\phi^2\nabla\phi\|_2
&\leq\|\phi\|_6^2\|\nabla\phi\|_6\\
&\leq C\|\nabla\phi\|_2^2\|D_x^2\phi\|_2
\leq 2CE B(t).
\end{aligned}
$$

Use the inhomogeneous [wave energy estimate](../../../partial-differential-equation.md#wave-energy-estimate) simultaneously for the three [spatial derivatives](../../../calculus.md#spatial-derivative). It gives

$$
B(t)\leq B(0)+C E\int_0^t B(s)\,ds.
$$

The [Gronwall inequality](../../../probability-and-statistics.md#gronwall-inequality) therefore yields $B(t)\leq D\exp(C E t)$. We may take the continuous, locally bounded function

$$
\boxed{f(T)=\sqrt2 D\exp(C E T).}
$$

The constant is universal; the dependence on the initial data is only through $D$ and $E$. The [H2 bound for the defocusing cubic wave equation](../../../wave-equation.md#h2-bound-for-the-defocusing-cubic-wave-equation) holds on every existing smooth interval, without assuming the global conclusion. If $D=0$ or $E=0$, the zero solution satisfies the same estimate.

<h3 id="3/3">3</h3>

↑ **Parent:** [3](#3)

<h4 id="3/3/solution">Solution</h4>

↑ **Parent:** [3](#3/3)

The opposite sign is the [focusing semilinear wave equation](../../../wave-equation.md#focusing-semilinear-wave-equation) $\phi_{tt}-\Delta\phi=\phi^3$. Begin with a spatially constant solution, reducing the [partial differential equation](../../../partial-differential-equation.md) to the [ordinary differential equation](../../../differential-equation.md#ordinary-differential-equation) $a''=a^3$. Substitution of $a(t)=\beta(t-1)^{-\alpha}$ gives

$$
\alpha(\alpha+1)\beta(t-1)^{-\alpha-2}=\beta^3(t-1)^{-3\alpha}.
$$

For a nonzero profile, equality of powers and coefficients gives $\alpha=1$ and $\beta^2=2$. Choose

$$
a(t)=\frac{\sqrt2}{1-t},\qquad a(0)=a'(0)=\sqrt2.
$$

To obtain [compact support](../../../function.md#compact-support), take a [smooth cutoff function](../../../analysis.md#smooth-cutoff-function) $\chi$ equal to one on $B(0,2)$ and zero outside $B(0,3)$, and prescribe

$$
\phi_0=\sqrt2\chi,\qquad\phi_1=\sqrt2\chi.
$$

These are smooth, compactly supported [Cauchy data](../../../partial-differential-equation.md#cauchy-data). By [finite propagation speed](../../../wave-equation.md#finite-propagation-speed), the local solution agrees with $a(t)$ throughout $|x|<2-t$ for $0\leq t<\min(1,T_*)$, where $T_*$ is its maximal forward smooth existence time.

For completeness, the semilinear [domain of dependence](../../../partial-differential-equation.md#domain-of-dependence) assertion follows by comparing two solutions: their difference $z$ obeys $z_{tt}-\Delta z=bz$, with $b=\phi^2+\phi a+a^2$. On any compact time interval before $t=1$ on which the solutions are smooth, $b$ is bounded in the backward [light cone](../../../special-relativity.md#light-cone). Add $z^2/2$ to the shrinking-ball [wave energy](../../../wave-equation.md#wave-energy); its derivative is bounded above by $C$ times that energy, with the same nonpositive boundary flux. Zero initial difference and the [Gronwall inequality](../../../probability-and-statistics.md#gronwall-inequality) give $z=0$ there.

If $T_*>1$, the identity at the origin would imply $\phi(t,0)=\sqrt2/(1-t)$ as $t\uparrow1$, contradicting smoothness at $t=1$. Thus

$$
\boxed{T_*\leq1<\infty.}
$$

If the solution loses regularity earlier, that is already finite-time blowup. The usual [smooth continuation criterion for semilinear wave equations](../../../wave-equation.md#smooth-continuation-criterion-for-semilinear-wave-equations) precludes a finite maximal time with all continuation norms bounded. This [localized ordinary differential equation blowup for a wave equation](../../../wave-equation.md#localized-ordinary-differential-equation-blowup-for-a-wave-equation) therefore supplies the required compactly supported examples.

<h2 id="4">4</h2>

↑ **Parent:** [Paper 10](paper-10.md)

<h3 id="4/1">1</h3>

↑ **Parent:** [4](#4)

<h4 id="4/1/solution">Solution</h4>

↑ **Parent:** [1](#4/1)

**Compatible [Cauchy data](../../../partial-differential-equation.md#cauchy-data)** for a [wave map](../../../wave-equation.md#wave-map) are $\phi_0:\mathbb R^n\to S^2$ and $\phi_1(x)\in T_{\phi_0(x)}S^2$: thus $|\phi_0|=1$ and $\phi_0\cdot\phi_1=0$. Smooth localized [wave map Cauchy data](../../../wave-equation.md#wave-map-cauchy-data) equal a constant $p\in S^2$ with zero velocity outside a compact set. It is $\phi_0-p$, rather than the [sphere](../../../geometry-and-topology.md#sphere)-valued map itself, that has [compact support](../../../function.md#compact-support). The geometric constraints propagate under the [wave map](../../../wave-equation.md#wave-map) equation.

<h3 id="4/2">2</h3>

↑ **Parent:** [4](#4)

<h4 id="4/2/solution">Solution</h4>

↑ **Parent:** [2](#4/2)

**Smooth compatible [wave map Cauchy data](../../../wave-equation.md#wave-map-cauchy-data) give a unique local smooth [wave map](../../../wave-equation.md#wave-map).** Relative to a constant map, [Sobolev spaces](../../../sobolev-space.md) $H^s\times H^{s-1}$ with $s>n/2+1$ provide a classical local theory. Iteration for the [semilinear wave equation](../../../wave-equation.md#semilinear-wave-equation), [Sobolev algebra](../../../sobolev-space.md#sobolev-algebra) and [energy estimates](../../../partial-differential-equation.md#energy-estimate) give existence, uniqueness and continuous dependence. The [smooth continuation criterion for semilinear wave equations](../../../wave-equation.md#smooth-continuation-criterion-for-semilinear-wave-equations) extends the solution while these norms stay bounded. The [sphere](../../../geometry-and-topology.md#sphere) constraint and tangency constraint remain satisfied.

<h3 id="4/3">3</h3>

↑ **Parent:** [4](#4)

<h4 id="4/3/solution">Solution</h4>

↑ **Parent:** [3](#4/3)

**[Harmonic maps](../../../differential-geometry.md#harmonic-map) give nonconstant [stationary wave maps](../../../wave-equation.md#stationary-wave-map).** For $n=2$, inverse [stereographic projection](../../../complex-analysis.md#stereographic-projection) gives

$$
Q(x)=\frac{(2x_1,2x_2,|x|^2-1)}{1+|x|^2}.
$$

It satisfies $|Q|=1$ and $\Delta Q=-|\nabla Q|^2Q$, so $\phi(t,x)=Q(x)$ is a smooth global [wave map](../../../wave-equation.md#wave-map). Its [wave map energy](../../../wave-equation.md#wave-map-energy) is $4\pi$, since $|\nabla Q|^2=8/(1+|x|^2)^2$. Translations and rescalings give further examples; these [harmonic maps](../../../differential-geometry.md#harmonic-map) approach a constant at infinity.

<h3 id="4/4">4</h3>

↑ **Parent:** [4](#4)

<h4 id="4/4/solution">Solution</h4>

↑ **Parent:** [4](#4/4)

The [wave map](../../../wave-equation.md#wave-map) [scaling symmetry](../../../partial-differential-equation.md#scaling-symmetry) is $\phi_\lambda(t,x)=\phi(t/\lambda,x/\lambda)$. Its conserved [wave map energy](../../../wave-equation.md#wave-map-energy) is

$$
E=\frac12\int(|\phi_t|^2+|\nabla\phi|^2)\,dx,\qquad E(\phi_\lambda)=\lambda^{n-2}E(\phi).
$$

Thus **energy is subcritical for $n=1$, critical for $n=2$, and supercritical for $n\geq3$**. The scaling-critical [homogeneous Sobolev spaces](../../../sobolev-space.md#homogeneous-sobolev-space) for perturbations of a constant map are $\dot H^{n/2}\times\dot H^{n/2-1}$. These relations constitute [wave map energy and criticality](../../../wave-equation.md#wave-map-energy-and-criticality).

<h3 id="4/5">5</h3>

↑ **Parent:** [4](#4)

<h4 id="4/5/solution">Solution</h4>

↑ **Parent:** [5](#4/5)

**[Global regularity for one-dimensional wave maps](../../../wave-equation.md#global-regularity-for-one-dimensional-wave-maps) holds for arbitrary smooth localized compatible data.** In [retarded and advanced null coordinates](../../../special-relativity.md#retarded-and-advanced-null-coordinates) $u=t-x$, $v=t+x$, the [wave map](../../../wave-equation.md#wave-map) equation says $D_v\phi_u=D_u\phi_v=0$, with $D$ the target [covariant derivative](../../../general-relativity.md#covariant-derivative). Hence $|\phi_u|^2$ depends only on $u$, and $|\phi_v|^2$ only on $v$. Initial derivative bounds persist. Compactness of the [sphere](../../../geometry-and-topology.md#sphere) and differentiated [energy estimates](../../../partial-differential-equation.md#energy-estimate) then prevent finite-time loss of smoothness.

<h3 id="4/6">6</h3>

↑ **Parent:** [4](#4)

<h4 id="4/6/solution">Solution</h4>

↑ **Parent:** [6](#4/6)

**[Small data global regularity for wave maps](../../../wave-equation.md#small-data-global-regularity-for-wave-maps) holds in four spatial dimensions.** Smallness is measured in sufficiently high weighted [Sobolev norms](../../../sobolev-space.md#sobolev-norm) relative to a constant map, with localized compatible [Cauchy data](../../../partial-differential-equation.md#cauchy-data). The [vector field method for wave equations](../../../wave-equation.md#vector-field-method-for-wave-equations) gives derivative decay $(1+t)^{-3/2}$. This is time-integrable, so [commuted wave energy](../../../wave-equation.md#commuted-wave-energy) estimates close a small-data [bootstrap argument](../../../partial-differential-equation.md#bootstrap-argument) for the derivative-quadratic [semilinear wave equation](../../../wave-equation.md#semilinear-wave-equation). Higher regularity persists. No smallness of energy alone is asserted.

<h3 id="4/7">7</h3>

↑ **Parent:** [4](#4)

<h4 id="4/7/solution">Solution</h4>

↑ **Parent:** [7](#4/7)

**[Small data global regularity for wave maps](../../../wave-equation.md#small-data-global-regularity-for-wave-maps) also holds in three spatial dimensions.** For localized compatible data small in high weighted [Sobolev norms](../../../sobolev-space.md#sobolev-norm), the key is the [classical null condition for wave equations](../../../wave-equation.md#classical-null-condition-for-wave-equations). Each derivative contraction is a [null form for wave equations](../../../wave-equation.md#null-form-for-wave-equations), vanishing for parallel null derivatives. The [vector field method for wave equations](../../../wave-equation.md#vector-field-method-for-wave-equations) exploits derivatives tangent to the [light cone](../../../special-relativity.md#light-cone) and weighted [energy estimates](../../../partial-differential-equation.md#energy-estimate) to close the [bootstrap argument](../../../partial-differential-equation.md#bootstrap-argument); ordinary $(1+t)^{-1}$ decay alone is insufficient.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2015](../../2015.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
