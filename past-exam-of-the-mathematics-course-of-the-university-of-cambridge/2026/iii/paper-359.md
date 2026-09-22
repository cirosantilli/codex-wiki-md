# Paper 359

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2026/III%20Paper%20359.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2026/III%20Paper%20359.pdf)

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
    - [iii](#1/b/iii)
      - [Solution](#1/b/iii/solution)
  - [c](#1/c)
    - [i](#1/c/i)
      - [Solution](#1/c/i/solution)
    - [ii](#1/c/ii)
      - [Solution](#1/c/ii/solution)
  - [d](#1/d)
    - [Solution](#1/d/solution)
  - [e](#1/e)
    - [Solution](#1/e/solution)
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
    - [Solution](#2/c/solution)
  - [d](#2/d)
    - [Solution](#2/d/solution)

## 1

↑ **Parent:** [Paper 359](paper-359.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/i">i</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/i/solution">Solution</h5>

↑ **Parent:** [I](#1/a/i)

The [sobolev embedding theorem](../../../sobolev-space.md#sobolev-embedding-theorem) in three dimensions and the [periodic elliptic estimate](../../../sobolev-space.md#periodic-elliptic-estimate) for the [Stokes operator](../../../viscous-fluid-flow.md#stokes-operator) give

$$
\|(v\mathbin\cdot\nabla)\eta\|_2
\leq \|v\|_\infty\|\nabla\eta\|_2
\leq C\|v\|_{H^2}\|\eta\|_{H^1}
\leq C|Av|\|\eta\|_{H^1}.
$$

The last step uses the absence of the zero Fourier mode: on mean-zero periodic fields, the [Poincaré inequality](../../../sobolev-space.md#poincare-inequality) makes the homogeneous $H^2$ norm controlled by $\|\Delta v\|_2=|Av|$.

<h4 id="1/a/ii">ii</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/a/ii)

Because $v$ is a [divergence-free vector field](../../../fluid-mechanics.md#divergence-free-vector-field), the [product rule](../../../calculus.md#product-rule) gives

$$
\nabla\mathbin\cdot(v\eta\chi)
=(v\mathbin\cdot\nabla\eta)\chi
+(v\mathbin\cdot\nabla\chi)\eta.
$$

The integral of a divergence over the [periodic domain](../../../partial-differential-equation.md#periodic-domain) vanishes. Hence [integration by parts](../../../calculus.md#integration-by-parts) yields

$$
\boxed{\int_\Omega((v\mathbin\cdot\nabla)\eta)\chi\,dx
=-\int_\Omega((v\mathbin\cdot\nabla)\chi)\eta\,dx}.
$$

This is the [skew-symmetry of incompressible transport](../../../viscous-fluid-flow.md#skew-symmetry-of-incompressible-transport).

<h4 id="1/a/iii">iii</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#1/a/iii)

Set $\chi=\eta$ in part (ii). The integral is equal to its own negative, so

$$
\boxed{\int_\Omega((v\mathbin\cdot\nabla)\eta)\eta\,dx=0}.
$$

Equivalently, incompressible advection does not change the scalar's quadratic energy.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/i">i</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/i/solution">Solution</h5>

↑ **Parent:** [I](#1/b/i)

Both $P_m$ and the [Leray-Helmholtz projection](../../../viscous-fluid-flow.md#leray-helmholtz-projection) are [orthogonal projections](../../../hilbert-space.md#orthogonal-projection), hence contractions in $L^2$. Taking the $H$ norm of the first Galerkin equation gives

$$
\nu|Au_m|
=\alpha|P_mP_\sigma(\theta_me_3)|
\leq\alpha\|\theta_me_3\|_2
=\alpha\|\theta_m\|_2.
$$

Therefore

$$
\boxed{|Au_m|\leq\frac{\alpha}{\nu}\|\theta_m\|_2}.
$$

<h4 id="1/b/ii">ii</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/b/ii)

The first equation determines $u_m$ linearly from $\theta_m$:

$$
u_m=\frac{\alpha}{\nu}A^{-1}P_mP_\sigma(\theta_me_3).
$$

Substitution into the second equation gives an [ordinary differential equation](../../../differential-equation.md#ordinary-differential-equation) on the finite-dimensional space $\widetilde H_m$. Its right-hand side is polynomial, and therefore locally [Lipschitz continuous](../../../real-analysis.md#lipschitz-continuity). The [Picard-Lindelöf theorem](../../../differential-equation.md#picard-lindelof-theorem) supplies a unique local solution. The [energy estimate](../../../partial-differential-equation.md#energy-estimate) in part (iii) bounds $\theta_m$ on every finite time interval, so the [finite-dimensional continuation criterion](../../../differential-equation.md#finite-dimensional-continuation-criterion) rules out finite-time escape. The solution is consequently unique on every interval $[0,T]$.

<h4 id="1/b/iii">iii</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#1/b/iii)

Take the $L^2$ inner product of the temperature equation with $\theta_m$. The spectral projection disappears against $\theta_m\in\widetilde H_m$, and part (a)(iii) cancels transport. Thus

$$
\frac12\frac d{dt}\|\theta_m\|_2^2
+\kappa\|\nabla\theta_m\|_2^2
=\beta(u_m\mathbin\cdot e_3,\theta_m).
$$

The periodic [Poincaré inequality](../../../sobolev-space.md#poincare-inequality), part (i), and the [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) imply

$$
|(u_m\mathbin\cdot e_3,\theta_m)|
\leq |u_m|\|\theta_m\|_2
\leq C|Au_m|\|\theta_m\|_2
\leq C\frac{\alpha}{\nu}\|\theta_m\|_2^2.
$$

The [Gronwall inequality](../../../probability-and-statistics.md#gronwall-inequality) therefore gives, for $0\leq t\leq T$,

$$
\|\theta_m(t)\|_2^2
\leq e^{C\alpha\beta T/\nu}\|\theta_0\|_2^2.
$$

This defines a bound $K_0(T)$ independent of $m$, and part (i) then gives

$$
\|Au_m\|_{L^\infty(0,T;H)}
\leq\frac{\alpha}{\nu}K_0(T)=:K_2(T).
$$

Integrating the energy identity and using the same bound on its right-hand side gives

$$
\|\theta_m\|_{L^2(0,T;H^1_{\rm per})}\leq K_1(T).
$$

It remains to estimate the time derivative. For $\varphi\in H^1_{\rm per}$, the Fourier projection $\Pi_m$ is a contraction in $H^1$, and the skew identity from part (a) gives

$$
|\langle\Pi_m((u_m\mathbin\cdot\nabla)\theta_m),\varphi\rangle|
=\left|\int_\Omega(u_m\mathbin\cdot\nabla\Pi_m\varphi)\theta_m\,dx\right|
\leq\|u_m\|_\infty\|\theta_m\|_2\|\varphi\|_{H^1}.
$$

The [sobolev embedding theorem](../../../sobolev-space.md#sobolev-embedding-theorem) and the [periodic elliptic estimate](../../../sobolev-space.md#periodic-elliptic-estimate) for the Stokes operator bound $\|u_m\|_\infty$ by $C|Au_m|$. Moreover,

$$
\|\Delta\theta_m\|_{H^{-1}}\leq\|\nabla\theta_m\|_2,
\qquad
\|\Pi_m(u_m\mathbin\cdot e_3)\|_{H^{-1}}\leq C|u_m|.
$$

The already obtained bounds therefore imply

$$
\boxed{\left\|\frac{d\theta_m}{dt}\right\|_{L^2(0,T;H^{-1}_{\rm per})}\leq K'_0(T)}
$$

with $K'_0(T)$ independent of $m$.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/i">i</h4>

↑ **Parent:** [C](#1/c)

<h5 id="1/c/i/solution">Solution</h5>

↑ **Parent:** [I](#1/c/i)

The uniform bounds and the [Banach-Alaoglu theorem](../../../functional-analysis.md#banach-alaoglu-theorem) provide a subsequence, not relabelled, and a function $\theta$ such that

$$
\theta_m\rightharpoonup^\ast\theta
\quad\hbox{in }L^\infty(0,T;L^2_{\rm per}),
\qquad
\theta_m\rightharpoonup\theta
\quad\hbox{in }L^2(0,T;H^1_{\rm per}),
$$

and

$$
\partial_t\theta_m\rightharpoonup\partial_t\theta
\quad\hbox{in }L^2(0,T;H^{-1}_{\rm per}).
$$

Since $H^1_{\rm per}$ embeds compactly into $L^2_{\rm per}$, the [Aubin-Lions lemma](../../../partial-differential-equation.md#aubin-lions-lemma) strengthens the first convergence to

$$
\boxed{\theta_m\longrightarrow\theta
\quad\hbox{strongly in }L^2(0,T;L^2_{\rm per})}.
$$

The [weak continuity from evolution-space bounds](../../../partial-differential-equation.md#weak-continuity-from-evolution-space-bounds) gives a representative

$$
\boxed{\theta\in C([0,T];L^2_{\rm weak})
\cap L^\infty(0,T;L^2_{\rm per})
\cap L^2(0,T;H^1_{\rm per}),\qquad
\partial_t\theta\in L^2(0,T;H^{-1}_{\rm per})}.
$$

Testing against fixed spatial modes and using $\theta_m(0)=\Pi_m\theta_0$ shows that this representative satisfies $\theta(0)=\theta_0$ weakly.

<h4 id="1/c/ii">ii</h4>

↑ **Parent:** [C](#1/c)

<h5 id="1/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/c/ii)

Define

$$
u=\frac{\alpha}{\nu}A^{-1}P_\sigma(\theta e_3).
$$

The first equation and the bounded inverse of the [Stokes operator](../../../viscous-fluid-flow.md#stokes-operator) show that $u\in L^\infty(0,T;D(A))$ and that

$$
\nu Au=\alpha P_\sigma(\theta e_3)
$$

in $L^\infty(0,T;H)$. In fact, the strong convergence from part (i) and convergence of the spectral projections imply

$$
u_m\longrightarrow u
\quad\hbox{strongly in }L^2(0,T;D(A)).
$$

In three dimensions $D(A)\subset H^2\hookrightarrow L^\infty$, so $u_m\theta_m\to u\theta$ in $L^1(0,T;L^2)$. Because $\nabla\mathbin\cdot u_m=0$,

$$
(u_m\mathbin\cdot\nabla)\theta_m
=\nabla\mathbin\cdot(u_m\theta_m),
$$

and the nonlinear term consequently converges in distributions and in the required weak $L^2(0,T;H^{-1}_{\rm per})$ sense. The linear terms pass by weak convergence, while $\Pi_m$ tends strongly to the identity. Hence

$$
\partial_t\theta-\kappa\Delta\theta
+(u\mathbin\cdot\nabla)\theta
=\beta(u\mathbin\cdot e_3)
$$

in $L^2(0,T;H^{-1}_{\rm per})$. Together with part (i), this proves existence of a global [weak solution](../../../partial-differential-equation.md#weak-solution) of the [Rayleigh-Bénard convection](../../../viscous-fluid-flow.md#rayleigh-benard-convection) system on every finite interval.

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

Let $(u_1,\theta_1)$ and $(u_2,\theta_2)$ be two weak solutions with the same initial data, and set $U=u_1-u_2$ and $\Theta=\theta_1-\theta_2$. The diagnostic Stokes equation gives

$$
|AU|\leq\frac{\alpha}{\nu}\|\Theta\|_2,
\qquad
\|U\|_\infty\leq C\|\Theta\|_2.
$$

Subtracting the temperature equations yields

$$
\partial_t\Theta-\kappa\Delta\Theta
+(u_1\mathbin\cdot\nabla)\Theta
+(U\mathbin\cdot\nabla)\theta_2
=\beta U\mathbin\cdot e_3.
$$

Pair this equation with $\Theta$. The term transported by $u_1$ vanishes by the [skew-symmetry of incompressible transport](../../../viscous-fluid-flow.md#skew-symmetry-of-incompressible-transport), while the other nonlinear term satisfies

$$
\left|\int_\Omega(U\mathbin\cdot\nabla\theta_2)\Theta\,dx\right|
\leq C\|\nabla\theta_2\|_2\|\Theta\|_2^2.
$$

The forcing difference is at most $C\|\Theta\|_2^2$. Consequently

$$
\frac d{dt}\|\Theta\|_2^2
\leq C\bigl(1+\|\nabla\theta_2\|_2\bigr)\|\Theta\|_2^2.
$$

The coefficient is integrable on $[0,T]$ because $\theta_2\in L^2(0,T;H^1)$. Since $\Theta(0)=0$, the [Gronwall inequality](../../../probability-and-statistics.md#gronwall-inequality) gives $\Theta=0$, and the Stokes equation then gives $U=0$. The weak solution is unique.

<h3 id="1/e">e</h3>

↑ **Parent:** [1](#1)

<h4 id="1/e/solution">Solution</h4>

↑ **Parent:** [E](#1/e)

Part (c)(i) already gives weak continuity of $t\mapsto\theta(t)$ in $L^2$. In the assumed energy equality, the dissipation integral

$$
t\longmapsto\int_0^t\|\nabla\theta(\tau)\|_2^2\,d\tau
$$

is absolutely continuous. The forcing integrand is in $L^1(0,T)$ because $u\in L^\infty(0,T;L^2)$ and $\theta\in L^\infty(0,T;L^2)$. The equality therefore makes $t\mapsto\|\theta(t)\|_2^2$ continuous.

Whenever $t_n\to t$, weak continuity gives $\theta(t_n)\rightharpoonup\theta(t)$ and the energy equality gives convergence of their norms. The [Radon-Riesz theorem](../../../hilbert-space.md#radon-riesz-theorem), or directly the [strong continuity from weak continuity and an energy equality](../../../partial-differential-equation.md#strong-continuity-from-weak-continuity-and-an-energy-equality), now gives $\theta(t_n)\to\theta(t)$ in $L^2$. Thus

$$
\boxed{\theta\in C([0,T];L^2_{\rm per}(\Omega))}.
$$

## 2

↑ **Parent:** [Paper 359](paper-359.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/i">i</h4>

↑ **Parent:** [A](#2/a)

<h5 id="2/a/i/solution">Solution</h5>

↑ **Parent:** [I](#2/a/i)

Take the $L^2$ inner product of the first Galerkin equation with $\omega_m$. The [orthogonal projection](../../../hilbert-space.md#orthogonal-projection) may be removed against $\omega_m\in\widetilde H_m$, and [skew-symmetry of incompressible transport](../../../viscous-fluid-flow.md#skew-symmetry-of-incompressible-transport) cancels the nonlinear term. Hence

$$
\nu\|\nabla\omega_m\|_2^2+\gamma\|\omega_m\|_2^2
=(g,\omega_m).
$$

The [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) and [Young inequality](../../../nonlinear-analysis.md#young-s-inequality-for-products) give

$$
\nu\|\nabla\omega_m\|_2^2+\frac{\gamma}{2}\|\omega_m\|_2^2
\leq\frac1{2\gamma}\|g\|_2^2.
$$

Thus both quantities requested in the first estimate are bounded by, for example,

$$
\boxed{R_1^2=\frac{\|g\|_2^2}{\gamma}}.
$$

Next take the inner product with $-\Delta\omega_m$. Periodicity and incompressibility give

$$
\begin{aligned}
\left|((u_m\mathbin\cdot\nabla)\omega_m,-\Delta\omega_m)\right|
&=\left|\int_\Omega\partial_j(u_m)_i\,\partial_i\omega_m\,\partial_j\omega_m\,dx\right|\\
&\leq \|\nabla u_m\|_2\|\nabla\omega_m\|_4^2.
\end{aligned}
$$

The given curl identity and the two-dimensional [Gagliardo-Nirenberg inequality](../../../sobolev-space.md#gagliardo-nirenberg-interpolation-inequality) imply

$$
\|\nabla u_m\|_2\leq C\|\omega_m\|_2,
\qquad
\|\nabla\omega_m\|_4^2
\leq C\|\nabla\omega_m\|_2\|\Delta\omega_m\|_2.
$$

Applying Young's inequality to this term and to $(g,-\Delta\omega_m)$ yields

$$
\frac{\nu}{2}\|\Delta\omega_m\|_2^2
+\gamma\|\nabla\omega_m\|_2^2
\leq\frac{C}{\nu}
\left(\|g\|_2^2+\|\omega_m\|_2^2\|\nabla\omega_m\|_2^2\right).
$$

The first estimate bounds the right-hand side independently of $m$. Therefore one may choose a constant $R_2=R_2(\|g\|_2,\gamma,\nu,\mu_1)$ such that

$$
\boxed{\nu\|\Delta\omega_m\|_2^2\leq R_2^2,
\qquad
\gamma\|\nabla\omega_m\|_2^2\leq R_2^2}.
$$

<h4 id="2/a/ii">ii</h4>

↑ **Parent:** [A](#2/a)

<h5 id="2/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/a/ii)

Use on $\widetilde H_m$ the inner product $(w,z)_1=(\nabla w,\nabla z)$. The map $F_m$ in the hint is continuous because it is a finite-dimensional polynomial map. Since the velocity $v=\nabla^\perp\Phi$ is divergence-free,

$$
\begin{aligned}
\nu(F_m(w),w)_1
&=-\nu\|\nabla w\|_2^2-\gamma\|w\|_2^2
-((v\mathbin\cdot\nabla)w,w)+(g,w)\\
&=-\nu\|\nabla w\|_2^2-\gamma\|w\|_2^2+(g,w).
\end{aligned}
$$

The [Poincaré inequality](../../../sobolev-space.md#poincare-inequality) bounds $\|w\|_2\leq\mu_1^{-1/2}\|\nabla w\|_2$. Thus $(F_m(w),w)_1<0$ on every $H^1$ sphere whose radius is larger than $\|g\|_2/(\nu\sqrt{\mu_1})$. The [Brouwer inward-pointing zero lemma](../../../topological-analysis.md#brouwer-inward-pointing-zero-lemma) supplies $w_\ast$ inside that sphere with $F_m(w_\ast)=0$.

Set $\omega_m=w_\ast$, solve $-\Delta\Psi_m=\omega_m$ in $\widetilde H_m$, and put $u_m=\nabla^\perp\Psi_m$. Expanding $F_m(w_\ast)=0$ gives exactly the first equation of the Galerkin system, so $(\omega_m,\Psi_m,u_m)$ is a solution.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/i">i</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/i/solution">Solution</h5>

↑ **Parent:** [I](#2/b/i)

The second estimate in part (a) bounds $(\omega_m)$ in $H^2_{\rm per}$. The periodic [Poisson equation](../../../partial-differential-equation.md#poisson-equation) $-\Delta\Psi_m=\omega_m$ and the supplied curl identity then bound $(\Psi_m)$ in $H^4_{\rm per}$ and $(u_m)$ in $H^3_{\rm per}$. After passing to a subsequence,

$$
\omega_m\rightharpoonup\omega\ \hbox{in }H^2,
\qquad
\Psi_m\rightharpoonup\Psi\ \hbox{in }H^4,
\qquad
u_m\rightharpoonup u\ \hbox{in }H^3.
$$

The [Rellich-Kondrachov compactness theorem](../../../sobolev-space.md#rellich-kondrachov-theorem) also gives strong convergence in the corresponding spaces with one fewer derivative. In particular, $u_m\to u$ in $L^\infty$ and $\nabla\omega_m\to\nabla\omega$ in $L^2$, so

$$
(u_m\mathbin\cdot\nabla)\omega_m
\longrightarrow(u\mathbin\cdot\nabla)\omega
\quad\hbox{in }L^2.
$$

Passing to the limit in the Galerkin equations gives

$$
-\nu\Delta\omega+\gamma\omega+(u\mathbin\cdot\nabla)\omega=g,
\qquad
u=\nabla^\perp\Psi,
\qquad
-\Delta\Psi=\omega.
$$

These identities have the claimed [Sobolev regularity](../../../sobolev-space.md), and the first holds in $L^2_{\rm per}$. Finally, the [weak lower semicontinuity of the Hilbert norm](../../../hilbert-space.md#weak-lower-semicontinuity-of-the-hilbert-norm) preserves the estimates

$$
\boxed{\nu\|\Delta\omega\|_2^2\leq R_2^2,
\qquad
\gamma\|\nabla\omega\|_2^2\leq R_2^2}.
$$

<h4 id="2/b/ii">ii</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/b/ii)

The regularity from part (i) makes $u\omega$ and its first weak derivatives square-integrable. The [product rule](../../../calculus.md#product-rule) therefore holds in the [distributional derivative](../../../distribution-theory.md#distributional-derivative) sense:

$$
\nabla\mathbin\cdot(u\omega)
=(\nabla\mathbin\cdot u)\omega+u\mathbin\cdot\nabla\omega.
$$

Since $u=\nabla^\perp\Psi$, equality of mixed weak derivatives gives $\nabla\mathbin\cdot u=0$. Both remaining expressions belong to $L^2_{\rm per}$, so their distributional equality is an equality in that space:

$$
\boxed{u\mathbin\cdot\nabla\omega=\nabla\mathbin\cdot(u\omega)}.
$$

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Let $q=2p+2$ and multiply the vorticity equation by $\omega^{q-1}$, first for an odd power as in the hint. Periodic [integration by parts](../../../calculus.md#integration-by-parts) and $\nabla\mathbin\cdot u=0$ give

$$
\nu(q-1)\int_\Omega\omega^{q-2}|\nabla\omega|^2\,dx
+\gamma\|\omega\|_q^q
=\int_\Omega g\omega^{q-1}\,dx.
$$

The diffusion term is nonnegative, while the [Holder inequality](../../../functional-analysis.md#holder-inequality) bounds the right-hand side by $\|g\|_q\|\omega\|_q^{q-1}$. Consequently

$$
\gamma\|\omega\|_q\leq\|g\|_q.
$$

On the finite-volume torus, $L^q$ norms increase to the [essential supremum](../../../measure-theory.md#essential-supremum) as $q\to\infty$. Hence the [damped-vorticity maximum estimate](../../../viscous-fluid-flow.md#damped-vorticity-maximum-estimate) gives

$$
\boxed{\gamma\|\omega\|_\infty\leq\|g\|_\infty}.
$$

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

For each $\nu>0$, choose the solution from parts (a)--(c). The maximum estimate gives a $\nu$-independent bound

$$
\|\omega_\nu\|_\infty\leq\gamma^{-1}\|g\|_\infty.
$$

Thus a sequence $\nu_j\downarrow0$ has $\omega_{\nu_j}\rightharpoonup^\ast\omega$ in $L^\infty$. The periodic elliptic estimates for

$$
-\Delta\Psi_{\nu_j}=\omega_{\nu_j},
\qquad
u_{\nu_j}=\nabla^\perp\Psi_{\nu_j}
$$

bound $\Psi_{\nu_j}$ in $W^{2,p}$ and $u_{\nu_j}$ in $W^{1,p}$ for every finite $p$. Taking $p>2$ and using compact [Sobolev embedding](../../../sobolev-space.md#failure-of-first-order-sobolev-embedding-into-linfinity-in-two-dimensions) gives, after a further subsequence, uniform convergence $u_{\nu_j}\to u$. It follows that $u_{\nu_j}\omega_{\nu_j}\rightharpoonup u\omega$ distributionally.

The first energy estimate gives

$$
\|\nu_j\nabla\omega_{\nu_j}\|_2
\leq\sqrt{\nu_j}\,R_1\longrightarrow0.
$$

Therefore the viscous term vanishes in $H^{-1}$, and the weak formulation passes to the limit as

$$
\boxed{\gamma\omega+\nabla\mathbin\cdot(u\omega)=g}.
$$

The elliptic relations pass to the limit as well and give

$$
u=\nabla^\perp\Psi,\qquad-\Delta\Psi=\omega.
$$

Since $\omega\in L^\infty\subset L^2$, periodic elliptic regularity gives $\Psi\in H^2_{\rm per}$ and $u\in H^1_{\rm per}\cap H$. Moreover $u\omega\in L^2$, so its divergence lies in $H^{-1}_{\rm per}$. This constructs the required weak solution of the damped-driven Euler system by a [vanishing-viscosity limit](../../../viscous-fluid-flow.md#vanishing-viscosity-limit).

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2026](../../2026.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
