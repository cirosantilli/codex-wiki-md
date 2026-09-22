# Paper 344

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2018/paper_344.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2018/paper_344.pdf)

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
  - [e](#3/e)
    - [Solution](#3/e/solution)

## 1

↑ **Parent:** [Paper 344](paper-344.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Write $E(t)=\delta A/\delta x(t)$ for the [functional derivative](../../../calculus-of-variations.md#functional-derivative) of the [action](../../../classical-mechanics.md#action). Under [time reversal in classical mechanics](../../../classical-mechanics.md#time-reversal-in-classical-mechanics), $\dot x$ changes sign whereas $E$ is even by assumption. Thus the forward and reversed [Gaussian white noise](../../../stochastic-process.md#gaussian-white-noise) histories associated with the same geometric path are

$$
f_F=\zeta\dot x-E,\qquad f_B=-\zeta\dot x-E,
\qquad f_F^2-f_B^2=-4\zeta\dot xE.
$$

The [Onsager--Machlup path probability](../../../critical-phenomenon.md#onsager-machlup-path-probability) therefore gives

$$
\log\frac{\mathbb P_F}{\mathbb P_B}
=-\frac1{2\sigma^2}\int_{t_1}^{t_2}(f_F^2-f_B^2)\,dt,
\qquad
\boxed{\frac{\mathbb P_F}{\mathbb P_B}
=\exp\!\left[\frac{2\zeta}{\sigma^2}\int_{t_1}^{t_2}\dot x\frac{\delta A}{\delta x(t)}\,dt\right]}.
$$

Here the [path probabilities](../../../stochastic-process.md#path-probability) are densities conditional on their respective initial states; they are not separately normalized bridges conditioned on both endpoints. The noise-to-path [Jacobian determinant](../../../calculus.md#jacobian-determinant) must be treated with a consistent discretization: it cancels when it is invariant under [time reversal in classical mechanics](../../../classical-mechanics.md#time-reversal-in-classical-mechanics). This is the usual additive-noise [Langevin dynamics](../../../stochastic-process.md#langevin-dynamics) convention, including a constant-mass [Underdamped Langevin dynamics](../../../stochastic-calculus.md#underdamped-langevin-dynamics) or the [time-reversal invariance of a path Jacobian](../../../critical-phenomenon.md#time-reversal-invariance-of-a-path-jacobian) in midpoint [overdamped Langevin dynamics](../../../stochastic-calculus.md#overdamped-langevin-dynamics). A completely arbitrary velocity-dependent [Lagrangian](../../../calculus-of-variations.md#lagrangian) would require specifying that measure rather than deducing its cancellation solely from the parity of $E$.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

For an autonomous [Lagrangian](../../../calculus-of-variations.md#lagrangian), the [Euler-Lagrange equation](../../../analysis.md#euler-lagrange-equation) uses

$$
\frac{\delta A}{\delta x}=L_x-\frac{d}{dt}L_{\dot x},
\qquad H=\dot xL_{\dot x}-L.
$$

Apply the [chain rule](../../../calculus.md#chain-rule) to the [Hamiltonian](../../../classical-mechanics.md#hamiltonian) along an arbitrary smooth path, without assuming the unforced [Euler-Lagrange equation](../../../analysis.md#euler-lagrange-equation):

$$
\frac{dH}{dt}
=\ddot xL_{\dot x}+\dot x\frac{d}{dt}L_{\dot x}
-L_x\dot x-L_{\dot x}\ddot x
=-\dot x\frac{\delta A}{\delta x}.
$$

Consequently the [energy balance for an autonomous Lagrangian](../../../classical-mechanics.md#energy-balance-for-an-autonomous-lagrangian) is

$$
\boxed{-\int_{t_1}^{t_2}\dot x\frac{\delta A}{\delta x(t)}\,dt=H_2-H_1}.
$$

With explicit time dependence, an additional $-\partial_tL$ enters $dH/dt$. For ideal [Gaussian white noise](../../../stochastic-process.md#gaussian-white-noise), the identity is understood through smooth-noise regularization or the [Stratonovich chain rule](../../../stochastic-calculus.md#stratonovich-chain-rule). The original PDF correctly differentiates $L$ with respect to $\dot x$ in $H$; the supplied TeX's derivative with respect to $x$, its endpoint $t^2$, and its ordinary derivative of $A$ are transcription errors.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

At [thermal equilibrium](../../../thermodynamics.md#thermal-equilibrium), [microscopic reversibility](../../../thermodynamics.md#microscopic-reversibility) equates the probabilities of a path and its reversed path when both include their [Boltzmann distribution](../../../thermodynamics.md#boltzmann-distribution) initial weights. Denote their endpoint states by $z_1,z_2$, including velocity if needed. Since the [Hamiltonian](../../../classical-mechanics.md#hamiltonian) is even under [time reversal in classical mechanics](../../../classical-mechanics.md#time-reversal-in-classical-mechanics),

$$
\rho_{\rm eq}(z_1)\mathbb P_F
=\rho_{\rm eq}(z_2)\mathbb P_B,
\qquad \rho_{\rm eq}(z)\propto e^{-\beta H(z)},
\qquad \beta=\frac1{k_BT}.
$$

This [detailed balance](../../../markov-process.md#detailed-balance) condition and the [energy balance for an autonomous Lagrangian](../../../classical-mechanics.md#energy-balance-for-an-autonomous-lagrangian) yield

$$
\frac{\mathbb P_F}{\mathbb P_B}=e^{-\beta(H_2-H_1)},
\qquad \frac{2\zeta}{\sigma^2}=\beta,
\qquad \boxed{\sigma^2=2\zeta k_BT}.
$$

This is the [fluctuation-dissipation relation for a Langevin particle](../../../thermodynamics.md#fluctuation-dissipation-relation-for-a-langevin-particle): the strength of [Gaussian white noise](../../../stochastic-process.md#gaussian-white-noise) is fixed by the damping and [temperature](../../../thermodynamics.md#temperature), with $k_B$ the [Boltzmann constant](../../../thermodynamics.md#boltzmann-constant).

For an equilibrium [coarse-grained variable](../../../statistical-physics.md#coarse-grained-variable), the unresolved microscopic states contribute [entropy](../../../thermodynamics.md#entropy); their statistical weight is encoded in the [Helmholtz free energy](../../../thermodynamics.md#helmholtz-free-energy), rather than in a single microscopic energy. Relative to the same reference measure, $\rho_{\rm eq}(x)\propto e^{-\beta F(x)}$, so [microscopic reversibility](../../../thermodynamics.md#microscopic-reversibility) becomes

$$
\boxed{\frac{\mathbb P_F}{\mathbb P_B}=e^{-\beta(F_2-F_1)}}.
$$

This extension assumes an equilibrium coarse-grained description with reversible path statistics; externally driven dynamics need not obey this relation.

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

The [Neumann boundary conditions](../../../differential-equation.md#neumann-boundary-condition) give [Fourier modes](../../../fourier-analysis.md#fourier-mode) $q=n\pi/L$, including the spatially uniform mode $q=0$. In the frame translating with the mean deposition height, that mode has no restoring force and obeys

$$
dh_0=\sigma\,dW_t,\qquad
h_0(t)=h_0(0)+\sigma W_t,
\qquad \boxed{\operatorname{Var}h_0(t)=\operatorname{Var}h_0(0)+\sigma^2t}.
$$

Here $W_t$ is [Brownian motion](../../../brownian-motion.md), independent of the initial height. More generally $\langle h_0(t)^2\rangle=\langle h_0(0)^2\rangle+\sigma^2t$ when these [second moments](../../../probability-theory.md#second-moment) exist. Removing the mean deposition drift does not remove the [Gaussian white noise](../../../stochastic-process.md#gaussian-white-noise).

The [Brownian zero mode of a fluctuating interface](../../../stochastic-process.md#brownian-zero-mode-of-a-fluctuating-interface) has no [stationary distribution](../../../markov-process.md#stationary-distribution) on the real height axis for $\sigma^2>0$. This conclusion does not depend on assuming finite [variance](../../../variance.md): a stationary [characteristic function](../../../probability-theory.md#characteristic-function) would satisfy $\widehat\mu(k)=\widehat\mu(k)e^{-\sigma^2k^2t/2}$, hence vanish for every $k\ne0$, contradicting its continuity at zero and $\widehat\mu(0)=1$. Any stationary joint distribution of the whole height would have a stationary zero-mode marginal, which is impossible. Thus **the full unpinned height has no Boltzmann equilibrium**. Pinning the mean height, or retaining only the nonzero [Fourier modes](../../../fourier-analysis.md#fourier-mode), removes this obstruction. The PDF has $\dot h_q$; the TeX's $\hbar_q$ is a transcription error.

<h3 id="1/e">e</h3>

↑ **Parent:** [1](#1)

<h4 id="1/e/solution">Solution</h4>

↑ **Parent:** [E](#1/e)

For $q\ne0$ and $\alpha>0$, each [Fourier mode](../../../fourier-analysis.md#fourier-mode) is an [Ornstein-Uhlenbeck process](../../../stochastic-process.md#ornstein-uhlenbeck-process) with decay rate $r_q=\alpha q^2$. Its [explicit Ornstein-Uhlenbeck solution](../../../stochastic-process.md#explicit-ornstein-uhlenbeck-solution) is

$$
h_q(t)=e^{-r_qt}h_q(0)+\sigma\int_0^t e^{-r_q(t-s)}\,dW_q(s),
$$

so the [Itô isometry](../../../stochastic-calculus.md#ito-isometry) gives

$$
\langle h_q(t)^2\rangle
=e^{-2r_qt}\langle h_q(0)^2\rangle
+\frac{\sigma^2}{2r_q}(1-e^{-2r_qt}).
$$

To identify the [overdamped Langevin dynamics](../../../stochastic-calculus.md#overdamped-langevin-dynamics), choose a friction $\zeta_q>0$, a [harmonic oscillator](../../../classical-mechanics.md#simple-harmonic-motion) potential $V_q=\zeta_q\alpha q^2h_q^2/2$, and force noise $f_q=\zeta_q\eta_q$. The [fluctuation-dissipation relation for a Langevin particle](../../../thermodynamics.md#fluctuation-dissipation-relation-for-a-langevin-particle) then defines $k_BT_{\rm eff}=\zeta_q\sigma^2/2$. Its [Boltzmann distribution](../../../thermodynamics.md#boltzmann-distribution) is

$$
P_q(h)=\sqrt{\frac{\alpha q^2}{\pi\sigma^2}}
\exp\!\left(-\frac{\alpha q^2h^2}{\sigma^2}\right),
\qquad \boxed{\langle h_q^2\rangle_{\rm st}=\frac{\sigma^2}{2\alpha q^2}\propto q^{-2}}.
$$

This is the [stationary spectrum of a linear fluctuating interface](../../../stochastic-process.md#stationary-spectrum-of-a-linear-fluctuating-interface), also following from the [equipartition theorem](../../../statistical-physics.md#equipartition-theorem). The numerical prefactor uses exactly the mode-noise normalization given in the paper. The nonzero modes can therefore have a stationary [Gaussian distribution](../../../probability-theory.md#normal-distribution) even though the unpinned zero mode cannot.

## 2

↑ **Parent:** [Paper 344](paper-344.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Use the paper's [velocity gradient](../../../continuum-mechanics.md#velocity-gradient) convention $A_{ij}=\partial_i v_j$, so $\Omega=(A-A^T)/2$ and $D=(A+A^T)/2$. In a [rigid motion](../../../geometry-and-topology.md#rigid-transformation) there is rotation but no [rate-of-strain tensor](../../../viscous-fluid-flow.md#strain-rate-tensor): $D=0$. A [polar order parameter](../../../critical-phenomenon.md#polar-order-parameter) attached to the material must rotate exactly with it. In this convention its [material derivative](../../../continuum-mechanics.md#material-derivative) is $-\Omega\mathbf p$, and its [corotational derivative of a polar vector](../../../rheology.md#corotational-derivative-of-a-polar-vector) must vanish.

Thus the compensating term is $+\Omega\mathbf p$ with **coefficient exactly one**. This follows from an [objective time derivative](../../../rheology.md#objective-time-derivative) and is independent of material properties. By contrast, the response to $D\mathbf p$ describes deformation and [flow alignment of a polar order parameter](../../../critical-phenomenon.md#flow-alignment-of-a-polar-order-parameter); its coefficient $\xi$ can depend on the material. The transposed [velocity gradient](../../../continuum-mechanics.md#velocity-gradient) convention is essential to the sign of $\Omega$.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Let $h_i=\delta F/\delta p_i$ be the [polar molecular field](../../../critical-phenomenon.md#polar-molecular-field), with the positive [functional derivative](../../../calculus-of-variations.md#functional-derivative) convention used in the paper. During a pure advective displacement $u_j$, the [polar order parameter](../../../critical-phenomenon.md#polar-order-parameter) changes by

$$
\delta p_i=-u_j\partial_jp_i-\Omega^u_{ij}p_j+\xi D^u_{ij}p_j,
\quad \Omega^u_{ij}=\frac{\partial_i u_j-\partial_j u_i}{2},
\quad D^u_{ij}=\frac{\partial_i u_j+\partial_j u_i}{2}.
$$

The [free energy](../../../thermodynamics.md#thermodynamic-free-energy) change is $\delta F=\int h_i\delta p_i\,d^dr$. Assume periodic boundaries, or boundary conditions that eliminate the surface work, and [incompressibility](../../../fluid-mechanics.md#incompressible-flow) $\partial_j u_j=0$. [Integration by parts](../../../calculus.md#integration-by-parts) in the advective term gives

$$
-\int h_i u_j\partial_jp_i\,d^dr
=\int u_jp_i\partial_jh_i\,d^dr
=\int\Sigma^{(1)}_{ij}\partial_i u_j\,d^dr,
\qquad \partial_i\Sigma^{(1)}_{ij}=-p_k\partial_jh_k.
$$

Relabelling the dummy indices in the rotational and [flow alignment of a polar order parameter](../../../critical-phenomenon.md#flow-alignment-of-a-polar-order-parameter) terms gives

$$
-h_i\Omega^u_{ij}p_j
=\frac{p_i h_j-p_jh_i}{2}\partial_i u_j,
\qquad
\xi h_iD^u_{ij}p_j
=\frac{\xi(p_i h_j+p_jh_i)}2\partial_i u_j.
$$

Therefore $\delta F=\int\Sigma^p_{ij}\partial_i u_j\,d^dr$, with the [reversible stress of a polar liquid crystal](../../../critical-phenomenon.md#reversible-stress-of-a-polar-liquid-crystal)

$$
\boxed{\Sigma^p_{ij}=\Sigma^{(1)}_{ij}
+\frac{p_i h_j-p_jh_i}{2}
+\frac{\xi(p_i h_j+p_jh_i)}2,
\quad \partial_i\Sigma^{(1)}_{ij}=-p_k\partial_jh_k}.
$$

For a local [free-energy density](../../../statistical-physics.md#free-energy-density) $f(\mathbf p,\nabla\mathbf p)$, an explicit choice is

$$
\Sigma^{(1)}_{ij}=(f-p_kh_k)\delta_{ij}
-\frac{\partial f}{\partial(\partial_i p_k)}\partial_jp_k.
$$

Its [divergence](../../../calculus.md#divergence) is exactly $-p_k\partial_jh_k$, by the [Euler-Lagrange equation](../../../analysis.md#euler-lagrange-equation) for $h_k$. A [pressure](../../../thermodynamics.md#pressure) term can be reassigned in an [incompressible flow](../../../fluid-mechanics.md#incompressible-flow); the chosen representative realizes the printed divergence without that ambiguity. The force density $\partial_i\Sigma^p_{ij}$ has mechanical power $-\int\Sigma^p_{ij}\partial_i v_j$, the negative of the advective [free energy](../../../thermodynamics.md#thermodynamic-free-energy) rate, which checks the stress sign.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

The [polar molecular field](../../../critical-phenomenon.md#polar-molecular-field) is

$$
h_i=(a+b|\mathbf p|^2)p_i-\kappa\nabla^2p_i.
$$

For a spatially uniform [polar order parameter](../../../critical-phenomenon.md#polar-order-parameter), $\mathbf h=(a+bp^2)\mathbf p$, so it is colinear with $\mathbf p$ and its magnitude is $|\mathbf h|=|a+bp^2|p$. The scalar factor can be negative; colinearity does not necessarily mean parallel orientation.

For the [simple shear flow](../../../viscous-fluid-flow.md#simple-shear-flow), the paper's [velocity gradient](../../../continuum-mechanics.md#velocity-gradient) convention gives

$$
\Omega=\frac g2\begin{pmatrix}0&-1\\1&0\end{pmatrix},
\qquad D=\frac g2\begin{pmatrix}0&1\\1&0\end{pmatrix}.
$$

Substitute these matrices into $\dot{\mathbf p}=-\Omega\mathbf p+\xi D\mathbf p-\Gamma\mathbf h$. Projection along and perpendicular to the [polar order parameter](../../../critical-phenomenon.md#polar-order-parameter) yields

$$
\frac{\dot p}{p}=\frac{\xi g}{2}\sin2\theta-\Gamma(a+bp^2),
\qquad \dot\theta=\frac g2(\xi\cos2\theta-1).
$$

Assume $g\ne0$, $\Gamma>0$, $b>0$ and $p>0$. The [flow-alignment angle in planar shear](../../../critical-phenomenon.md#flow-alignment-angle-in-planar-shear) must satisfy

$$
\boxed{\cos2\theta=\frac1\xi,
\quad |\xi|\ge1,
\quad \tan^2\theta=\frac{\xi-1}{\xi+1}}.
$$

For $\xi=-1$, use the cosine equation: $\theta=\pi/2$ modulo $\pi$, and the displayed tangent is infinite. The radial equation gives

$$
\boxed{p^2=\frac{-a+\xi g\sin2\theta/(2\Gamma)}b
=\frac{-a\ \pm\ g\sqrt{\xi^2-1}/(2\Gamma)}b},
$$

where the sign distinguishes the angular branches, and only positive right-hand sides are ordered solutions. Linearizing the angular equation gives $\delta\dot\theta=-g\xi\sin2\theta\,\delta\theta$. For $|\xi|>1$, the stable angular branch therefore has

$$
\boxed{p_{\rm stable}^2=\frac{-a+|g|\sqrt{\xi^2-1}/(2\Gamma)}b>0}.
$$

Its radial relaxation eigenvalue is $-2\Gamma bp^2<0$. At $|\xi|=1$ the angular linearization is marginal and $p^2=-a/b$ requires $a<0$. If $g=0$, the shear restriction disappears and any orientation is allowed for $p^2=-a/b>0$. The printed request for dependence only on $a,b,\Gamma,g$ omits $\xi$: in general the magnitude necessarily depends on it.

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

At $\xi=0$, the [polar order parameter](../../../critical-phenomenon.md#polar-order-parameter) obeys

$$
\dot\theta=-\frac g2,\qquad \dot p=-\Gamma(a+bp^2)p.
$$

For $a<0$, $b>0$, the magnitude relaxes to $\sqrt{-a/b}$ while the direction rotates continuously. Thus the likely ordered behaviour is **tumbling rather than a fixed alignment**.

More generally, for $|\xi|<1$ and $g\ne0$, $\xi\cos2\theta-1$ never vanishes, so the [tumbling of a polar order parameter](../../../critical-phenomenon.md#tumbling-of-a-polar-order-parameter) persists. The [polar order parameter](../../../critical-phenomenon.md#polar-order-parameter) completes a full $2\pi$ rotation in

$$
\boxed{T_{\rm polar}=\frac{4\pi}{|g|\sqrt{1-\xi^2}}},
$$

obtained by integrating $dt=2\,|d\theta|/(|g|(1-\xi\cos2\theta))$ over a full rotation. An unoriented [nematic director](../../../critical-phenomenon.md#nematic-director) repeats after half this period, whereas a [polar order parameter](../../../critical-phenomenon.md#polar-order-parameter) distinguishes opposite directions. For $\xi\ne0$ its magnitude can also oscillate. If the [polar order parameter](../../../critical-phenomenon.md#polar-order-parameter) decays to zero, its orientation is no longer a physical observable; the tumbling conclusion concerns a persistent ordered state.

## 3

↑ **Parent:** [Paper 344](paper-344.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Take $b>0$ for a stable quartic [Landau free energy](../../../critical-phenomenon.md#landau-free-energy). The [cubic-term removal in a conserved quartic Landau free energy](../../../critical-phenomenon.md#cubic-term-removal-in-a-conserved-quartic-landau-free-energy) uses $\phi=\psi-c/(3b)$ and gives, apart from a constant,

$$
f=\frac{a'}2\psi^2+\frac b4\psi^4+d'\psi,
\qquad a'=a-\frac{c^2}{3b},
\qquad d'=d-\frac{ac}{3b}+\frac{2c^3}{27b^2}.
$$

For a closed [binary fluid mixture](../../../critical-phenomenon.md#binary-fluid-mixture), the [compositional order parameter](../../../critical-phenomenon.md#compositional-order-parameter) has fixed integral. Adding $d\int\phi$ therefore adds the same constant to every allowed state. Equivalently, in the [common-tangent construction for phase coexistence](../../../critical-phenomenon.md#common-tangent-construction-for-phase-coexistence), a linear term changes the tangent slope, hence the [chemical potential](../../../thermodynamics.md#chemical-potential), by $d$, but leaves the coexistence compositions unchanged. This is why [linear composition bias leaves coexistence compositions unchanged](../../../critical-phenomenon.md#linear-composition-bias-leaves-coexistence-compositions-unchanged); it would not mean an unchanged composition at a fixed externally imposed [chemical potential](../../../thermodynamics.md#chemical-potential).

In the shifted variable, the [binodal](../../../critical-phenomenon.md#binodal) compositions are $\psi_\pm=\pm\sqrt{-a'/b}$ for $a'<0$. They merge at

$$
\boxed{a_c=\frac{c^2}{3b},\qquad \phi_c=-\frac{c}{3b}}.
$$

The [continuous phase transition](../../../critical-phenomenon.md#continuous-phase-transition) therefore has the same scalar quartic [Landau theory](../../../critical-phenomenon.md#landau-theory) as the symmetric [binary fluid mixture](../../../critical-phenomenon.md#binary-fluid-mixture), with a shifted critical composition and control parameter. In the [mean-field approximation](../../../critical-phenomenon.md#mean-field-approximation), the composition difference vanishes with [order-parameter critical exponent](../../../critical-phenomenon.md#order-parameter-critical-exponent) $1/2$. This argument presumes the critical composition lies in the physically accessible composition range; conservation affects the dynamics, not this static [phase coexistence](../../../critical-phenomenon.md#phase-coexistence) construction.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

The [nematic order parameter](../../../critical-phenomenon.md#nematic-order-parameter) is a [symmetric second-rank tensor](../../../linear-algebra.md#symmetric-second-rank-tensor) and a [traceless second-rank tensor](../../../linear-algebra.md#traceless-second-rank-tensor) describing orientational anisotropy. For molecular unit axes $\mathbf s$, $Q_{ij}$ is proportional to $\langle s_i s_j-\delta_{ij}/3\rangle$. It vanishes in an [isotropic phase](../../../critical-phenomenon.md#isotropic-phase) and is unchanged by head-tail reversal $\mathbf s\mapsto-\mathbf s$, unlike a [polar order parameter](../../../critical-phenomenon.md#polar-order-parameter). For [uniaxial nematic order](../../../critical-phenomenon.md#uniaxial-nematic-order), the [nematic director](../../../critical-phenomenon.md#nematic-director) is thus an unoriented axis.

One convention for the [Landau-de Gennes free energy](../../../critical-phenomenon.md#landau-de-gennes-free-energy) through fourth order, respecting [rotational symmetry](../../../linear-algebra.md#rotational-symmetry), is

$$
\boxed{f(Q)=\frac a2\operatorname{Tr}Q^2
+\frac c3\operatorname{Tr}Q^3
+\frac b4(\operatorname{Tr}Q^2)^2},\qquad b>0.
$$

For a [traceless second-rank tensor](../../../linear-algebra.md#traceless-second-rank-tensor) in three dimensions, the [Cayley-Hamilton theorem](../../../mathematics.md#cayley-hamilton-theorem) gives $\operatorname{Tr}Q^4=(\operatorname{Tr}Q^2)^2/2$, so there is only one independent quartic [rotational invariant of a symmetric traceless tensor](../../../critical-phenomenon.md#rotational-invariant-of-a-symmetric-traceless-tensor). The only possible linear scalar is $\operatorname{Tr}Q=0$; without an external anisotropy no linear term survives.

The cubic [rotational invariant of a symmetric traceless tensor](../../../critical-phenomenon.md#rotational-invariant-of-a-symmetric-traceless-tensor) distinguishes prolate and oblate forms of [uniaxial nematic order](../../../critical-phenomenon.md#uniaxial-nematic-order). Head-tail reversal leaves $Q$ unchanged and does not impose $Q\mapsto-Q$. Thus a cubic term is allowed in three dimensions and generically produces a [first-order phase transition](../../../thermodynamics.md#first-order-phase-transition), rather than a symmetry-enforced continuous onset. In two dimensions a symmetric [traceless second-rank tensor](../../../linear-algebra.md#traceless-second-rank-tensor) has [eigenvalues](../../../linear-operator-theory.md#eigenvalue) $s,-s$, hence $\operatorname{Tr}Q^3=0$: **the cubic invariant vanishes identically in two dimensions**. This is a statement about the [Landau free energy](../../../critical-phenomenon.md#landau-free-energy); fluctuations in two dimensions require a separate treatment.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

For the stated [uniaxial nematic order](../../../critical-phenomenon.md#uniaxial-nematic-order) normalization, the [nematic director](../../../critical-phenomenon.md#nematic-director) is an [eigenvector](../../../linear-operator-theory.md#eigenvector) of $Q$ with [eigenvalue](../../../linear-operator-theory.md#eigenvalue) $\lambda$, and the two perpendicular [eigenvalues](../../../linear-operator-theory.md#eigenvalue) are $-\lambda/2$. Therefore

$$
\operatorname{Tr}Q^2=\frac32\lambda^2,
\qquad \operatorname{Tr}Q^3=\frac34\lambda^3,
\qquad (\operatorname{Tr}Q^2)^2=\frac94\lambda^4.
$$

Using precisely the [Landau-de Gennes free energy](../../../critical-phenomenon.md#landau-de-gennes-free-energy) convention in the preceding solution gives

$$
\boxed{\bar a=\frac{3a}{4},\qquad \bar b=\frac{9b}{16},\qquad \bar c=\frac c4}.
$$

If the quartic invariant were instead normalized as $b\operatorname{Tr}Q^4/4$, its coefficient would be $\bar b=9b/32$; the physical predictions are unchanged after redefining $b$.

For a nonzero [global minimizer](../../../analysis.md#global-minimizer) of the [free energy](../../../thermodynamics.md#thermodynamic-free-energy), compare opposite values of the scalar [nematic order parameter](../../../critical-phenomenon.md#nematic-order-parameter):

$$
f(\lambda)-f(-\lambda)=2\bar c\lambda^3.
$$

The lower one has $\bar c\lambda<0$, so

$$
\boxed{\operatorname{sgn}\lambda_{\rm eq}=-\operatorname{sgn}\bar c\quad(\bar c\ne0)}.
$$

The claim concerns the stable ordered phase, not every metastable stationary point. For $\bar c=0$ the two signs are degenerate. For $\bar c\ne0$, equality of the ordered and isotropic [free energies](../../../thermodynamics.md#thermodynamic-free-energy), together with stationarity, gives $\lambda_t=-\bar c/(2\bar b)$ and $\bar a_t=\bar c^2/(4\bar b)>0$. The finite jump $\lambda_t$ exhibits the [first-order phase transition](../../../thermodynamics.md#first-order-phase-transition) driven by the cubic invariant.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

A scalar coupling linear in the [nematic order parameter](../../../critical-phenomenon.md#nematic-order-parameter) requires a second-rank anisotropy. A single [electric field](../../../electromagnetism.md#electric-field) supplies no such tensor, while $E_iE_j$ does. Its isotropic part gives $E^2\operatorname{Tr}Q=0$. Hence the lowest joint order in $E$ and $Q$ of the [electric-field coupling to nematic order](../../../critical-phenomenon.md#electric-field-coupling-to-nematic-order) is

$$
\boxed{f_E=-\chi E_iQ_{ij}E_j}.
$$

Terms depending only on $E$ do not affect minimization over $Q$. With $\vartheta$ the angle between the [nematic director](../../../critical-phenomenon.md#nematic-director) and the [electric field](../../../electromagnetism.md#electric-field),

$$
f_E=-\frac32\chi\lambda E^2\left(\cos^2\vartheta-\frac13\right).
$$

For $\chi\lambda>0$, the lowest [free energy](../../../thermodynamics.md#thermodynamic-free-energy) occurs at $\cos^2\vartheta=1$, so the [nematic director](../../../critical-phenomenon.md#nematic-director) aligns along either $+\mathbf E$ or $-\mathbf E$. Then $E_iQ_{ij}E_j=\lambda E^2$, giving

$$
\boxed{f_E=\bar d\lambda,\qquad \bar d=-\chi E^2<0\quad(E\ne0,\ \chi>0)}.
$$

Unlike the linear composition term in a conserved [binary fluid mixture](../../../critical-phenomenon.md#binary-fluid-mixture), this term changes the equilibrium [nematic order parameter](../../../critical-phenomenon.md#nematic-order-parameter): its spatial integral is not fixed.

<h3 id="3/e">e</h3>

↑ **Parent:** [3](#3)

<h4 id="3/e/solution">Solution</h4>

↑ **Parent:** [E](#3/e)

Within this analytic quartic [Landau theory](../../../critical-phenomenon.md#landau-theory), equilibrium of a nonconserved scalar [order parameter](../../../critical-phenomenon.md#order-parameter) requires $f'=0$. At a [continuous phase transition](../../../critical-phenomenon.md#continuous-phase-transition), its restoring curvature vanishes, so $f''=0$. A nonzero $f'''$ would leave a cubic leading term in the [Taylor expansion](../../../calculus.md#taylor-expansion) about that state and prevent it from being a local minimum. Thus a stable [critical endpoint of a quartic Landau free energy](../../../critical-phenomenon.md#critical-endpoint-of-a-quartic-landau-free-energy) requires all three derivatives to vanish, with $f''''>0$. The condition $f''=0$ alone can instead identify a [spinodal point](../../../critical-phenomenon.md#spinodal-point).

For $f=\bar b\lambda^4+\bar c\lambda^3+\bar a\lambda^2+\bar d\lambda$, $\bar b>0$, the successive equations are

$$
f'''=24\bar b\lambda+6\bar c=0,
\quad f''=12\bar b\lambda^2+6\bar c\lambda+2\bar a=0,
\quad f'=4\bar b\lambda^3+3\bar c\lambda^2+2\bar a\lambda+\bar d=0.
$$

They give

$$
\boxed{\lambda_c=-\frac{\bar c}{4\bar b},
\qquad \bar a_c=\frac{3\bar c^2}{8\bar b},
\qquad \bar d_c=\frac{\bar c^3}{16\bar b^2}}.
$$

At these values, the [free energy](../../../thermodynamics.md#thermodynamic-free-energy) is exactly $f(\lambda_c)+\bar b(\lambda-\lambda_c)^4$, proving stability. With no [electric field](../../../electromagnetism.md#electric-field), $\bar d=0$, so necessarily $\bar c=0$, followed by $\lambda_c=\bar a_c=0$.

For $\bar c<0$ and $\chi>0$, the [electric-field coupling to nematic order](../../../critical-phenomenon.md#electric-field-coupling-to-nematic-order) supplies the required negative $\bar d_c$ at

$$
\boxed{E_c^2=-\frac{\bar c^3}{16\chi\bar b^2},
\qquad E_c=\frac{(-\bar c)^{3/2}}{4\sqrt\chi\,\bar b}}>0.
$$

Tuning the quadratic coefficient to $\bar a_c$ simultaneously reaches the [field-induced critical endpoint of the isotropic-nematic transition](../../../critical-phenomenon.md#field-induced-critical-endpoint-of-the-isotropic-nematic-transition). The PDF's $\tilde c$ in the last clause is undefined; it is interpreted here as the previously defined $\bar c$. The endpoint is a prediction of the stable quartic, small-field [mean-field approximation](../../../critical-phenomenon.md#mean-field-approximation); higher-order terms or a field beyond the expansion's validity can shift it.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2018](../../2018.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
