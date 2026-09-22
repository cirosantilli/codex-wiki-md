# Paper 44

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2013/paper_44.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2013/paper_44.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
  - [i](#3/i)
    - [Solution](#3/i/solution)
  - [ii](#3/ii)
    - [Solution](#3/ii/solution)
- [4](#4)
  - [Solution](#4/solution)

## 1

↑ **Parent:** [Paper 44](paper-44.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Write $z=z_c+\eta$, with $\eta(0)=\eta(T)=0$. Independent variations of $z$ and $z^*$ give the [Euler-Lagrange equation](../../../analysis.md#euler-lagrange-equation) $\ddot z_c+\omega^2z_c=0$. Away from $\sin\omega T=0$ its unique endpoint solution is

$$
z_c(t)=\frac{z_i\sin\omega(T-t)+z_f\sin\omega t}{\sin\omega T}.
$$

[Integration by parts](../../../calculus.md#integration-by-parts) cancels the linear fluctuation terms and gives $S[z]=S[z_c]+\int_0^T\eta^*\Delta_\omega\eta\,dt$. On the [classical solution](../../../partial-differential-equation.md#classical-solution), the [action](../../../classical-mechanics.md#action) is the boundary term $[z_c^*\dot z_c]_0^T$. Substituting the endpoint derivatives therefore gives

$$
S[z_c]=\frac{\omega}{\sin\omega T}\bigl[(|z_f|^2+|z_i|^2)\cos\omega T-z_f^*z_i-z_i^*z_f\bigr].
$$

The remaining [Gaussian path integral](../../../quantum-field-theory.md#gaussian-path-integral) contains two real fluctuation coordinates per mode, so it contributes an inverse [functional determinant](../../../quantum-field-theory.md#functional-determinant), rather than its inverse square root. Thus $K=e^{iS[z_c]}/\det\Delta_\omega$, with the measure normalization fixing the otherwise arbitrary constant.

For [Dirichlet boundary conditions](../../../differential-equation.md#dirichlet-boundary-condition), the normalized sine modes have [eigenvalues](../../../linear-operator-theory.md#eigenvalue) $\lambda_j=(\pi j/T)^2-\omega^2$, $j\ge1$. Their [determinant](../../../linear-algebra.md#determinant) ratio is the convergent [Dirichlet oscillator determinant ratio](../../../quantum-field-theory.md#dirichlet-oscillator-determinant-ratio)

$$
\frac{\det\Delta_\omega}{\det\Delta_0}
=\prod_{j\ge1}\left(1-\frac{\omega^2T^2}{\pi^2j^2}\right)
=\frac{\sin\omega T}{\omega T}.
$$

The last equality is the [sine infinite product](../../../geometry-and-topology.md#sine-infinite-product). With the prescribed free [determinant](../../../linear-algebra.md#determinant) this gives

$$
\boxed{\det\Delta_\omega=\frac{\pi i\sin\omega T}{\omega},\qquad K(z_f,z_i;T)=\frac{\omega}{\pi i\sin\omega T}e^{iS[z_c]}.}
$$

The kernel uses the [Feynman i-epsilon prescription](../../../quantum-field-theory.md#feynman-i-epsilon-prescription); at a caustic it is a distributional limit, not an ordinary finite function. Its $\omega\to0$ limit is $(\pi iT)^{-1}\exp(i|z_f-z_i|^2/T)$.

There is a sign error in the printed complex-integral hint. For a positive damping parameter $\alpha$, polar integration gives the [regulated complex Fresnel integral](../../../analysis.md#regulated-complex-fresnel-integral)

$$
\int_{\mathbb C}e^{(i\lambda-\alpha)|z|^2}\,d^2z=\frac{\pi}{\alpha-i\lambda}\longrightarrow\frac{i\pi}{\lambda}=-\frac{\pi}{i\lambda}.
$$

This regulated value, together with the stated free-kernel normalization, fixes the phase consistently.

For $\omega>0$ and positive imaginary-time length $\beta$, [Wick rotation](../../../perturbative-quantum-field-theory.md#wick-rotation) gives

$$
K_E(z_f,z_i;\beta)=\frac{\omega}{\pi\sinh\omega\beta}\exp\left[-\frac{\omega}{\sinh\omega\beta}\bigl((|z_f|^2+|z_i|^2)\cosh\omega\beta-z_f^*z_i-z_i^*z_f\bigr)\right].
$$

Put $z_f=sz_i$ with $s=\pm1$ and use the convergent real [Gaussian integral](../../../calculus.md#gaussian-integral). Writing $r=e^{-\omega\beta}$ gives

$$
\int d^2z\,K_E(sz,z;\beta)=\frac1{2(\cosh\omega\beta-s)}=\frac r{(1-sr)^2}=\sum_{n\ge1}s^{n-1}nr^n.
$$

This is the [parity-twisted oscillator thermal trace](../../../statistical-physics.md#parity-twisted-oscillator-thermal-trace). The complex coordinate describes two independent real [quantum harmonic oscillators](../../../quantum-mechanics.md#quantum-harmonic-oscillator), each with mass two in these units. Their total energy is $E=\omega(n_x+n_y+1)$; level $n\omega$ has degeneracy $n$, and spatial inversion has [parity operator](../../../quantum-mechanics.md#parity-operator) [eigenvalue](../../../linear-operator-theory.md#eigenvalue) $(-1)^{n_x+n_y}=(-1)^{n-1}$. The plus sign is $\operatorname{Tr}e^{-\beta H}$; the minus sign is $\operatorname{Tr}(Pe^{-\beta H})$. The alternating [trace](../../../linear-algebra.md#matrix-trace) inserts parity into a bosonic system; it does not change the oscillators into fermions.

## 2

↑ **Parent:** [Paper 44](paper-44.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

Normalize the vacuum [path integral](../../../quantum-field-theory.md#path-integral) by $Z[0]$. The scalar [two-point correlation function](../../../critical-phenomenon.md#two-point-correlation-function) is $Z[0]^{-1}\int\mathcal D\phi\,\phi(x)\phi(0)e^{iS_F}$, and the spinor [two-point correlation function](../../../critical-phenomenon.md#two-point-correlation-function) is $Z[0]^{-1}\int\mathcal D\psi\mathcal D\bar\psi\,\psi(x)\bar\psi(0)e^{iS_F}$. Vacuum boundary conditions make these time-ordered [Feynman propagators](../../../quantum-field-theory.md#feynman-propagator). After [integration by parts](../../../calculus.md#integration-by-parts), the scalar quadratic [action](../../../classical-mechanics.md#action) is $-\frac12\int\phi(-\partial^2+m^2)\phi$.

The [Schwinger-Dyson equation](../../../perturbative-quantum-field-theory.md#schwinger-dyson-equation) follows by integrating a [functional derivative](../../../calculus-of-variations.md#functional-derivative) of $\phi(0)e^{iS_F}$: the derivative of the insertion supplies $\delta^d(x)$, and the [action](../../../classical-mechanics.md#action) derivative supplies the kinetic operator. The analogous [left Grassmann derivative](../../../linear-algebra.md#left-grassmann-derivative) calculation, or differentiation of the [Grassmann Gaussian integral](../../../quantum-field-theory.md#grassmann-gaussian-integral), gives

$$
(-\partial^2+m^2)G_\phi(x)=-i\delta^d(x),\qquad(\gamma^\mu\partial_\mu+M)G_\psi(x)=-i\delta^d(x).
$$

Using $\partial_\mu\mapsto ip_\mu$ and the [Clifford algebra](../../../algebra.md#clifford-algebra), $(i\gamma\cdot p+M)(-i\gamma\cdot p+M)=p^2+M^2$. Consequently

$$
\boxed{G_\phi(p)=\frac{-i}{p^2+m^2-i0},\qquad G_\psi(p)=\frac{-i(-i\gamma\cdot p+M)}{p^2+M^2-i0}.}
$$

The free [quantum effective action](../../../perturbative-quantum-field-theory.md#effective-action) is quadratic, so all scalar [one-particle-irreducible vertices](../../../perturbative-quantum-field-theory.md#one-particle-irreducible-vertex) with $n>2$ vanish. Its two-point vertex is the stated inverse kinetic form $-p^2-m^2$.

For the [Yukawa interaction](../../../standard-model.md#yukawa-interaction), two vertices contribute $(-iy)^2$, and a closed [fermion loop](../../../perturbative-quantum-field-theory.md#fermion-loop) contributes an extra minus sign. Tracing the two spinor numerators gives $4[M^2-k\cdot(k-p)]$, since the one-gamma traces vanish. Removing the overall $i$ from the amplitude gives the displayed loop integral. Define

$$
I(M)=\frac1{(2\pi)^di}\int\frac{d^dk}{k^2+M^2-i0},\quad
J(p;M)=\frac1{(2\pi)^di}\int\frac{d^dk}{(k^2+M^2-i0)((k-p)^2+M^2-i0)}.
$$

The numerator decomposition and translation invariance of [dimensional regularization](../../../perturbative-quantum-field-theory.md#dimensional-regularization) reduce it to

$$
\widehat\tau_2^{(1)}=-4y^2\left[\left(2M^2+\frac{p^2}2\right)J(p;M)-I(M)\right].
$$

The supplied tadpole [pole](../../../isolated-singularity.md#pole) is $I(M)\sim-2M^2/(\varepsilon16\pi^2)$. A [Feynman parameter](../../../perturbative-quantum-field-theory.md#feynman-parameter) combines the two bubble denominators. Shifting its loop momentum gives mass squared $M^2+x(1-x)p^2$; differentiating the tadpole integral with respect to this squared mass gives the double-denominator [pole](../../../isolated-singularity.md#pole) $2/(\varepsilon16\pi^2)$, independent of $x$. Thus $J(p;M)\sim2/(\varepsilon16\pi^2)$ and

$$
\boxed{\widehat\tau_2^{(1)}\sim-\frac{y^2}{\varepsilon16\pi^2}(4p^2+24M^2),\qquad a=4,\quad b=24.}
$$

The [counterterms](../../../perturbative-quantum-field-theory.md#counterterm) contribute $-Ap^2-B$, so their minimal [pole](../../../isolated-singularity.md#pole) parts are

$$
A=-\frac{4y^2}{\varepsilon16\pi^2},\qquad B=-\frac{24y^2M^2}{\varepsilon16\pi^2}.
$$

Combining the kinetic terms gives [wavefunction renormalization](../../../perturbative-quantum-field-theory.md#wave-function-renormalization) $Z_\phi=1+A$, and combining the mass terms gives $Z_\phi m_0^2=m^2+B$. Therefore

$$
\boxed{Z_\phi=1-\frac{4y^2}{\varepsilon16\pi^2},\qquad m_0^2=\frac{m^2+B}{Z_\phi}.}
$$

These are the [Yukawa scalar self-energy pole coefficients](../../../standard-model.md#yukawa-scalar-self-energy-pole-coefficients); finite parts depend on the chosen [renormalization condition](../../../perturbative-quantum-field-theory.md#renormalization-condition).

The four-point graph is a [Yukawa fermion box](../../../perturbative-quantum-field-theory.md#yukawa-fermion-box), with four external scalar legs attached to a closed spinor loop:

<a id="2/image-fermion-box-with-four-external-scalar-legs-in-a-yukawa-theory"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-44-yukawa-box.png)

**[Figure 1](#2/image-fermion-box-with-four-external-scalar-legs-in-a-yukawa-theory). Fermion box with four external scalar legs in a Yukawa theory**.

Each high-momentum [dirac propagator](../../../quantum-field-theory.md#dirac-propagator) is $O(k^{-1})$. The product of four is $O(k^{-4})$, and the leading [gamma matrix trace identities](../../../algebra.md#gamma-matrix-trace-identities) is nonzero. The four-dimensional radial integral therefore contains $\int^\infty dk/k$: a logarithmic [ultraviolet divergence](../../../perturbative-quantum-field-theory.md#ultraviolet-divergence). This local four-scalar divergence cannot be absorbed by scalar mass or field normalization. Add $-\lambda\phi^4/4!$, and, using the stipulated four-point [pole](../../../isolated-singularity.md#pole) normalization, take $\delta\lambda=-8y^4/(\varepsilon16\pi^2)$ so that $-\delta\lambda$ cancels it.

For literal cancellation of every one-loop divergence with $M\ne0$, [counterterm closure of a massive Yukawa theory](../../../perturbative-quantum-field-theory.md#counterterm-closure-of-a-massive-yukawa-theory) also requires the allowed scalar linear and cubic terms. A constant scalar background shifts the fermion mass to $M+y\phi$; the divergent local fermion contribution contains a polynomial proportional to $(M+y\phi)^4$. Its linear and cubic terms are not forbidden by a symmetry when the fermion mass is nonzero. A closed renormalizable family therefore has

$$
\mathcal L=-\frac12(\partial\phi)^2-\bar\psi(\gamma\cdot\partial+M)\psi-y\bar\psi\psi\phi-V(\phi),\qquad
V(\phi)=\Lambda+h\phi+\frac{m^2}2\phi^2+\frac{\kappa}{3!}\phi^3+\frac\lambda{4!}\phi^4,
$$

with field, mass and coupling redefinitions for both scalar and spinor fields. A tadpole condition can set the renormalized $h$ to zero, but its [counterterm](../../../perturbative-quantum-field-theory.md#counterterm) still exists. The vacuum constant is needed if vacuum energy is retained. If an exact discrete chiral symmetry is imposed with $M=0$, the scalar potential can be even and the odd terms are forbidden; the essential new interaction is then the quartic one.

## 3

↑ **Parent:** [Paper 44](paper-44.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

A regulator and a [renormalization condition](../../../perturbative-quantum-field-theory.md#renormalization-condition) introduce the reference mass scale $\mu$, even when the classical theory has no mass. Loop amplitudes contain dimensionless logarithms of momentum or distance ratios involving $\mu$. The resulting [running coupling](../../../perturbative-quantum-field-theory.md#running-coupling) and field normalization compensate changes of this arbitrary reference scale.

Let $\phi_0=Z_\phi^{1/2}\phi$ and $G_n=Z_\phi^{-n/2}G_{n,0}$. Hold the bare parameters fixed and define $\beta(g)=\mu\,dg/d\mu$ and $\gamma(g)=\frac12\mu\,d\log Z_\phi/d\mu$. Assuming multiplicative field [renormalization](../../../perturbative-quantum-field-theory.md#renormalization) and no mixing or additive contact terms for the correlator, differentiating gives the [Callan-Symanzik equation](../../../perturbative-quantum-field-theory.md#callan-symanzik-equation)

$$
\boxed{(\mu\partial_\mu+\beta(g)\partial_g+n\gamma(g))G_n=0.}
$$

For the dimensionless two-point factor put $r=p^2/\mu^2$. Its equation is $(-2r\partial_r+\beta\partial_g+2\gamma)C=0$. Let

$$
\frac{dg(t)}{dt}=\beta(g(t)),\quad g(0)=g,\qquad f(t)=\exp\left(2\int_0^t\gamma(g(u))\,du\right).
$$

The [characteristic solution of the multiplicative Callan-Symanzik equation](../../../perturbative-quantum-field-theory.md#characteristic-solution-of-the-multiplicative-callan-symanzik-equation) is

$$
\boxed{C(e^{2t}r,g)=f(t)C(r,g(t)).}
$$

To check the sign, $\partial_tC(e^{2t}r,g)=2e^{2t}r\partial_rC$ equals $(\beta\partial_g+2\gamma)C$. The characteristic flow and its accumulated multiplier give precisely this evolution. Changing $\mu$ changes the dimensionless momentum and renormalized $g$; the same bare [two-point correlation function](../../../critical-phenomenon.md#two-point-correlation-function) is recovered after the compensating field normalization. An unnormalized renormalized correlator need not remain numerically identical under that change, but physical predictions do.

With a mass, write $v=m/\mu$ and define its [running mass](../../../perturbative-quantum-field-theory.md#running-mass) by $m'(t)=\delta(g(t))m(t)$, $m(0)=m$. The dimensionless equation becomes

$$
[-2r\partial_r+\beta\partial_g+(\delta-1)v\partial_v+2\gamma]C=0.
$$

Its flow is therefore

$$
\boxed{C(e^{2t}r,m/\mu,g)=f(t)C(r,e^{-t}m(t)/\mu,g(t)),\quad m(t)=m\exp\left(\int_0^t\delta(g(u))\,du\right).}
$$

The [renormalization-group mass suppression criterion](../../../perturbative-quantum-field-theory.md#renormalization-group-mass-suppression-criterion) is $\int_0^t(\delta(g(u))-1)du\to-\infty$, for example an eventual bound $\delta\le1-\eta$ with $\eta>0$. Then the mass argument on the right tends to zero. A regular [massless limit](../../../quantum-field-theory.md#massless-limit), uniform along the limiting coupling trajectory, makes the mass negligible at high energies. Merely calling $\delta$ small without controlling this integrated exponent is insufficient.

<h3 id="3/i">i</h3>

↑ **Parent:** [3](#3)

<h4 id="3/i/solution">Solution</h4>

↑ **Parent:** [I](#3/i)

For $0<g<g_*$, the positive [beta function](../../../complex-analysis.md#beta-function) makes the [running coupling](../../../perturbative-quantum-field-theory.md#running-coupling) increase toward the [ultraviolet fixed point](../../../critical-phenomenon.md#ultraviolet-fixed-point) $g_*$. Assume a continuous locally Lipschitz [beta function](../../../complex-analysis.md#beta-function), a continuous [anomalous dimension](../../../critical-phenomenon.md#anomalous-dimension) at the fixed point, and a finite nonzero reference value $C(r,g_*)$. Then $g(t)\to g_*$ and

$$
\log f(t)=2\gamma(g_*)t+o(t),\qquad C(e^{2t}r,g)=e^{2\gamma(g_*)t+o(t)}C(r,g_*).
$$

Thus the high-momentum factor has exponent $\gamma(g_*)$ in $p^2$, and the propagator scales as $(p^2)^{-1+\gamma(g_*)}$ up to slower corrections. If the fixed point is simple and attractive, $\beta'(g_*)<0$, the approach is exponential; suitable smoothness then gives $f(t)\sim A e^{2\gamma(g_*)t}$ with finite $A$. The stated beta-function information alone supplies no numerical value for the [anomalous dimension](../../../critical-phenomenon.md#anomalous-dimension) and does not exclude slower corrections at a nonsimple fixed point. This is [two-point scaling at an ultraviolet fixed point](../../../critical-phenomenon.md#two-point-scaling-at-an-ultraviolet-fixed-point).

<h3 id="3/ii">ii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#3/ii)

For the asymptotically free [beta function](../../../complex-analysis.md#beta-function), separation of variables gives

$$
\boxed{g(t)=\frac{g}{\sqrt{1+2bg^2t}}.}
$$

The anomalous-dimension integral is elementary:

$$
\log f(t)=2c\int_0^t\frac{g^2}{1+2bg^2u}\,du=\frac cb\log(1+2bg^2t),\qquad
\boxed{f(t)=(1+2bg^2t)^{c/b}\sim(2bg^2)^{c/b}t^{c/b}.}
$$

For a reference two-point factor regular and nonzero at the free coupling, $C(r,g(t))\to C(r,0)$, so the large-momentum correction is a power $c/b$ of $\log(p^2/\mu^2)$. These are [asymptotic freedom](../../../perturbative-quantum-field-theory.md#asymptotic-freedom) and [logarithmic two-point scaling from a cubic beta function](../../../perturbative-quantum-field-theory.md#logarithmic-two-point-scaling-from-a-cubic-beta-function). If the supplied beta and gamma expressions are leading small-coupling terms rather than exact functions, they fix the leading logarithmic exponent, while subleading corrections and the prefactor depend on higher orders.

## 4

↑ **Parent:** [Paper 44](paper-44.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

Fix the current sign convention by defining the localized variation as $\delta_\epsilon S=-\int d^dx\,(\partial_\mu\epsilon^a)j_a^\mu$. For a first-derivative Lagrangian invariant without a boundary term under constant parameters, this means $j_a^\mu=-\partial\mathcal L/\partial(\partial_\mu\phi)\,t_a\phi$; include the usual improvement term if the constant variation is a total derivative. On solutions, arbitrary compactly supported parameters imply $\partial_\mu j_a^\mu=0$. The [Noether charge](../../../quantum-field-theory.md#noether-charge) is $Q_a=\int d^{d-1}x\,j_a^0$ and is conserved if the spatial flux vanishes. This sign convention matches the printed [Ward identity](../../../perturbative-quantum-field-theory.md#ward-identity); reversing the current also reverses the corresponding generator convention.

Assume an invariant regulated [functional measure](../../../quantum-field-theory.md#functional-measure), invariant vacuum boundary conditions and no [quantum anomaly](../../../relativistic-quantum-field.md#anomaly-physics). Changing variables in the normalized [path integral](../../../quantum-field-theory.md#path-integral) gives $0=\langle\delta_\epsilon X\rangle+i\langle X\delta_\epsilon S\rangle$. Integration by parts then yields

$$
-i\int d^dx\,\epsilon^a(x)\partial_\mu\langle j_a^\mu(x)X\rangle=\langle\delta_\epsilon X\rangle.
$$

For a product of [scalar fields](../../../quantum-field-theory.md#scalar-field), the local [Ward identity contact terms](../../../perturbative-quantum-field-theory.md#ward-identity-contact-terms) are

$$
\boxed{-i\partial_\mu\langle j_a^\mu(x)\phi(x_1)\cdots\phi(x_n)\rangle
=\sum_{r=1}^n\delta^d(x-x_r)\langle\phi(x_1)\cdots(t_a\phi)(x_r)\cdots\phi(x_n)\rangle.}
$$

Away from the insertions this is current conservation. Time-ordering or the distributional functional identity supplies the contact terms.

For the gauge theory write $[X,Y]^a=f^{abc}X^bY^c$ and use the [left-acting BRST differential](../../../relativistic-quantum-field.md#left-acting-brst-differential) $s$, with $\delta_\epsilon=\epsilon s$. It obeys the [graded Leibniz rule](../../../commutative-algebra.md#graded-leibniz-rule) and

$$
sA_\mu=D_\mu c,\quad sc=-\tfrac12[c,c],\quad s\bar c=b,\quad sb=0.
$$

Assume the structure constants satisfy the [Jacobi identity](../../../lie-algebra.md#jacobi-identity) and the dot product is invariant; antisymmetry alone would not be enough. Since $c$ and $D_\mu c$ are odd, their [Lie brackets](../../../lie-algebra.md#lie-bracket) are symmetric in these two arguments. Consequently

$$
s(D_\mu c)=D_\mu(sc)+[sA_\mu,c]
=-\tfrac12D_\mu[c,c]+[D_\mu c,c]=0.
$$

Also $sF_{\mu\nu}=D_\mu D_\nu c-D_\nu D_\mu c=[F_{\mu\nu},c]$. The [graded Jacobi identity](../../../lie-algebra.md#graded-jacobi-identity) gives $s[c,c]=0$, so $s^2c=0$; the other three fields have zero second variation immediately. For independent odd parameters, $\delta_{\epsilon'}\delta_\epsilon=-\epsilon'\epsilon s^2=0$. These are off-shell [BRST nilpotence](../../../relativistic-quantum-field.md#brst-nilpotence) identities because the [Nakanishi-Lautrup field](../../../relativistic-quantum-field.md#nakanishi-lautrup-field) $b$ is retained.

The [Yang-Mills theory](../../../relativistic-quantum-field.md#yang-mills-theory) variation is proportional to $F^{\mu\nu}\cdot[F_{\mu\nu},c]=0$. The gauge-fixing variation is $(\partial^\mu b)\cdot D_\mu c$, while the ghost variation is its negative; the $b^2$ term does not vary. Equivalently these terms are $s\Psi$ for the [gauge-fixing fermion](../../../relativistic-quantum-field.md#gauge-fixing-fermion) $\Psi=(\partial^\mu\bar c)\cdot A_\mu+\xi\bar c\cdot b/2$. [BRST nilpotence](../../../relativistic-quantum-field.md#brst-nilpotence) makes this expression invariant. Ghost-number scaling also leaves every term invariant: the ghost and antighost factors carry opposite weights.

Here are the two explicit currents in the same sign convention as the Ward identity. Localizing the even ghost parameter gives coefficient $(\partial_\mu\theta)[\bar c\cdot D^\mu c-(\partial^\mu\bar c)\cdot c]$. Localizing the odd parameter, keeping it on the left, gives coefficient

$$
(\partial_\mu\epsilon)\left[-F^{\mu\nu}\cdot D_\nu c-b\cdot D^\mu c-\frac12(\partial^\mu\bar c)\cdot[c,c]\right].
$$

The last sign comes from moving the odd parameter through the odd antighost derivative. Since the current was defined as minus this coefficient,

$$
\boxed{j_G^\mu=(\partial^\mu\bar c)\cdot c-\bar c\cdot D^\mu c,\qquad
j_B^\mu=F^{\mu\nu}\cdot D_\nu c+b\cdot D^\mu c+\frac12(\partial^\mu\bar c)\cdot[c,c].}
$$

These are the [ghost-number Noether current](../../../relativistic-quantum-field.md#ghost-number-noether-current) and the [BRST current in derivative-b gauge fixing](../../../relativistic-quantum-field.md#brst-current-in-derivative-b-gauge-fixing). If the opposite Noether sign is used, both displayed currents acquire an overall minus sign. Integrating the gauge-fixing term by parts changes the Noether representative by the associated boundary improvement; mixing the two Lagrangian conventions without that improvement gives incorrect signs.

With no BRST anomaly, the conserved odd [BRST charge](../../../relativistic-quantum-field.md#brst-charge) has $Q_B^2=0$. The [BRST cohomology](../../../relativistic-quantum-field.md#brst-cohomology) identifies closed states $Q_B|\psi\rangle=0$ modulo exact states $Q_B|\chi\rangle$. Nilpotence puts every exact state in the closed space. In the usual indefinite gauge-fixed state space, a Hermitian BRST charge makes exact states orthogonal to closed states; the standard no-ghost/positivity assumptions then give a physical [inner product](../../../linear-algebra.md#inner-product) on the quotient. The physical sector is its ghost-number-zero component,

$$
\boxed{\mathcal H_{\mathrm{phys}}=H^0(Q_B)=\frac{\ker Q_B\cap\mathcal H^0}{Q_B\mathcal H^{-1}}.}
$$

The [ghost number](../../../relativistic-quantum-field.md#ghost-number) assigns $+1$ to $c$, $-1$ to $\bar c$ and zero to gauge and auxiliary fields. Gauge-invariant observables and the chosen vacuum have [ghost number](../../../relativistic-quantum-field.md#ghost-number) zero; unphysical ghost excitations are removed in BRST pairs. Thus physical representatives are expected to satisfy $Q_G|\psi\rangle=0$. This zero-grading selection is part of the physical-state prescription, not a consequence of nilpotence alone.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2013](../../2013.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
