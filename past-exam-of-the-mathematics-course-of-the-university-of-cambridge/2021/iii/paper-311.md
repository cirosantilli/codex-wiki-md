# Paper 311

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2021/paper_311.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2021/paper_311.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [i](#1/a/i)
      - [Solution](#1/a/i/solution)
    - [ii](#1/a/ii)
      - [Solution](#1/a/ii/solution)
    - [iii](#1/a/iii)
      - [Solution](#1/a/iii/solution)
    - [iv](#1/a/iv)
      - [Solution](#1/a/iv/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
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
  - [e](#2/e)
    - [Solution](#2/e/solution)
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
    - [i](#4/b/i)
      - [Solution](#4/b/i/solution)
    - [ii](#4/b/ii)
      - [Solution](#4/b/ii/solution)
  - [c](#4/c)
    - [i](#4/c/i)
      - [Solution](#4/c/i/solution)
    - [ii](#4/c/ii)
      - [Solution](#4/c/ii/solution)
    - [iii](#4/c/iii)
      - [Solution](#4/c/iii/solution)
    - [iv](#4/c/iv)
      - [Solution](#4/c/iv/solution)

## 1

↑ **Parent:** [Paper 311](paper-311.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/i">i</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/i/solution">Solution</h5>

↑ **Parent:** [I](#1/a/i)

A [null geodesic congruence](../../../geodesic-congruence.md#null-geodesic-congruence) is a smooth family of nonintersecting null geodesics filling an open spacetime region. For its affinely parametrized tangent $U^a$,

$$
U^aU_a=0,
\qquad
U^b\nabla_bU^a=0.
$$

Writing $B_{ab}=\nabla_bU_a$, differentiation of the null norm and the [geodesic equation](../../../riemannian-geometry.md#geodesic-equation) give respectively

$$
\boxed{U^aB_{ab}=\frac12\nabla_b(U^aU_a)=0,
\qquad
B_{ab}U^b=U^b\nabla_bU_a=0.}
$$

<h4 id="1/a/ii">ii</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/a/ii)

Choose at one transverse cross-section a null vector $N^a$ satisfying $N^aN_a=0$ and $U^aN_a=-1$, then [parallel transport](../../../fiber-bundle.md#parallel-transport) it along every generator:

$$
U^b\nabla_bN^a=0.
$$

Metric compatibility and the affine [geodesic equation](../../../riemannian-geometry.md#geodesic-equation) imply that both $N^2$ and $U\mathbin\cdot N$ are constant along each generator, so the required normalization persists.

<h4 id="1/a/iii">iii</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#1/a/iii)

The [screen-space projector](../../../geodesic-congruence.md#screen-space-projector)

$$
P^a{}_b=\delta^a_b+U^aN_b+N^aU_b
$$

defines the [optical tensor](../../../geodesic-congruence.md#optical-tensor) $\widehat B_{ab}=P_a{}^cP_b{}^dB_{cd}$. In four spacetime dimensions its irreducible decomposition is

$$
\boxed{\theta=P^{ab}\widehat B_{ab},\qquad
\widehat\omega_{ab}=\widehat B_{[ab]},\qquad
\widehat\sigma_{ab}=\widehat B_{(ab)}-\frac12\theta P_{ab}}.
$$

These are the [null expansion](../../../geodesic-congruence.md#null-expansion), [null twist](../../../geodesic-congruence.md#null-twist), and [null shear](../../../geodesic-congruence.md#null-shear).

<h4 id="1/a/iv">iv</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#1/a/iv)

On the [null hypersurface](../../../general-relativity.md#null-hypersurface), the generator covector is proportional to a normal, locally $U_a=f\nabla_a u$ for a level-set function $u$. The [Frobenius theorem](../../../differential-geometry.md#frobenius-theorem) therefore gives

$$
U_{[a}\nabla_bU_{c]}=0.
$$

Contracting once with $N^a$ and projecting the remaining indices with $P^a{}_b$ removes every term containing $U$ or $N$ and leaves $P_b{}^dP_c{}^e\nabla_{[d}U_{e]}=0$. Hence

$$
\boxed{\widehat\omega_{ab}=0}
$$

on the hypersurface.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Commuting [covariant derivatives](../../../general-relativity.md#covariant-derivative) and using $U^b\nabla_bU_a=0$ gives the optical evolution equation

$$
U^c\nabla_cB_{ab}=-B_{ac}B^c{}_b-R_{acbd}U^cU^d.
$$

Taking its screen trace yields

$$
\frac{d\theta}{d\lambda}
=-\widehat B_{ab}\widehat B^{ba}-R_{ab}U^aU^b.
$$

The optical decomposition and the symmetry or antisymmetry of its pieces imply

$$
\widehat B_{ab}\widehat B^{ba}
=\frac12\theta^2+widehat\sigma_{ab}\widehat\sigma^{ab}
-\widehat\omega_{ab}\widehat\omega^{ab}.
$$

Thus the four-dimensional [Null Raychaudhuri equation](../../../geodesic-congruence.md#null-raychaudhuri-equation) is

$$
\boxed{\frac{d\theta}{d\lambda}
=-\frac12\theta^2
-\widehat\sigma_{ab}\widehat\sigma^{ab}
+\widehat\omega_{ab}\widehat\omega^{ab}
-R_{ab}U^aU^b}.
$$

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

The hypersurface generators have zero [null twist](../../../geodesic-congruence.md#null-twist). Contracting the [Einstein field equations](../../../general-relativity.md#einstein-field-equations) twice with the null tangent removes the trace term, and the [null energy condition](../../../general-relativity.md#null-energy-condition) gives $R_{ab}U^aU^b=8\pi T_{ab}U^aU^b\geq0$. Since the squared [null shear](../../../geodesic-congruence.md#null-shear) is nonnegative, the [Null Raychaudhuri equation](../../../geodesic-congruence.md#null-raychaudhuri-equation) implies

$$
\frac{d\theta}{d\lambda}\leq-\frac12\theta^2.
$$

While $\theta<0$ this is equivalent to

$$
\frac{d}{d\lambda}\left(\frac1\theta\right)\geq\frac12.
$$

Starting from $\theta(0)=\theta_0<0$, the right-hand side reaches zero no later than $\lambda=2/|\theta_0|$. The reciprocal expansion must therefore vanish and

$$
\boxed{\theta\longrightarrow-\infty
\quad\text{within affine distance }2/|\theta_0|}.
$$

This is the [null focusing theorem](../../../geodesic-congruence.md#null-focusing-theorem).

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

Suppose the closed [trapped surface](../../../general-relativity.md#trapped-surface) $T$ were not wholly in the [black hole](../../../general-relativity.md#black-hole). The stated consequence of [strong asymptotic predictability](../../../general-relativity.md#strong-asymptotic-predictability) then supplies a point $p\in\dot J^+(T)\cap\mathcal I^+$ lying on a future null generator $\gamma$ orthogonal to $T$, with no point conjugate to $T$ before $p$. Both future null expansions at $T$ are negative. The [null focusing theorem](../../../geodesic-congruence.md#null-focusing-theorem) therefore forces the expansion along $\gamma$ to diverge after finite [affine parameter](../../../riemannian-geometry.md#affine-parameter), producing a [conjugate point](../../../calculus-of-variations.md#conjugate-point) before the generator reaches [future null infinity](../../../general-relativity.md#future-null-infinity). A null geodesic with such a point cannot continue to generate the achronal boundary $\dot J^+(T)$, contradicting the property of $p$. Hence no point of $T$ can communicate with future null infinity, and

$$
\boxed{T\subset B=M\setminus J^-(\mathcal I^+)}.
$$

## 2

↑ **Parent:** [Paper 311](paper-311.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Every metric coefficient is independent of $t$ and $\phi$. The corresponding coordinate flows therefore preserve the metric, so

$$
\boxed{K=\partial_t,\qquad m=\partial_\phi}
$$

satisfy the [Killing equation](../../../general-relativity.md#killing-equation) and are [Killing vector fields](../../../general-relativity.md#killing-vector-field). They generate stationarity and axial symmetry respectively.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Put $\mu=r_+(r_+^2+a^2)$. At large $r$, the one-form dual to $K$ has

$$
K^\flat=g_{tt}\,dt+g_{t\phi}\,d\phi,
\qquad
g_{tt}=-1+\frac{\mu}{r\Sigma}
=-1+\frac{\mu}{r^3}+O(r^{-5}).
$$

Only the $dr\wedge dt$ term contributes to the constant-$t,r$ [Komar integral](../../../general-relativity.md#komar-charge), and

$$
dK^\flat=-\frac{3\mu}{r^4},dr\wedge dt+O(r^{-5}).
$$

With the stated [orientation](../../../algebraic-topology.md#orientation-of-a-simplex), the asymptotic [Hodge star operator](../../../differential-form.md#hodge-star-operator) gives

$$
\star(dr\wedge dt)=r^4\sin\theta\cos^2\theta\sin\lambda\,
d\theta\wedge d\phi\wedge d\lambda\wedge d\psi.
$$

The angular integral is the area of the unit four-sphere,

$$
\int\sin\theta\cos^2\theta\sin\lambda\,
d\theta,d\phi,d\lambda,d\psi=\frac{8\pi^2}{3}.
$$

Consequently

$$
\int\star dK^\flat=-8\pi^2\mu,
\qquad
\boxed{M=-\frac1{12\pi}\int\star dK^\flat
=\frac{2\pi}{3}r_+(r_+^2+a^2)}.
$$

This is the [Komar mass](../../../general-relativity.md#komar-mass) of the [Singly rotating six-dimensional Myers-Perry black hole](../../../general-relativity.md#singly-rotating-six-dimensional-myers-perry-black-hole) in the units of the question.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Substituting the two differential coordinate transformations cancels every coefficient singular as $\Delta^{-1}$, so the ingoing Kerr-like coordinates are regular at $r=r_+$. The inverse metric applied to the normal covector $dr$ has

$$
g^{ab}(dr)_b
=\frac{r^2+a^2}{\Sigma}\,\partial_v^a
+\frac{a}{\Sigma}\,\partial_\chi^a
+\frac{\Delta}{\Sigma}\,\partial_r^a.
$$

Its norm is $g^{rr}=\Delta/\Sigma$, which vanishes at $r=r_+$. Thus that level set is a [null hypersurface](../../../general-relativity.md#null-hypersurface). On it the raised normal is proportional to

$$
\partial_v+\frac{a}{r_+^2+a^2}\partial_\chi.
$$

Since the transformed stationary and axial Killing fields are $K=\partial_v$ and $m=\partial_\chi$, the horizon is a [Killing horizon](../../../general-relativity.md#killing-horizon) generated by

$$
\boxed{\xi=K+\Omega_Hm,
\qquad
\Omega_H=\frac{a}{r_+^2+a^2}}.
$$

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

For this horizon generator, direct evaluation of $\xi^b\nabla_b\xi^a=\kappa\xi^a$, or the radial derivative of $\Delta$, gives

$$
\kappa=\frac{\Delta'(r_+)}{2(r_+^2+a^2)}.
$$

Because $\Delta=r^2+a^2-\mu/r$ and $\mu=r_+(r_+^2+a^2)$,

$$
\Delta'(r_+)=2r_++\frac{\mu}{r_+^2}
=\frac{3r_+^2+a^2}{r_+},
$$

and therefore

$$
\boxed{\kappa=\frac{3r_+^2+a^2}{2r_+(r_+^2+a^2)}}.
$$

The induced horizon cross-section has volume element

$$
dA=r_+^2(r_+^2+a^2)\sin\theta\cos^2\theta\sin\lambda\,
d\theta,d\phi,d\lambda,d\psi.
$$

Using the unit-four-sphere integral from part b gives

$$
\boxed{A_H=\frac{8\pi^2}{3}r_+^2(r_+^2+a^2)}.
$$

<h3 id="2/e">e</h3>

↑ **Parent:** [2](#2)

<h4 id="2/e/solution">Solution</h4>

↑ **Parent:** [E](#2/e)

On $\theta=\lambda=0$, the radial function $r\Delta=r^3+a^2r-\mu$ is strictly increasing and has the single positive root $r_+$. The curvature invariant diverges at $r=0$, and $g^{rr}=\Delta/\Sigma<0$ immediately inside the horizon, so this is a spacelike singularity. The maximally extended [Penrose diagram](../../../general-relativity.md#penrose-diagram) therefore has the Schwarzschild form: two asymptotically flat exterior diamonds separated by future and past event horizons, with a spacelike future singularity above the black-hole regions and a spacelike past singularity below the white-hole regions. A collapse spacetime retains one exterior, the future horizon, and the future spacelike singularity.

## 3

↑ **Parent:** [Paper 311](paper-311.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

The [Physical-process first law for a rotating black hole](../../../general-relativity.md#physical-process-first-law-for-a-rotating-black-hole) states that a small flux of matter through an initially and finally stationary horizon obeys

$$
\boxed{\Delta M-\Omega_H\Delta J=\frac{\kappa}{8\pi}\Delta A}
$$

in units $G=1$. Let $k^a$ be an affinely parametrized horizon tangent with affine parameter $\lambda=0$ on a [bifurcation surface](../../../general-relativity.md#bifurcation-surface). Constancy of the [surface gravity](../../../general-relativity.md#surface-gravity) from the [Zeroth law of black-hole mechanics](../../../general-relativity.md#zeroth-law-of-black-hole-mechanics) and [Gaussian null coordinates](../../../general-relativity.md#gaussian-null-coordinates) give the horizon generator

$$
\xi^a=t^a+\Omega_Hm^a=\kappa\lambda k^a.
$$

To first order about a stationary horizon, the squared expansion and shear in the [Null Raychaudhuri equation](../../../geodesic-congruence.md#null-raychaudhuri-equation) are second order. The [Einstein field equations](../../../general-relativity.md#einstein-field-equations) reduce it to

$$
\frac{d\theta}{d\lambda}=-8\pi T_{ab}k^ak^b.
$$

The final stationary condition $\theta(\infty)=0$ gives

$$
\theta(\lambda)=8\pi\int_\lambda^\infty
T_{ab}k^ak^b\,d\lambda'.
$$

Since $d(\delta A)/d\lambda=\int\theta\,dA$, reversing the order of integration yields

$$
\Delta A=8\pi\int_H\lambda T_{ab}k^ak^b\,d\lambda,dA.
$$

The [stress-energy current from a Killing vector](../../../general-relativity.md#stress-energy-current-from-a-killing-vector) gives the horizon Killing-energy flux

$$
\Delta M-\Omega_H\Delta J
=\int_HT_{ab}\xi^ak^b\,d\lambda,dA
=\kappa\int_H\lambda T_{ab}k^ak^b\,d\lambda,dA,
$$

which proves the stated law.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

The [second law of black-hole mechanics](../../../general-relativity.md#second-law-of-black-hole-mechanics), or [Hawking's area theorem](../../../general-relativity.md#hawking-s-area-theorem), states that the total area of future-event-horizon cross-sections cannot decrease toward the future under the [null energy condition](../../../general-relativity.md#null-energy-condition) and the usual predictability assumptions. If any horizon generator had $\theta<0$, the twist-free [Null Raychaudhuri equation](../../../geodesic-congruence.md#null-raychaudhuri-equation) and the [null focusing theorem](../../../geodesic-congruence.md#null-focusing-theorem) would force a conjugate point at finite affine parameter. A generator complete to the future cannot pass through such a point while remaining on the achronal boundary of $J^-(\mathcal I^+)$. Hence $\theta\geq0$ everywhere on the regular future horizon, and $dA/d\lambda=\theta A\geq0$ proves the area law.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

The two initial [Kerr black holes](../../../general-relativity.md#kerr-black-hole) have total area

$$
A_i=16\pi\left(M^2+\sqrt{M^4-J^2}\right),
$$

whereas the final [Schwarzschild black hole](../../../general-relativity.md#schwarzschild-spacetime) has $A_f=16\pi M'^2$. [Hawking's area theorem](../../../general-relativity.md#hawking-s-area-theorem) implies

$$
M'^2\geq M^2+\sqrt{M^4-J^2}.
$$

Since $\eta=1-M'/(2M)$, the radiated fraction is bounded by

$$
\boxed{\eta\leq
1-\frac12\sqrt{1+\sqrt{1-\left(\frac{J}{M^2}\right)^2}}}.
$$

This upper bound increases with $|J|/M^2$ and reaches

$$
\boxed{\eta_{\rm max}=\frac12}
$$

for two initially extremal holes, $|J|=M^2$. For the final hole to be Schwarzschild, their spins must be oppositely directed so the total angular momentum vanishes. The bound assumes an idealized merger saturating the area law.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

First, causal futures of black-hole points remain in the black-hole region. Indeed, if $p\in B$ and $q\in J^+(p)$ could send a signal to [future null infinity](../../../general-relativity.md#future-null-infinity), concatenating the causal curves would put $p$ in $J^-(\mathcal I^+)$, a contradiction. Hence

$$
J^+(B)\cap\Sigma_2\subset B\cap\Sigma_2.
$$

Global hyperbolicity supplies the following connectedness lemma: if $C$ is connected on one [Cauchy hypersurface](../../../general-relativity.md#cauchy-surface), then $J^+(C)$ intersects any later Cauchy hypersurface in a connected set. To see the relevant mechanism, flow $C$ to the later surface along a continuous future timelike vector field; the image is connected, and every additional causally reachable point is joined to that image by the endpoint deformation of a causal curve inside the globally hyperbolic diamond. Applying the lemma to the connected component $B$ shows that $J^+(B)\cap\Sigma_2$ is connected. Since it is contained in $B\cap\Sigma_2$, it must lie wholly inside one connected component of that set. This is the [black-hole non-splitting theorem](../../../general-relativity.md#black-hole-non-splitting-theorem): later black-hole components may merge, but one earlier connected black hole cannot split into two future components.

## 4

↑ **Parent:** [Paper 311](paper-311.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

On a [stationary spacetime](../../../general-relativity.md#stationary-spacetime), choose a complete set of complex solutions $u_i$ of the massive [Klein-Gordon equation](../../../wave-equation.md#klein-gordon-equation) that have positive frequency with respect to the timelike [Killing vector field](../../../general-relativity.md#killing-vector-field) and are orthonormal in the conserved [Klein-Gordon inner product](../../../quantum-field-theory.md#klein-gordon-inner-product):

$$
(u_i,u_j)_{KG}=\delta_{ij},
\qquad
(u_i^*,u_j^*)_{KG}=-\delta_{ij},
\qquad
(u_i,u_j^*)_{KG}=0.
$$

The existence of a [Cauchy hypersurface](../../../general-relativity.md#cauchy-surface) in the [globally hyperbolic spacetime](../../../general-relativity.md#globally-hyperbolic-spacetime) makes the classical initial-value problem and this inner product well defined. Expand the real field as

$$
\widehat\phi=\sum_i\left(\widehat a_i u_i+\widehat a_i^\dagger u_i^*\right),
\qquad
[\widehat a_i,\widehat a_j^\dagger]=\delta_{ij}.
$$

The [vacuum state in a stationary spacetime](../../../quantum-field-theory.md#vacuum-state-in-a-stationary-spacetime) is defined by

$$
\boxed{\widehat a_i|0\rangle=0\quad\text{for every positive-frequency mode }i}.
$$

Acting with the creation operators builds the [bosonic Fock space](../../../quantum-field-theory.md#bosonic-fock-space).

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/i">i</h4>

↑ **Parent:** [B](#4/b)

<h5 id="4/b/i/solution">Solution</h5>

↑ **Parent:** [I](#4/b/i)

The early and late stationary regions define distinct positive-frequency mode bases and hence an in-vacuum and out-vacuum. Write their [Bogoliubov transformation](../../../quantum-field-theory.md#bogoliubov-transformation) as

$$
u_i^{\rm out}=\sum_j
\left(\alpha_{ij}u_j^{\rm in}+\beta_{ij}u_j^{{\rm in}*}\right).
$$

The corresponding operators satisfy

$$
\widehat b_i^{\rm out}=\sum_j
\left(\alpha_{ij}^*\widehat a_j^{\rm in}
-\beta_{ij}^*\widehat a_j^{{\rm in}\dagger}\right).
$$

Using $\widehat a_j^{\rm in}|0_{\rm in}\rangle=0$ and the canonical commutator gives the [particle number from Bogoliubov coefficients](../../../quantum-field-theory.md#particle-number-from-bogoliubov-coefficients):

$$
\boxed{\langle0_{\rm in}|\widehat N_i^{\rm out}|0_{\rm in}\rangle
=\sum_j|\beta_{ij}|^2}.
$$

Time dependence in the sandwich region can make $\beta_{ij}\neq0$, so the in-vacuum contains out-particles.

<h4 id="4/b/ii">ii</h4>

↑ **Parent:** [B](#4/b)

<h5 id="4/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#4/b/ii)

A gravitational-collapse spacetime is stationary and approximately empty in the remote past and settles to a stationary black-hole exterior in the future, with a dynamical region between them. The same comparison of in- and out-positive-frequency modes therefore applies. Tracing an outgoing late-time mode backward through the collapse produces an exponentially blueshifted mixture of early positive and negative frequencies. Its nonzero Bogoliubov beta coefficient yields the thermal occupation numbers of [Hawking radiation](../../../general-relativity.md#hawking-radiation), while partner modes pass through the [event horizon](../../../general-relativity.md#event-horizon).

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/i">i</h4>

↑ **Parent:** [C](#4/c)

<h5 id="4/c/i/solution">Solution</h5>

↑ **Parent:** [I](#4/c/i)

The horizon generator must be null at $r=r_+$. Substitution of $\xi=\partial_v+\Omega_H\partial_\chi$ in the [Kerr black hole](../../../general-relativity.md#kerr-black-hole) metric gives

$$
\boxed{\Omega_H=\frac{a}{r_+^2+a^2}
=\frac{a}{2Mr_+}}.
$$

The [surface gravity](../../../general-relativity.md#surface-gravity) and [Hawking temperature](../../../general-relativity.md#hawking-temperature) are

$$
\kappa=\frac{r_+-r_-}{2(r_+^2+a^2)},
\qquad
\boxed{T_H=\frac{\kappa}{2\pi}
=\frac{r_+-r_-}{4\pi(r_+^2+a^2)}
=\frac{\sqrt{M^2-a^2}}{4\pi Mr_+}}.
$$

<h4 id="4/c/ii">ii</h4>

↑ **Parent:** [C](#4/c)

<h5 id="4/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#4/c/ii)

For $a=0$, $T_H=(8\pi M)^{-1}$, so the Schwarzschild black hole has negative [heat capacity](../../../thermodynamics.md#heat-capacity). A small energy gain from a reservoir lowers its temperature below the reservoir temperature and causes further absorption; a small energy loss raises its temperature and causes further emission. The equilibrium is therefore unstable in the [canonical ensemble](../../../statistical-physics.md#canonical-ensemble).

<h4 id="4/c/iii">iii</h4>

↑ **Parent:** [C](#4/c)

<h5 id="4/c/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#4/c/iii)

Define

$$
s=\sqrt{1-\frac{J^2}{M^4}}=\sqrt{1-\frac{a^2}{M^2}}.
$$

The [Bekenstein-Hawking entropy](../../../general-relativity.md#bekenstein-hawking-entropy) and [Hawking temperature](../../../general-relativity.md#hawking-temperature) become

$$
S_{BH}=\frac A4=2\pi Mr_+=2\pi M^2(1+s),
\qquad
T_H=\frac{s}{4\pi M(1+s)}.
$$

At fixed $J$,

$$
\frac{ds}{dM}=\frac{2(1-s^2)}{sM},
\qquad
\left.\frac{dT_H}{dM}\right|_J
=\frac{T_H}{M}\frac{2-2s-s^2}{s^2}.
$$

The fixed-$J$ first law gives $(\partial S_{BH}/\partial M)_J=1/T_H$, so

$$
C_J=T_H\left(\frac{\partial S_{BH}}{\partial T_H}\right)_J
=\left(\frac{\partial T_H}{\partial M}\right)_J^{-1}.
$$

Therefore the [Kerr black-hole heat capacity at fixed angular momentum](../../../general-relativity.md#kerr-black-hole-heat-capacity-at-fixed-angular-momentum) is

$$
\boxed{C_J=4\pi M^2
\frac{s(1+s)}{2-2s-s^2}}.
$$

At $a=0$, this correctly reduces to $C_J=-8\pi M^2$.

<h4 id="4/c/iv">iv</h4>

↑ **Parent:** [C](#4/c)

<h5 id="4/c/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#4/c/iv)

Local thermal stability against energy exchange with a fixed-temperature reservoir requires $C_J>0$. Since $s\geq0$, this means

$$
2-2s-s^2>0
\quad\Longleftrightarrow\quad
s<\sqrt3-1.
$$

Equivalently,

$$
\boxed{\sqrt{2\sqrt3-3}<\frac{|a|}{M}<1}.
$$

The lower endpoint is the divergent-heat-capacity transition. The extremal endpoint $|a|=M$ has $T_H=0$ and $C_J=0$ and is obtained only as a limiting case.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2021](../../2021.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
