# Paper 344

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2021/paper_344.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2021/paper_344.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
  - [d](#1/d)
    - [Solution](#1/d/solution)
  - [e](#1/e)
    - [Solution](#1/e/solution)
  - [f](#1/f)
    - [Solution](#1/f/solution)
  - [g](#1/g)
    - [Solution](#1/g/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
  - [d](#2/d)
    - [Solution](#2/d/solution)
  - [e](#2/e)
    - [Solution](#2/e/solution)
  - [f](#2/f)
    - [Solution](#2/f/solution)
  - [g](#2/g)
    - [Solution](#2/g/solution)
  - [h](#2/h)
    - [Solution](#2/h/solution)
- [3](#3)
  - [a](#3/a)
    - [i](#3/a/i)
      - [Solution](#3/a/i/solution)
    - [ii](#3/a/ii)
      - [Solution](#3/a/ii/solution)
    - [iii](#3/a/iii)
      - [Solution](#3/a/iii/solution)
  - [b](#3/b)
    - [i](#3/b/i)
      - [Solution](#3/b/i/solution)
    - [ii](#3/b/ii)
      - [Solution](#3/b/ii/solution)
  - [c](#3/c)
    - [i](#3/c/i)
      - [Solution](#3/c/i/solution)
    - [ii](#3/c/ii)
      - [Solution](#3/c/ii/solution)
    - [iii](#3/c/iii)
      - [Solution](#3/c/iii/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [Solution](#4/c/solution)
  - [d](#4/d)
    - [Solution](#4/d/solution)
  - [e](#4/e)
    - [Solution](#4/e/solution)

## 1

↑ **Parent:** [Paper 344](paper-344.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Impose the fixed [conserved order parameter](../../../critical-phenomenon.md#conserved-order-parameter)

$$
\int\phi\,d\mathbf r=\Phi
$$

with a [Lagrange multiplier](../../../mathematical-optimization.md#lagrange-multiplier) $\mu_0$. Stationarity of

$$
\mathcal F[\phi]-\mu_0\int\phi\,d\mathbf r
$$

under every local variation gives

$$
\frac{\delta\mathcal F}{\delta\phi(\mathbf r)}
=\mu(\mathbf r)=\mu_0.
$$

**Thus the [chemical potential](../../../thermodynamics.md#chemical-potential) is spatially constant at constrained equilibrium.**

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

For constant $\kappa$ and a planar profile,

$$
\mu=f'(\phi)-\kappa\phi''
=a\phi+b\phi^3-\kappa\phi''.
$$

Far inside either bulk phase, derivatives vanish and $\phi=\pm\phi_B$, where $\phi_B^2=-a/b$. Therefore

$$
\mu=a(\pm\phi_B)+b(\pm\phi_B)^3=0.
$$

Since part a makes $\mu$ constant, it vanishes throughout the interface.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

The Euler–Lagrange equation is $\kappa\phi''=a\phi+b\phi^3$. Multiplication by $\phi'$ and integration gives the first integral

$$
\frac\kappa2(\phi')^2=f(\phi)-f(\phi_B).
$$

With $\phi=\phi_Bg$, $u=x/\xi_0$, and $\xi_0^2=-2\kappa/a$, this becomes

$$
\boxed{2g^2-g^4+(g')^2=1}.
$$

The monotone heteroclinic solutions are

$$
\boxed{
\phi(x)=\pm\phi_B
\tanh\left(\frac{x-x_0}{\xi_0}\right)
}.
$$

[Translation invariance](../../../physics.md#translation-invariance) leaves $x_0$ undetermined in an infinite system. A fixed global composition, boundary condition, or pinning field fixes this midpoint position.

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

For

$$
\mathcal F=\int\left[
f(\phi)+\frac{\kappa(\phi)}2|\nabla\phi|^2
\right]d\mathbf r,
$$

the [functional derivative](../../../calculus-of-variations.md#functional-derivative) is

$$
\boxed{
\mu=f'(\phi)-\nabla\mathbin{\cdot}
[\kappa(\phi)\nabla\phi]
+\frac{\kappa'(\phi)}2|\nabla\phi|^2
=f'(\phi)-\kappa(\phi)\nabla^2\phi
-\frac{\kappa'(\phi)}2|\nabla\phi|^2
}.
$$

The constrained minimum again makes $\mu$ constant. Evaluating it in either uniform bulk phase gives $\mu=f'(\pm\phi_B)=0$, so $\mu=0$ everywhere.

<h3 id="1/e">e</h3>

↑ **Parent:** [1](#1)

<h4 id="1/e/solution">Solution</h4>

↑ **Parent:** [E](#1/e)

For a planar equilibrium, multiply $\mu=0$ by $\phi'$ and use the [chain rule](../../../calculus.md#chain-rule). The result is

$$
\frac d{dx}\left[
f(\phi)-\frac{\kappa(\phi)}2(\phi')^2
\right]=0.
$$

Matching to either bulk phase fixes the constant:

$$
\boxed{
f(\phi)-\frac{\kappa(\phi)}2(\phi')^2=f(\phi_B)
}.
$$

Consequently

$$
\frac{dx}{d\phi}
=\pm\sqrt{\frac{\kappa(\phi)}
{2[f(\phi)-f(\phi_B)]}},
$$

and the inverse profile is

$$
\boxed{
x(\phi)-x_0
=\pm\int_0^\phi
\sqrt{\frac{\kappa(\psi)}
{2[f(\psi)-f(\phi_B)]}}\,d\psi
}.
$$

<h3 id="1/f">f</h3>

↑ **Parent:** [1](#1)

<h4 id="1/f/solution">Solution</h4>

↑ **Parent:** [F](#1/f)

The [interfacial tension](../../../critical-phenomenon.md#interfacial-tension) is the excess free energy per unit interfacial area:

$$
\sigma=\int_{-\infty}^{\infty}
\left[
f(\phi)-f(\phi_B)
+\frac{\kappa(\phi)}2(\phi')^2
\right]dx.
$$

The first integral from part e equates the first two terms inside the brackets to $\kappa(\phi)(\phi')^2/2$. Hence

$$
\boxed{
\sigma=\int_{-\infty}^{\infty}
\kappa(\phi)(\partial_x\phi)^2\,dx
}.
$$

<h3 id="1/g">g</h3>

↑ **Parent:** [1](#1)

<h4 id="1/g/solution">Solution</h4>

↑ **Parent:** [G](#1/g)

For the quartic free energy,

$$
f(\phi)-f(\phi_B)
=\frac b4(\phi^2-\phi_B^2)^2.
$$

With constant $\kappa$, part e gives, between the two bulk values,

$$
\frac{dx}{d\phi}
=\pm\frac{\sqrt{2\kappa/b}}
{\phi_B^2-\phi^2}.
$$

Integration gives

$$
x-x_0
=\pm\frac{\sqrt{2\kappa/b}}{\phi_B}
\operatorname{artanh}\frac{\phi}{\phi_B}
=\pm\xi_0\operatorname{artanh}\frac{\phi}{\phi_B},
$$

whose inversion is exactly the hyperbolic-tangent profile in part c.

## 2

↑ **Parent:** [Paper 344](paper-344.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

For a uniform field the gradient term vanishes and minimization over $p=|\mathbf p|$ gives

$$
ap+bp^3=0.
$$

When $a<0$, the nonzero minimum has

$$
\boxed{p_0=\sqrt{-a/b}},
$$

while its direction is arbitrary by [rotational symmetry](../../../linear-algebra.md#rotational-symmetry). A sudden [quench](../../../critical-phenomenon.md#quench-statistical-physics) creates many independently oriented domains. Their mismatches contain gradients and [topological defects](../../../critical-phenomenon.md#topological-defect), whose motion and pair annihilation are slow, so the uniform state is not reached promptly.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Outside a defect core write

$$
\mathbf p=p_0(\cos\theta,\sin\theta).
$$

Around any closed curve on which $\mathbf p\ne0$, its [topological charge](../../../classical-field-theory-soliton.md#topological-charge) is the [winding number](../../../complex-analysis.md#winding-number)

$$
\boxed{
q=\frac1{2\pi}\oint d\theta
}.
$$

Single-valued polar order requires $q\in\mathbb Z$. A nonzero value prevents the field inside the loop from being continuously deformed to a uniform nonvanishing field, so the core must contain a zero or singularity.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

In polar coordinates $(r,\varphi)$, a radial aster

$$
\theta=\varphi
$$

and a circulating vortex

$$
\theta=\varphi+\frac\pi2
$$

both have $q=+1$. The continuous family $\theta=\varphi+\chi$, $0\leq\chi\leq\pi/2$, deforms one into the other without making $\mathbf p$ vanish away from the core, proving their topological equivalence. The hyperbolic configuration $\theta=-\varphi$ has $q=-1$.

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

The field $\mathbf p=-p(r)\widehat{\mathbf r}$ has angle $\theta=\varphi+\pi$. Its defect is at $r=0$ and has $q=+1$. Since

$$
\partial_r\mathbf p=-p'\widehat{\mathbf r},
\qquad
\frac1r\partial_\varphi\mathbf p
=-\frac p r\widehat{\boldsymbol\varphi},
$$

one has

$$
(\partial_i p_j)(\partial_i p_j)
=(p')^2+\frac{p^2}{r^2}.
$$

The local free-energy density is therefore

$$
\boxed{
\mathcal F
=\frac a2p^2+\frac b4p^4
+\frac\kappa2\left[
\left(\frac{dp}{dr}\right)^2+\left(\frac p r\right)^2
\right]
}.
$$

<h3 id="2/e">e</h3>

↑ **Parent:** [2](#2)

<h4 id="2/e/solution">Solution</h4>

↑ **Parent:** [E](#2/e)

Outside the core, put $p=p_0$. The angular-gradient contribution is

$$
F_{\mathrm{el}}
=\int_{r_0}^L2\pi r\,dr\,
\frac\kappa2\frac{p_0^2}{r^2}
=\boxed{
\pi\kappa p_0^2\log\frac L{r_0}
}.
$$

The omitted core contribution is finite and independent of $L$.

<h3 id="2/f">f</h3>

↑ **Parent:** [2](#2)

<h4 id="2/f/solution">Solution</h4>

↑ **Parent:** [F](#2/f)

A defect of charge $q$ has far-field elastic energy proportional to $q^2\log(L/r_0)$. Splitting $q$ into allowed charges $q_i$ with $\sum q_i=q$ lowers $\sum q_i^2$ unless the pieces already have the smallest permitted magnitude. Polar order distinguishes $\mathbf p$ from $-\mathbf p$, so its smallest nonzero charge is $|q|=1$. A [nematic liquid crystal](../../../critical-phenomenon.md#nematic-liquid-crystal) identifies $\widehat{\mathbf n}\sim-\widehat{\mathbf n}$; a rotation by only $\pi$ closes a loop in its order-parameter space, permitting $q=\pm1/2$.

<h3 id="2/g">g</h3>

↑ **Parent:** [2](#2)

<h4 id="2/g/solution">Solution</h4>

↑ **Parent:** [G](#2/g)

Let $\chi$ be the angle between $\widehat{\mathbf p}$ and $\widehat{\mathbf n}$. Then

$$
p_iQ_{ij}p_j
=\lambda p^2(2\cos^2\chi-1)
=\lambda p^2\cos2\chi.
$$

For $\zeta,\lambda>0$, the coupling $-\zeta\lambda p^2\cos2\chi/2$ is minimized by $\cos2\chi=1$, so

$$
\boxed{\widehat{\mathbf p}=\pm\widehat{\mathbf n}}.
$$

The uniform terms depending on $p$ reduce to

$$
\frac12(a-\zeta\lambda)p^2+\frac b4p^4.
$$

Their nonzero minimum is

$$
\boxed{p^2=-\frac{a-\zeta\lambda}{b}}.
$$

<h3 id="2/h">h</h3>

↑ **Parent:** [2](#2)

<h4 id="2/h/solution">Solution</h4>

↑ **Parent:** [H](#2/h)

An isolated nematic half-defect reverses the representative director after one circuit. Alignment would then reverse the polar vector, which is not the same physical state. Half-integer defects can therefore occur only if accompanied by a branch wall on which polar order rotates sharply or vanishes. The wall has a tension proportional to its length, so half-defects are confined in pairs in the uniformly polar phase; they can deconfine where polar order disappears.

## 3

↑ **Parent:** [Paper 344](paper-344.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/i">i</h4>

↑ **Parent:** [A](#3/a)

<h5 id="3/a/i/solution">Solution</h5>

↑ **Parent:** [I](#3/a/i)

Under the [Euclidean isometry](../../../riemannian-geometry.md#euclidean-isometry) $\widetilde{\mathbf r}=\mathbf a+R\mathbf r$, where $R^TR=I$,

$$
\partial_u\widetilde{\mathbf r}=R\partial_u\mathbf r.
$$

Therefore

$$
\widetilde g
=(R\mathbf r_u)\mathbin{\cdot}(R\mathbf r_u)
=\mathbf r_u\mathbin{\cdot}\mathbf r_u=g.
$$

Since the integration parameter is unchanged,

$$
\widetilde S(u)=\int_0^u\sqrt{\widetilde g(u')}\,du'
=S(u).
$$

Both the [induced metric](../../../riemannian-geometry.md#induced-metric) and [arc length](../../../riemannian-geometry.md#arc-length) are invariant.

<h4 id="3/a/ii">ii</h4>

↑ **Parent:** [A](#3/a)

<h5 id="3/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/a/ii)

For an oriented planar curve, the [Frenet-Serret formulas](../../../differential-geometry.md#frenet-serret-formulas) are

$$
\partial_s
\begin{pmatrix}\mathbf t\\\mathbf n\end{pmatrix}
=
\begin{pmatrix}0&k\\-k&0\end{pmatrix}
\begin{pmatrix}\mathbf t\\\mathbf n\end{pmatrix}.
$$

The frame is orthonormal, so differentiating each scalar product gives

$$
\partial_s(\mathbf e_i\mathbin{\cdot}\mathbf e_j)=0.
$$

In matrix form this says that the connection matrix plus its transpose is zero; it must be antisymmetric.

<h4 id="3/a/iii">iii</h4>

↑ **Parent:** [A](#3/a)

<h5 id="3/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#3/a/iii)

The signed [curvature](../../../differential-geometry.md#curvature) is

$$
k=\mathbf n\mathbin{\cdot}\partial_s\mathbf t.
$$

An orientation-preserving isometry sends $\mathbf t,\mathbf n$ to $R\mathbf t,R\mathbf n$ and leaves $s$ unchanged, so

$$
\widetilde k=(R\mathbf n)\mathbin{\cdot}
R(\partial_s\mathbf t)=k.
$$

An orientation-reversing isometry reverses the chosen normal and hence the sign convention for signed curvature, while the geometric curvature $|k|$ remains invariant.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/i">i</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/i/solution">Solution</h5>

↑ **Parent:** [I](#3/b/i)

Because $\partial_u=\sqrt g\,\partial_s$ and $\mathbf r_t=U\mathbf n+W\mathbf t$, commuting $\partial_t$ and $\partial_u$ gives

$$
\partial_t\mathbf t=(\partial_sU+kW)\mathbf n.
$$

Preservation of orthonormality then gives

$$
\boxed{
\partial_t
\begin{pmatrix}\mathbf t\\\mathbf n\end{pmatrix}
=
\begin{pmatrix}
0&\partial_sU+kW\\
-\partial_sU-kW&0
\end{pmatrix}
\begin{pmatrix}\mathbf t\\\mathbf n\end{pmatrix}
}.
$$

The tangential derivative of the velocity is

$$
\partial_s\mathbf r_t
=(\partial_sW-kU)\mathbf t
+(\partial_sU+kW)\mathbf n,
$$

so

$$
\boxed{\partial_tg=2g(\partial_sW-kU)}.
$$

Finally commute the $s$ and $t$ derivatives in $\partial_s\mathbf t=k\mathbf n$, accounting for the evolving metric through

$$
[\partial_t,\partial_s]
=-(\partial_sW-kU)\partial_s.
$$

The normal component gives

$$
\boxed{
\partial_tk=(\partial_s^2+k^2)U+W\partial_sk
}.
$$

<h4 id="3/b/ii">ii</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/b/ii)

Since $\partial_t\sqrt g=\sqrt g(\partial_sW-kU)$,

$$
\partial_tS(u,t)
=\int_0^u\sqrt g(\partial_sW-kU)\,du'
=\int_0^{S(u,t)}(\partial_sW-kU)\,ds.
$$

Thus

$$
\boxed{
\partial_tS
=W(S,t)-W(0,t)-\int_0^S kU\,ds
}.
$$

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/i">i</h4>

↑ **Parent:** [C](#3/c)

<h5 id="3/c/i/solution">Solution</h5>

↑ **Parent:** [I](#3/c/i)

Local [force balance](../../../classical-mechanics.md#force-balance) and [moment balance](../../../classical-mechanics.md#moment-balance) on a slender rod are

$$
\boxed{
\partial_s\mathbf F+\mathbf f=0,
\qquad
\partial_s\mathbf M+\mathbf t\times\mathbf F+\mathbf m=0
}.
$$

In a planar rod, $\mathbf M$ and $\mathbf m$ point perpendicular to the plane.

<h4 id="3/c/ii">ii</h4>

↑ **Parent:** [C](#3/c)

<h5 id="3/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/c/ii)

Substitute

$$
\mathbf f=-\boldsymbol\gamma\mathbin{\cdot}\mathbf r_t
+\mathbf f^A
$$

into force balance. With $\boldsymbol\mu=\boldsymbol\gamma^{-1}$,

$$
\mathbf r_t
=\boldsymbol\mu\mathbin{\cdot}
(\partial_s\mathbf F+\mathbf f^A).
$$

Projection onto the local frame gives

$$
\boxed{
W=\mathbf t\mathbin{\cdot}\boldsymbol\mu
(\partial_s\mathbf F+\mathbf f^A),
\qquad
U=\mathbf n\mathbin{\cdot}\boldsymbol\mu
(\partial_s\mathbf F+\mathbf f^A)
}.
$$

<h4 id="3/c/iii">iii</h4>

↑ **Parent:** [C](#3/c)

<h5 id="3/c/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#3/c/iii)

Resolve

$$
\mathbf F=F_\parallel\mathbf t+F_\perp\mathbf n.
$$

The [Frenet-Serret formulas](../../../differential-geometry.md#frenet-serret-formulas) give

$$
\partial_s\mathbf F
=(\partial_sF_\parallel-kF_\perp)\mathbf t
+(\partial_sF_\perp+kF_\parallel)\mathbf n.
$$

Using

$$
\boldsymbol\mu
=\mu_\parallel\mathbf t\mathbf t
+\mu_\perp\mathbf n\mathbf n,
\qquad
\mathbf f^A=f_\parallel^A\mathbf t+f_\perp^A\mathbf n,
$$

therefore yields

$$
\boxed{
W=\mu_\parallel
(\partial_sF_\parallel-kF_\perp+f_\parallel^A)
},
$$



$$
\boxed{
U=\mu_\perp
(\partial_sF_\perp+kF_\parallel+f_\perp^A)
}.
$$

## 4

↑ **Parent:** [Paper 344](paper-344.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

For $\alpha>0$, variation of constants gives the stationary [Ornstein-Uhlenbeck process](../../../stochastic-process.md#ornstein-uhlenbeck-process)

$$
f(t)=c\int_{-\infty}^t
\Lambda_f(s)e^{-\alpha(t-s)}\,ds.
$$

For $t\geq t'$ its covariance is

$$
\begin{aligned}
\langle f(t)f(t')\rangle
&=c^2\int_{-\infty}^{t'}
e^{-\alpha(t-s)}e^{-\alpha(t'-s)}\,ds\\
&=\frac{c^2}{2\alpha}e^{-\alpha(t-t')}.
\end{aligned}
$$

Symmetry in $t,t'$ therefore gives

$$
\boxed{
\langle f(t)f(t')\rangle
=f_0^2e^{-\alpha|t-t'|},
\qquad
f_0^2=\frac{c^2}{2\alpha}
}.
$$

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

The [Fluctuation-dissipation theorem](../../../quantum-field-theory.md#fluctuation-dissipation-theorem) for mobility $\widetilde M$ requires

$$
\dot x=-\widetilde M V'(x)
+\sqrt{2\widetilde M k_BT}\,\Lambda_x.
$$

Comparison with the stated noise amplitude gives

$$
\boxed{C^2=2k_BT}.
$$

This choice makes the stationary [Fokker-Planck equation](../../../probability-theory.md#fokker-planck-equation) have the [Boltzmann distribution](../../../thermodynamics.md#boltzmann-distribution) proportional to $e^{-V/(k_BT)}$.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

Let $\tau=|t-t'|$. Integrating the equation for $x$ and using independence of the two noises gives

$$
R(\tau)
=C^2\tau+
\int_0^\tau\int_0^\tau
f_0^2e^{-\alpha|s-s'|}\,ds\,ds'.
$$

With the supplied integral,

$$
\boxed{
R(\tau)
=C^2\tau+
\frac{2f_0^2}{\alpha^2}
\left(\alpha\tau-1+e^{-\alpha\tau}\right)
}.
$$

For $\alpha\tau\ll1$, the active contribution is ballistic, $f_0^2\tau^2+O(\tau^3)$, in addition to the Brownian term. For $\alpha\tau\gg1$,

$$
R(\tau)
=\left(C^2+\frac{2f_0^2}{\alpha}\right)\tau
-\frac{2f_0^2}{\alpha^2}+o(1),
$$

so the long-time motion is diffusive with an enhanced [diffusion coefficient](../../../brownian-motion.md#diffusion-coefficient).

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

Conditioned on $f$, the additive-noise trajectory has the [Onsager–Machlup functional](../../../critical-phenomenon.md#onsager-machlup-functional)

$$
P[x\mid f]\propto
\exp\left[
-\frac1{2C^2}\int_0^T
(\dot x+V'(x)-f)^2dt
\right].
$$

Under time reversal, $\dot x$ changes sign while $x$ and the active force $f$ are even. Subtracting the forward and backward conditional actions gives

$$
\log\frac{P_F[x\mid f]}{P_B[x\mid f]}
=\frac2{C^2}\left[
V(x_0)-V(x_T)
+\int_0^T\dot x\,f\,dt
\right].
$$

The corresponding ratio for an Ornstein–Uhlenbeck path conditioned on its initial endpoint is

$$
\log\frac{P_F[f]}{P_B[f]}
=\frac{\alpha}{c^2}
\left[f(0)^2-f(T)^2\right].
$$

Consequently

$$
\boxed{
\log\frac{P_F[f,x]}{P_B[f,x]}
=\Delta U[f,x]
+\frac2{C^2}\int_0^T\dot x(t)f(t)\,dt
},
$$

where

$$
\boxed{
\Delta U[f,x]
=\frac{\alpha}{c^2}[f(0)^2-f(T)^2]
+\frac2{C^2}[V(x_0)-V(x_T)]
}.
$$

If stationary endpoint densities are included in the path measures, their ratio cancels the Ornstein–Uhlenbeck boundary term; the displayed convention is the endpoint-conditioned path probability used in the calculation.

<h3 id="4/e">e</h3>

↑ **Parent:** [4](#4)

<h4 id="4/e/solution">Solution</h4>

↑ **Parent:** [E](#4/e)

The first part of $\Delta U$ is the change of the quadratic energy associated with the active Ornstein–Uhlenbeck force. The second is minus the change in the particle's potential energy, measured in thermal-noise units. The time integral is the [work](../../../classical-mechanics.md#work) done by active propulsion, again divided by its noise scale; the full log ratio is the trajectory's time-reversal asymmetry or [entropy production](../../../thermodynamics.md#entropy-production).

In a stationary confining state the two endpoint terms remain $O(1)$ as $T\to\infty$ and have zero mean, while the mean active work and the mean log ratio grow proportionally to $T$. Endpoint-term distributions approach time-independent distributions with positive and negative fluctuations. Under mixing assumptions, the time-integrated work has a large-deviation distribution: its central part becomes approximately [Gaussian](../../../probability-theory.md#normal-distribution) with mean and variance proportional to $T$, while its far tails scale exponentially in $T$. The log-ratio distribution obeys the corresponding [fluctuation theorem](../../../thermodynamics.md#fluctuation-theorem) symmetry.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2021](../../2021.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
