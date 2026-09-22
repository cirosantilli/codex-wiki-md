# Paper 304

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2022/paper_304.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2022/paper_304.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [i](#1/a/i)
      - [Solution](#1/a/i/solution)
    - [ii](#1/a/ii)
      - [Solution](#1/a/ii/solution)
  - [b](#1/b)
    - [i](#1/b/i)
      - [Solution](#1/b/i/solution)
    - [ii](#1/b/ii)
      - [Solution](#1/b/ii/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
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
    - [i](#4/d/i)
      - [Solution](#4/d/i/solution)
    - [ii](#4/d/ii)
      - [Solution](#4/d/ii/solution)

## 1

↑ **Parent:** [Paper 304](paper-304.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/i">i</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/i/solution">Solution</h5>

↑ **Parent:** [I](#1/a/i)

Insert a complete set of [momentum eigenstates](../../../quantum-mechanics.md#momentum-eigenstate) into the [quantum-mechanical propagator](../../../quantum-mechanics.md#quantum-mechanical-propagator):

$$
\begin{aligned}
K(x_f,T;x_i,0)
&=\langle x_f|e^{-i\widehat p^2T/(2m\hbar)}|x_i\rangle\\
&=\int_{-\infty}^{\infty}\frac{dp}{2\pi\hbar}
\exp\!\left[\frac{i}{\hbar}p(x_f-x_i)-\frac{iT}{2m\hbar}p^2\right].
\end{aligned}
$$

Completing the square and evaluating the resulting [Gaussian integral](../../../calculus.md#gaussian-integral), with the usual [i-epsilon prescription](../../../quantum-field-theory.md#feynman-i-epsilon-prescription), gives the [free-particle propagator](../../../quantum-mechanics.md#free-particle-propagator)

$$
\boxed{K(x_f,T;x_i,0)=
\sqrt{\frac{m}{2\pi i\hbar T}}
\exp\!\left[\frac{im(x_f-x_i)^2}{2\hbar T}\right]}.
$$

The square-root branch is fixed by requiring $K(x_f,T;x_i,0)\to\delta(x_f-x_i)$ as $T\downarrow0$.

<h4 id="1/a/ii">ii</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/a/ii)

The [Euler-Lagrange equation](../../../analysis.md#euler-lagrange-equation) is $m\ddot x=0$. The unique path with the prescribed endpoints is therefore

$$
x_{\rm cl}(t)=x_i+\frac{x_f-x_i}{T}t.
$$

It is a minimum of the Euclidean action and a stationary point of the real-time action. Its classical action is

$$
S_{\rm cl}=\int_0^T\frac m2\dot x_{\rm cl}^{,2},dt
=\frac{m(x_f-x_i)^2}{2T}.
$$

The [principle of stationary action](../../../classical-mechanics.md#principle-of-stationary-action) consequently fixes the position-dependent phase of the [semiclassical propagator](../../../quantum-mechanics.md#semiclassical-propagator) as

$$
K(x_f,T;x_i,0)=C(T)e^{iS_{\rm cl}/\hbar}.
$$

Because the action is quadratic, the stationary-phase evaluation of the [path integral](../../../quantum-field-theory.md#path-integral) is exact. Composition of propagators, or the [Van Vleck determinant](../../../quantum-mechanics.md#van-vleck-determinant), gives $C(T)=\sqrt{m/(2\pi i\hbar T)}$, reproducing part i.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/i">i</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/i/solution">Solution</h5>

↑ **Parent:** [I](#1/b/i)

The [particle on a circle](../../../quantum-mechanics.md#particle-in-a-ring) has the complete orthonormal basis of [energy eigenstates](../../../quantum-mechanics.md#energy-eigenstate) $\{|n\rangle:n\in\mathbb Z\}$. Its spectral representation gives

$$
\begin{aligned}
K(\theta_f,T;\theta_i,0)
&=\sum_{n\in\mathbb Z}\langle\theta_f|n\rangle
e^{-iE_nT/\hbar}\langle n|\theta_i\rangle\\
&=\boxed{\frac1{2\pi}\sum_{n\in\mathbb Z}
\exp\!\left[in(\theta_f-\theta_i)
-\frac{in^2\hbar T}{2mR^2}\right]}.
\end{aligned}
$$

The integer $n$ is the quantized [angular momentum](../../../classical-mechanics.md#angular-momentum) in units of $\hbar$.

<h4 id="1/b/ii">ii</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/b/ii)

Choose a real lift $\Delta\theta=\theta_f-\theta_i$. Classical paths fall into [winding number](../../../complex-analysis.md#winding-number) sectors $j\in\mathbb Z$ and are

$$
\theta_j(t)=\theta_i+\frac{\Delta\theta+2\pi j}{T}t,
\qquad
S_j=\frac{mR^2}{2T}(\Delta\theta+2\pi j)^2.
$$

Each sector has the same fluctuation determinant, so the image-sum form of the propagator is

$$
K(\theta_f,T;\theta_i,0)
=\sqrt{\frac{mR^2}{2\pi i\hbar T}}
\sum_{j\in\mathbb Z}e^{iS_j/\hbar}.
$$

Set $a=\hbar T/(2mR^2)$. Applying the [Poisson summation formula](../../../fourier-analysis.md#poisson-summation-formula) to the Gaussian $e^{ix^2/(4a)}$ gives

$$
\frac1{\sqrt{4\pi ia}}
\sum_{j\in\mathbb Z}e^{i(\Delta\theta+2\pi j)^2/(4a)}
=\frac1{2\pi}\sum_{n\in\mathbb Z}e^{in\Delta\theta-ian^2},
$$

which is exactly the spectral propagator found in part i. Thus the angular-momentum sum is dual to a sum over homotopy classes of classical paths.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

With a nonconstant [potential energy](../../../classical-mechanics.md#potential-energy), momentum no longer diagonalizes the [Hamiltonian operator](../../../quantum-mechanics.md#hamiltonian-quantum-mechanics). The operator derivation must use the energy eigenfunctions of the full Hamiltonian, a [Dyson series](../../../perturbative-quantum-field-theory.md#dyson-series), or a time-sliced [Trotter product formula](../../../numerical-analysis.md#lie-product-formula). In the classical derivation, the straight paths are replaced by every solution of the nonlinear [Euler-Lagrange equation](../../../analysis.md#euler-lagrange-equation) with the specified endpoints. The [semiclassical propagator](../../../quantum-mechanics.md#semiclassical-propagator) becomes a sum

$$
K(q_f,T;q_i,0)\simeq
\sum_{q_{\rm cl}}
\left(\frac{1}{2\pi i\hbar}
\left|-\frac{\partial^2S_{\rm cl}}{\partial q_f\partial q_i}\right|\right)^{1/2}
e^{iS_{\rm cl}/\hbar-i\pi\mu_{\rm cl}/2},
$$

where the prefactor is the [Van Vleck determinant](../../../quantum-mechanics.md#van-vleck-determinant) and $\mu_{\rm cl}$ is a [Maslov index](../../../symplectic-geometry.md#maslov-index). Unlike a quadratic theory, the classical-path sum is generally only an asymptotic approximation: the exact [path integral](../../../quantum-field-theory.md#path-integral) includes fluctuations of every order. On the circle, the sum must still include all [winding number](../../../complex-analysis.md#winding-number) sectors.

## 2

↑ **Parent:** [Paper 304](paper-304.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

For the Euclidean [quartic scalar field theory](../../../scalar-field-theory.md#quartic-interaction), expansion of $e^{-S}$ gives the momentum-space rules

- an internal scalar line of momentum $p$ contributes $(p^2+m^2)^{-1}$;
- a four-scalar vertex contributes $-\lambda$ and a momentum-conserving delta function;
- each independent [loop momentum](../../../perturbative-quantum-field-theory.md#loop-momentum) is integrated with $\int d^4k/(2\pi)^4$;
- each graph is divided by its [Feynman-diagram symmetry factor](../../../perturbative-quantum-field-theory.md#feynman-diagram-symmetry-factor).

At one loop, the [four-point one-particle-irreducible correlation function](../../../perturbative-quantum-field-theory.md#four-point-one-particle-irreducible-correlation-function) receives the three bubble diagrams in the $s$, $t$, and $u$ channels. If $P$ is the momentum through one channel, its contribution is

$$
\frac{\lambda_a^2}{2}I(P;m,\Lambda),
\qquad
I(P;m,\Lambda)=\int_{|k|<\Lambda}\frac{d^4k}{(2\pi)^4}
\frac1{(k^2+m^2)((k+P)^2+m^2)}.
$$

Using a [Feynman parameter](../../../perturbative-quantum-field-theory.md#feynman-parameter), shifting the loop momentum, and writing $\Delta_x=m^2+x(1-x)P^2$ gives, up to terms caused by shifting the boundary of a hard cutoff,

$$
I(P;m,\Lambda)=\frac1{16\pi^2}\int_0^1dx
\left[
\log\frac{\Lambda^2+\Delta_x}{\Delta_x}
+\frac{\Delta_x}{\Lambda^2+\Delta_x}-1
\right].
$$

Thus every channel has the logarithmic ultraviolet divergence

$$
I(P;m,\Lambda)=\frac1{16\pi^2}\log\Lambda^2+O(1).
$$

The complete one-loop vertex is

$$
V_a^{(4)}=-\lambda_a+\frac{\lambda_a^2}{2}
\bigl[I(p_1+p_2;m,\Lambda)+I(p_1+p_3;m,\Lambda)+I(p_1+p_4;m,\Lambda)\bigr]
+O(\lambda_a^3).
$$

Let $I_{m,\mathrm{os}}$ denote the bracket evaluated at the chosen on-shell kinematic point. The [on-shell renormalization scheme](../../../perturbative-quantum-field-theory.md#on-shell-renormalization-scheme) requires $V_a^{(4)}|_{\mathrm{os}}=-\lambda_{\mathrm{phys}}$, hence the perturbative solution is

$$
\boxed{\lambda_a=\lambda_{\mathrm{phys}}
+\frac{\lambda_{\mathrm{phys}}^2}{2}I_{m,\mathrm{os}}
+O(\lambda_{\mathrm{phys}}^3)}.
$$

The cutoff dependence of $\lambda_a$ is the coupling [counterterm](../../../perturbative-quantum-field-theory.md#counterterm) needed to hold the measured coupling fixed.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

After integration by parts, the quadratic ghost operator is $c_1(-\partial^2)+c_2M^2$. Matching its propagator to the scalar propagator after $M\mapsto m$ requires

$$
c_1=c_2=1.
$$

Differentiating $c_3\lambda\bar\eta\phi^2\eta$ with respect to its two identical scalar fields gives the ghost-scalar vertex $-2c_3\lambda$. Matching it to the four-scalar vertex therefore requires

$$
c_3=\frac12.
$$

The additional rules are an oriented ghost propagator $(p^2+M^2)^{-1}$, a two-scalar two-ghost vertex $-\lambda$, and a minus sign for every closed loop of [Grassmann-valued fields](../../../quantum-field-theory.md#grassmann-field).

Besides the scalar bubbles from part a, each channel now has a closed heavy-ghost bubble. Its two directed internal lines cannot be interchanged, so it has no scalar bubble's factor $1/2$. Consequently

$$
V_b^{(4)}=-\lambda_b+\lambda_b^2
\sum_{P\in\{p_1+p_2,p_1+p_3,p_1+p_4\}}
\left[\frac12I(P;m,\Lambda)-I(P;M,\Lambda)\right]
+O(\lambda_b^3).
$$

If $I_{M,\mathrm{os}}$ denotes the corresponding sum of heavy integrals, on-shell matching gives

$$
\boxed{\lambda_b=\lambda_{\mathrm{phys}}
+\lambda_{\mathrm{phys}}^2
\left(\frac12I_{m,\mathrm{os}}-I_{M,\mathrm{os}}\right)
+O(\lambda_{\mathrm{phys}}^3)}.
$$

The root continuously connected to $\lambda_b=\lambda_{\mathrm{phys}}$ is the perturbative, small positive root.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

After $\lambda_a$ and $\lambda_b$ have been matched to the same measured coupling, the nonanalytic low-energy dependence from the light scalar loops is identical. For $|P|\ll M$, a heavy loop has the local expansion

$$
I(P;M,\Lambda)=I(0;M,\Lambda)+O(P^2/M^2).
$$

Its constant term is already absorbed into the matched quartic coupling, while the remaining terms are higher-dimensional local interactions suppressed by powers of $M$. Dependence on the finite ultraviolet cutoff is similarly suppressed by powers of $\Lambda$. This is [heavy-field decoupling](../../../quantum-field-theory.md#heavy-field-decoupling): low-energy scattering agrees up to $O(p^2/M^2,p^2/\Lambda^2)$ corrections after all relevant parameters are matched. At energies comparable to $M$, the two theories differ sharply because the second theory contains wrong-statistics heavy states.

## 3

↑ **Parent:** [Paper 304](paper-304.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Under the global [U(1) gauge symmetry](../../../relativistic-quantum-field.md#u-1-gauge-symmetry), the phases in $\bar\psi\psi$ cancel and $\alpha$ is constant, so

$$
D_\mu(e^{i\alpha}\psi)=e^{i\alpha}D_\mu\psi.
$$

Both the fermion term and $F_{\mu\nu}F^{\mu\nu}$ are therefore invariant. To extract the [Noether current](../../../quantum-field-theory.md#noether-current), temporarily promote $\alpha$ to a function. The variation of the action is

$$
\delta S=i\int d^4x\,(\partial_\mu\alpha)\bar\psi\gamma^\mu\psi
=-i\int d^4x\,\alpha\,\partial_\mu j^\mu,
\qquad j^\mu=\bar\psi\gamma^\mu\psi.
$$

The [Euler-Lagrange equations](../../../analysis.md#euler-lagrange-equation) then imply the [current conservation](../../../quantum-field-theory.md#conserved-current) law $\partial_\mu j^\mu=0$.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Perform the infinitesimal local change of integration variables

$$
\delta\psi(x)=i\alpha(x)\psi(x),
\qquad
\delta\bar\psi(x)=-i\alpha(x)\bar\psi(x)
$$

in the Euclidean [path integral](../../../quantum-field-theory.md#path-integral) for $\langle j^\mu(x)\psi(x_1)\bar\psi(x_2)\rangle$. The vector transformation has no [quantum anomaly](../../../relativistic-quantum-field.md#anomaly-physics), so its [functional measure](../../../quantum-field-theory.md#functional-measure) is invariant. The action variation supplies $-i\int\alpha\,\partial_\mu j^\mu$, while varying the two charged insertions supplies contact terms at $x_1$ and $x_2$ with opposite signs. Since a change of integration variables cannot change the integral, the coefficient of the arbitrary function $\alpha(x)$ vanishes:

$$
\boxed{
\partial_\mu\langle j^\mu(x)\psi(x_1)\bar\psi(x_2)\rangle
=-\bigl[\delta^{(4)}(x-x_1)-\delta^{(4)}(x-x_2)\bigr]
\langle\psi(x_1)\bar\psi(x_2)\rangle }.
$$

This [Schwinger-Dyson equation](../../../perturbative-quantum-field-theory.md#schwinger-dyson-equation) is the position-space [Ward-Takahashi identity](../../../perturbative-quantum-field-theory.md#ward-identity).

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Fourier transformation sends $\partial_\mu$ to $iq_\mu$. Write the connected current three-point function as the two full [Dirac propagators](../../../quantum-field-theory.md#dirac-propagator) joined to the amputated vertex:

$$
\langle j^\mu\psi\bar\psi\rangle_{
m conn}
=G(p_1)V_3^\mu(q,p_1,p_2)G(p_2),
\qquad q=p_1-p_2.
$$

The two contact terms remove one propagator at a time. Multiplying the transformed identity by $G^{-1}(p_1)$ on the left and $G^{-1}(p_2)$ on the right yields

$$
\boxed{iq_\mu V_3^\mu(q,p_1,p_2)
=ie\bigl[G^{-1}(p_1)-G^{-1}(p_2)\bigr]},
\qquad p_2=p_1-q.
$$

This is the momentum-space [Ward-Takahashi identity](../../../perturbative-quantum-field-theory.md#ward-identity) for the full vertex and full propagator.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

Taking $q\to0$ in the [Ward-Takahashi identity](../../../perturbative-quantum-field-theory.md#ward-identity) gives

$$
V_3^\mu(0,p,p)=e\,\frac{\partial G^{-1}(p)}{\partial p_\mu}
$$

up to the displayed Euclidean $i$ conventions. The ultraviolet divergence of the zero-momentum vertex is therefore exactly the derivative of the fermion self-energy divergence. In renormalization-constant notation this is

$$
\boxed{Z_1=Z_2},
$$

so the vertex and fermion [wave-function renormalization](../../../perturbative-quantum-field-theory.md#wave-function-renormalization) are not independent. The remaining [charge renormalization](../../../perturbative-quantum-field-theory.md#charge-renormalization) is controlled by photon wave-function renormalization; in a common convention $e_0=Z_3^{-1/2}e$.

The derivation used only an exact change of variables, invariance of the action, and invariance of the measure. It therefore holds nonperturbatively whenever the regulator and definition of the theory preserve the vector symmetry. A symmetry-breaking regulator requires symmetry-restoring [counterterms](../../../perturbative-quantum-field-theory.md#counterterm); a genuine [quantum anomaly](../../../relativistic-quantum-field.md#anomaly-physics) would obstruct the identity, but vector QED has no such anomaly.

## 4

↑ **Parent:** [Paper 304](paper-304.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

Substituting $\delta A_\mu=g^{-1}\partial_\mu\alpha-i[A_\mu,\alpha]$ into the curvature and collecting terms gives the covariant transformation

$$
\boxed{\delta F_{\mu\nu}=-i[F_{\mu\nu},\alpha]}.
$$

Equivalently, $\delta F_{\mu\nu}^a=f^{abc}F_{\mu\nu}^b\alpha^c$ in the stated conventions. Since $F_{\mu\nu}^aF^{\mu\nu,a}$ is proportional to $\operatorname{tr}(F_{\mu\nu}F^{\mu\nu})$, cyclicity of the [matrix trace](../../../linear-algebra.md#matrix-trace) gives

$$
\delta\operatorname{tr}(F_{\mu\nu}F^{\mu\nu})
=-i\operatorname{tr}([F_{\mu\nu}F^{\mu\nu},\alpha])=0.
$$

**Thus the [Yang-Mills action](../../../relativistic-quantum-field.md#yang-mills-action) is [gauge-invariant](../../../relativistic-quantum-field.md#gauge-invariance).**

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

In components the [BRST transformation](../../../relativistic-quantum-field.md#brst-symmetry) is

$$
sA_\mu^a=\partial_\mu c^a+gf^{abc}A_\mu^bc^c,
\qquad
sc^a=-\frac g2f^{abc}c^bc^c,
\qquad
s\bar c^a=B^a,
\qquad
sB^a=0.
$$

The last two equations immediately give $s^2\bar c=s^2B=0$. Applying the graded Leibniz rule to $s^2c$ produces a sum of three ghost monomials whose coefficient is the [Jacobi identity](../../../lie-algebra.md#jacobi-identity) $f^{e[ab}f^{c]de}$, so $s^2c=0$. Finally,

$$
s^2A_\mu=D_\mu(sc)-ig[D_\mu c,c]=0;
$$

the derivative terms cancel by anticommutation of the [Faddeev-Popov ghost fields](../../../relativistic-quantum-field.md#faddeev-popov-ghost), and the remaining terms again cancel by the Jacobi identity. Hence $s^2=0$ on every field: $s$ is a nilpotent Grassmann-odd differential.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

The [Yang-Mills action](../../../relativistic-quantum-field.md#yang-mills-action) is BRST invariant because its field strength transforms covariantly, and the gauge-fixing contribution is BRST exact. Nilpotence therefore gives

$$
s\mathcal L=s\mathcal L_{\rm YM}+s^2\!\left(\bar c^aL[A^a]-\frac\xi2\bar c^aB^a\right)=0.
$$

The gauge-fixing functional itself is generally not closed: $sL[A]=L[Dc]$. Applying the graded Leibniz rule gives

$$
\boxed{\mathcal L=\frac14F_{\mu\nu}^aF^{\mu\nu,a}
+B^aL[A^a]-\frac\xi2B^aB^a-\bar c^aL[(D c)^a]}.
$$

The [Nakanishi-Lautrup field](../../../relativistic-quantum-field.md#nakanishi-lautrup-field) $B^a$ is auxiliary. Its algebraic equation $B^a=L[A^a]/\xi$ turns the middle terms into $L[A]^2/(2\xi)$, while the final term is the [Faddeev-Popov ghost field](../../../relativistic-quantum-field.md#faddeev-popov-ghost) action.

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/i">i</h4>

↑ **Parent:** [D](#4/d)

<h5 id="4/d/i/solution">Solution</h5>

↑ **Parent:** [I](#4/d/i)

For $L[A^a]=\partial^\mu A_\mu^a$, eliminating the [Nakanishi-Lautrup field](../../../relativistic-quantum-field.md#nakanishi-lautrup-field) gives the [covariant gauge](../../../relativistic-quantum-field.md#covariant-gauge) Lagrangian

$$
\mathcal L=\frac14F_{\mu\nu}^aF^{\mu\nu,a}
+\frac1{2\xi}(\partial^\mu A_\mu^a)^2
-\bar c^a\partial^\mu(D_\mu c)^a.
$$

The first term supplies the gluon kinetic term, three-gluon vertex, and four-gluon vertex. The second makes the quadratic gauge-field operator invertible. The last supplies the ghost propagator and ghost-antighost-gluon vertex.

The nonzero one-loop contributions to the [gluon propagator](../../../relativistic-quantum-field.md#gluon-propagator) are a gluon bubble with two three-gluon vertices and a closed ghost bubble with two ghost-antighost-gluon vertices. A four-gluon tadpole is also present with a cutoff regulator; for massless fields it is a scaleless integral and vanishes in [dimensional regularization](../../../perturbative-quantum-field-theory.md#dimensional-regularization).

<h4 id="4/d/ii">ii</h4>

↑ **Parent:** [D](#4/d)

<h5 id="4/d/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#4/d/ii)

For $L[A^a]=n^\mu A_\mu^a$, eliminating $B^a$ gives the [axial gauge](../../../relativistic-quantum-field.md#axial-gauge) term $(n\mathbin\cdot A^a)^2/(2\xi)$ and ghost operator

$$
-\bar c^a n^\mu(D_\mu c)^a.
$$

In the strict $\xi\to0$ gauge, $n\mathbin\cdot A=0$. The gauge-field-dependent part of $n\mathbin\cdot D$ then vanishes, the [Faddeev-Popov determinant](../../../relativistic-quantum-field.md#faddeev-popov-determinant) becomes field independent, and the ghosts decouple. The one-loop [gluon propagator](../../../relativistic-quantum-field.md#gluon-propagator) therefore receives the gluon bubble but no ghost bubble. As in the covariant gauge, the four-gluon tadpole can occur with a hard cutoff and vanishes as a scaleless integral in dimensional regularization. Gauge-invariant observables agree between the two gauges even though their individual propagators and diagrammatic decompositions differ.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2022](../../2022.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
