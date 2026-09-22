# Paper 51

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2008/Paper51.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2008/Paper51.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)

## 1

↑ **Parent:** [Paper 51](paper-51.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Use units $\hbar=1$. The fluctuations about a [classical path](../../../quantum-field-theory.md#classical-path) satisfy $f(0)=f(T)=0$. Expanding the [action functional](../../../classical-mechanics.md#action) and integrating the term $m\dot q_c\dot f$ by parts gives

$$
S[q_c+f]=S[q_c]+\int_0^T(-m\ddot q_c-V^{\prime}(q_c))f\,dt+\frac12\int_0^T\{m\dot f^2-V^{\prime\prime}(q_c)f^2\}\,dt+O(f^3).
$$

The linear term vanishes by the [Euler-Lagrange equation](../../../analysis.md#euler-lagrange-equation) and the endpoint conditions. Integrating the quadratic [kinetic term](../../../quantum-field-theory.md#kinetic-term) by parts yields the [Dirichlet fluctuation determinant of a semiclassical propagator](../../../quantum-mechanics.md#dirichlet-fluctuation-determinant-of-a-semiclassical-propagator):

$$
\mathcal O_c=-m\frac{d^2}{dt^2}-V^{\prime\prime}(q_c(t)),\qquad K(q_1,q_0;T)\simeq e^{iS[q_c]}\int\mathcal Df\,\exp\left(\frac i2\int f\mathcal O_cf\,dt\right).
$$

A finite time-slicing first turns this into a product of ordinary [Gaussian integrals](../../../calculus.md#gaussian-integral), whose limit is proportional to $(\det\mathcal O_c)^{-1/2}$. A useful normalization relative to the free operator $\mathcal O_0=-m\,d^2/dt^2$ is

$$
D_c=\left(\frac{m}{2\pi iT}\right)^{1/2}\left(\frac{\det\mathcal O_c}{\det\mathcal O_0}\right)^{-1/2}.
$$

The oscillatory square root is fixed by the short-time limit and the [Feynman i-epsilon prescription](../../../quantum-field-theory.md#feynman-i-epsilon-prescription). Away from [zero modes](../../../linear-operator-theory.md#zero-mode) this gives the [semiclassical propagator](../../../quantum-mechanics.md#semiclassical-propagator); if several [classical paths](../../../quantum-field-theory.md#classical-path) contribute, their saddle contributions are summed with their corresponding determinant phases.

**For a general potential the prefactor depends on the endpoints through $q_c$; writing only $D(T)$ suppresses that dependence.** If $V(q)=aq^2/2+bq+c$, the Taylor expansion has no terms beyond quadratic and $V^{\prime\prime}=a$ is independent of $q_c$. The [Gaussian functional integral](../../../quantum-field-theory.md#gaussian-functional-integral) is then exact, and its prefactor genuinely depends only on $T$ and the potential parameters. Singular focusing times are understood by continuation of the kernel, rather than by assigning a finite value to a zero-mode determinant.

For the [free-particle propagator](../../../quantum-mechanics.md#free-particle-propagator), $q_c(t)=q_0+(q_1-q_0)t/T$ and $S_c=m(q_1-q_0)^2/(2T)$. The free determinant supplies the factor $\sqrt{m/(2\pi iT)}$. Its normalization can also be checked by the momentum-space representation

$$
K_0=\int\frac{dp}{2\pi}\exp\left\{ip(q_1-q_0)-\frac{iTp^2}{2m}\right\}=\sqrt{\frac{m}{2\pi iT}}\exp\left\{\frac{im(q_1-q_0)^2}{2T}\right\},
$$

where completing the square evaluates the [Gaussian integral](../../../calculus.md#gaussian-integral) and the short-time limit gives the position-space delta function.

For the gravitational potential, the original PDF contains $-mgq$; the TeX aid drops the final $q$. The [Euler-Lagrange equation](../../../analysis.md#euler-lagrange-equation) is $\ddot q_c=g$, and its endpoint solution is

$$
q_c(t)=q_0+\left(\frac{q_1-q_0}{T}-\frac{gT}{2}\right)t+\frac12gt^2.
$$

Substitution into the kinetic and potential terms gives

$$
S_c=\frac{m(q_1-q_0)^2}{2T}+\frac{mgT}{2}(q_1+q_0)-\frac{mg^2T^3}{24}.
$$

Since $V^{\prime\prime}=0$, the fluctuation operator is the free one. Thus the [quantum-mechanical propagator in a constant force](../../../quantum-mechanics.md#quantum-mechanical-propagator-in-a-constant-force) is exactly

$$
\boxed{K_g(q_1,q_0;T)=\sqrt{\frac{m}{2\pi iT}}\exp\left[i\left\{\frac{m(q_1-q_0)^2}{2T}+\frac{mgT}{2}(q_1+q_0)-\frac{mg^2T^3}{24}\right\}\right].}
$$

The [quantum-mechanical propagator](../../../quantum-mechanics.md#quantum-mechanical-propagator) is $\langle q_1|e^{-iHT}|q_0\rangle$, with [Hamiltonian operator](../../../quantum-mechanics.md#hamiltonian-quantum-mechanics) $H=-\partial_q^2/(2m)+V(q)$. For imaginary time $-i\tau$, insert an orthonormal complete set of [energy eigenstates](../../../quantum-mechanics.md#energy-eigenstate) to obtain

$$
\boxed{K(q_1,q_0;-i\tau)=\sum_n e^{-\tau E_n}\psi_n(q_1)\psi_n(q_0)^*,\qquad\tau>0.}
$$

Here $\psi_n(q)=\langle q|n\rangle$. This discrete sum assumes a discrete complete spectrum; continuous spectral components require the corresponding spectral integral. The heat-semigroup expression is well defined for an appropriate [self-adjoint](../../../linear-operator-theory.md#self-adjoint-operator) Hamiltonian bounded below. It is this spectral condition, not an unrestricted formal rotation for every conceivable potential, that justifies the imaginary-time kernel.

A path on the circle lifts to a path on the real line ending at $q_1+2\pi w$, where the integer $w$ is its [winding number](../../../complex-analysis.md#winding-number). The periodic quantum theory sums all these winding sectors with equal weight, giving the [real-time winding representation of a quantum rotor kernel](../../../quantum-mechanics.md#real-time-winding-representation-of-a-quantum-rotor-kernel). For imaginary time, put $x=q_1-q_0$ and $y=\tau/m$ in the supplied Gaussian summation identity:

$$
K_{S^1}(q_1,q_0;-i\tau)=\sqrt{\frac{m}{2\pi\tau}}\sum_{w\in\mathbb Z}e^{-m(x+2\pi w)^2/(2\tau)}=\frac1{2\pi}\sum_{n\in\mathbb Z}e^{-\tau n^2/(2m)+inx}.
$$

Comparison with the spectral expansion determines

$$
\boxed{E_n=\frac{n^2}{2m},\qquad\psi_n(q)=\frac{e^{inq}}{\sqrt{2\pi}},\qquad n\in\mathbb Z.}
$$

The normalization uses $0\le q<2\pi$. The ground state is nondegenerate; levels with $n\ne0$ have the degeneracy $n\leftrightarrow-n$. Returning to real time replaces $e^{-\tau E_n}$ by $e^{-iTE_n}$, with the usual limiting prescription. No twisted boundary condition or flux phase is present in the stated image sum.

## 2

↑ **Parent:** [Paper 51](paper-51.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

Write $\varepsilon=\varepsilon_a t_a$ and $A_\mu=A_{\mu a}t_a$. The proposed [gauge-field transformation law](../../../relativistic-quantum-field.md#gauge-field-transformation-law) becomes $\delta A_\mu=-\partial_\mu\varepsilon+[\varepsilon,A_\mu]$. Consequently

$$
\delta(D_\mu\phi)=\varepsilon\partial_\mu\phi+(\partial_\mu\varepsilon)\phi+\delta A_\mu\phi+A_\mu\varepsilon\phi=\varepsilon D_\mu\phi.
$$

Both $\phi$ and its [gauge covariant derivative](../../../relativistic-quantum-field.md#gauge-covariant-derivative) therefore transform as the same multiplet, with no derivative of the local parameter left over. The original algebraic invariance of the [Lagrangian density](../../../quantum-field-theory.md#lagrangian-density) now applies pointwise to $\mathcal L(\phi,D\phi)$, so this constructs the local symmetry.

Also transform $J$ by $\delta J=\varepsilon J$. Antisymmetry gives $(t_aJ)\cdot\phi+J\cdot(t_a\phi)=0$, so the [source](../../../perturbative-quantum-field-theory.md#source-quantum-field-theory) coupling is invariant. Let $S_{A_{\mu a}}$ denote the [functional derivative](../../../calculus-of-variations.md#functional-derivative) at a point. Vary the [action functional](../../../classical-mechanics.md#action) and integrate the derivative of $\varepsilon_a$ by parts, taking the local parameter to have compact support:

$$
\delta S=\int d^dx\,\varepsilon_a\left[(t_a\phi)\cdot S_\phi+(t_aJ)\cdot S_J+\partial_\mu S_{A_{\mu a}}+f_{abc}A_{\mu b}S_{A_{\mu c}}\right].
$$

Since every $\varepsilon_a(x)$ is arbitrary, its coefficient vanishes. This proves the requested local identity, including the derivative sign and the order of the structure-constant indices.

For the [generating functional](../../../perturbative-quantum-field-theory.md#generating-functional), the integral of the first term is zero as a change-of-variable identity:

$$
\int\mathcal D\phi\,(t_a\phi)\cdot\frac{\delta}{\delta\phi}e^{iS}=0.
$$

The divergence of this vector field in field space is proportional to $\operatorname{tr}t_a=0$. Thus an invariant regulated [functional measure](../../../quantum-field-theory.md#functional-measure), with no [gauge anomaly](../../../relativistic-quantum-field.md#gauge-anomaly), leaves no Jacobian term. Inserting the classical identity into the integral gives

$$
\boxed{\left[(t_aJ)\cdot\frac{\delta}{\delta J}+\partial_\mu\frac{\delta}{\delta A_{\mu a}}+f_{abc}A_{\mu b}\frac{\delta}{\delta A_{\mu c}}\right]Z[J,A]=0.}
$$

The same first-order differential operator annihilates the [connected generating functional](../../../perturbative-quantum-field-theory.md#connected-generating-functional) $W$, because $Z=e^{iW}$. Its [source](../../../perturbative-quantum-field-theory.md#source-quantum-field-theory) term is $(t_aJ)\cdot\varphi$.

For the specified [Legendre transform](../../../convex-optimization.md#convex-conjugate), vary $\Gamma=-W+\int J\varphi$. Since $W_J=\varphi$, the terms involving $\delta J$ cancel, leaving

$$
\delta\Gamma=\int J\cdot\delta\varphi-\int W_A\,\delta A,\qquad \Gamma_\varphi=J,\qquad \left.\Gamma_A\right|_\varphi=-\left.W_A\right|_J.
$$

Antisymmetry also gives $(t_aJ)\cdot\varphi=-J\cdot(t_a\varphi)$. Substitution in the identity for $W$, followed by multiplication by $-1$, proves the [background gauge invariance of a scalar effective action](../../../perturbative-quantum-field-theory.md#background-gauge-invariance-of-a-scalar-effective-action):

$$
\boxed{\left[(t_a\varphi)\cdot\frac{\delta}{\delta\varphi}+\partial_\mu\frac{\delta}{\delta A_{\mu a}}+f_{abc}A_{\mu b}\frac{\delta}{\delta A_{\mu c}}\right]\Gamma=0.}
$$

The derivatives of the [quantum effective action](../../../perturbative-quantum-field-theory.md#effective-action) are proper, amputated [one-particle-irreducible vertices](../../../perturbative-quantum-field-theory.md#one-particle-irreducible-vertex). At each [loop order](../../../perturbative-quantum-field-theory.md#loop-order) they receive contributions from [one-particle-irreducible Feynman diagrams](../../../perturbative-quantum-field-theory.md#one-particle-irreducible-feynman-diagram) with the indicated external scalar legs, including tree vertices and the required [counterterms](../../../perturbative-quantum-field-theory.md#counterterm). Diagrams which disconnect after cutting one internal line are not additional proper-vertex contributions. Translation invariance supplies the overall momentum-conserving delta function factored out in the definition. The signs of these vertices must follow the chosen overall convention for $\Gamma$.

Differentiate the effective-action identity twice with respect to $\varphi_i(y)$ and $\varphi_j(z)$ and set $\varphi=A=0$. In an invariant zero-field vacuum this gives the [Ward identity contact terms](../../../perturbative-quantum-field-theory.md#ward-identity-contact-terms)

$$
\partial_\mu\Gamma^\mu_{a,ij}(x;y,z)+(t_a)_{ki}\delta(x-y)\Gamma^{(2)}_{kj}(x,z)+(t_a)_{kj}\delta(x-z)\Gamma^{(2)}_{ki}(x,y)=0.
$$

The term proportional to $A$ vanishes. With the printed Fourier factors $e^{ip_rx_r}$, integration by parts turns $\partial_\mu$ into $-ip_{1\mu}$. The first delta function combines $p_1$ with $p_2$, and the second combines $p_1$ with $p_3$. Using $(t_a)_{ki}=-(t_a)_{ik}$ and symmetry of the scalar two-point kernel then yields

$$
\boxed{p_{1\mu}\widehat\tau^\mu_{a,ij}=i(t_a)_{ik}\widehat\tau_{kj}(p_1+p_2,p_3)-\widehat\tau_{ik}(p_2,p_3+p_1)i(t_a)_{kj}.}
$$

This derivation fixes the relative signs independently of any vertex rule.

There is an overall-sign inconsistency in the final printed example. At tree level, stationarity of the [source](../../../perturbative-quantum-field-theory.md#source-quantum-field-theory) integral gives $W=S_0[\varphi,A]+\int J\varphi$, hence **the specified transform gives $\Gamma_{\mathrm{tree}}=-S_0$**. For the free scalar multiplet this implies, after factoring out the delta function,

$$
\widehat\tau_{ij}(p,-p)=(p^2+m^2)\delta_{ij},\qquad \boxed{\widehat\tau^\mu_{a,ij}=+i(p_2-p_3)^\mu(t_a)_{ij}.}
$$

The mixed result follows by expanding $-S_0$ to first order in $A$: its contribution is $\int A_{\mu a}(\partial^\mu\varphi_i)(t_a)_{ij}\varphi_j$. The two scalar derivatives yield $i p_2^\mu(t_a)_{ij}+i p_3^\mu(t_a)_{ji}$. [Momentum conservation](../../../classical-mechanics.md#momentum-conservation) gives

$$
p_1\cdot(p_2-p_3)=p_3^2-p_2^2,
$$

so both sides of the [Ward identity](../../../perturbative-quantum-field-theory.md#ward-identity) equal $i(p_3^2-p_2^2)(t_a)_{ij}$. Because the scalar theory is Gaussian for prescribed $A$, its fluctuation determinant depends on $A$ but not on $\varphi$; it cannot add further two-scalar vertices. Thus this quadratic verification is sufficient, not merely the first term of an omitted scalar-loop correction.

The printed mixed vertex instead has a minus sign. It satisfies the same [Ward identity](../../../perturbative-quantum-field-theory.md#ward-identity) if one uses the opposite effective-action convention $\Gamma_{\mathrm{alt}}=W-\int J\varphi=S_0$ at tree level, because its two-point vertex is then $-(p^2+m^2)\delta_{ij}$ as well. **Either overall convention works, but the printed [Legendre transform](../../../convex-optimization.md#convex-conjugate) and printed mixed vertex cannot both be used unchanged.** For example, with $p_2^2\ne p_3^2$ and a nonzero generator, they give opposite sides of the claimed identity.

## 3

↑ **Parent:** [Paper 51](paper-51.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

A [renormalizable quantum field theory](../../../perturbative-quantum-field-theory.md#renormalizable-quantum-field-theory) requires only finitely many independent field and parameter redefinitions to remove regulator dependence from its perturbative [correlation functions](../../../critical-phenomenon.md#correlation-function), order by order. The allowed local [counterterms](../../../perturbative-quantum-field-theory.md#counterterm) must close within that finite set; it is not necessary that the unrenormalized integrals be finite.

In four spacetime dimensions the [kinetic term](../../../quantum-field-theory.md#kinetic-term) fixes the [mass dimension](../../../perturbative-quantum-field-theory.md#mass-dimension) of $\phi$ to one. A coefficient multiplying $\phi^k$ therefore has dimension $4-k$. [Power counting](../../../perturbative-quantum-field-theory.md#power-counting-in-quantum-field-theory) excludes couplings of negative [mass dimension](../../../perturbative-quantum-field-theory.md#mass-dimension) for perturbative renormalizability. For a single scalar with a conventional nonderivative [polynomial](../../../polynomial.md) potential, the allowed form is

$$
\boxed{V(\phi)=v_0+h\phi+\frac12m^2\phi^2+\frac{\lambda_3}{3!}\phi^3+\frac{\lambda_4}{4!}\phi^4.}
$$

The constant controls vacuum energy and the linear term a possible tadpole. A field-reflection symmetry can remove the odd terms but is not necessary for renormalizability. Terms of degree above four generally require an infinite tower of [counterterms](../../../perturbative-quantum-field-theory.md#counterterm) when treated as fundamental interactions; they can instead be used in an [effective field theory](../../../quantum-field-theory.md#effective-field-theory). Stability of the potential is a separate requirement, for example a positive quartic leading term, and should not be confused with the power-counting criterion.

For a graph with $E$ external scalar lines, $I$ internal lines, $L$ loops and $V_k$ vertices of degree $k$, the superficial [ultraviolet divergence](../../../perturbative-quantum-field-theory.md#ultraviolet-divergence) degree is $\omega=4L-2I$. The identities $L=I-\sum_kV_k+1$ and $2I+E=\sum_k kV_k$ give

$$
\omega=4-E+\sum_k(k-4)V_k.
$$

When every $k\le4$, only the finitely many low-point local divergences, including the [kinetic term](../../../quantum-field-theory.md#kinetic-term), can require subtraction. Subdivergences are removed recursively by the same local [counterterms](../../../perturbative-quantum-field-theory.md#counterterm). A vertex with $k>4$ instead permits arbitrarily high divergence degrees as more such vertices are added. This explains the restriction rather than merely asserting it.

The bare [Lagrangian density](../../../quantum-field-theory.md#lagrangian-density) is written in terms of regulator-dependent bare quantities, before taking the regulator away:

$$
\mathcal L_B=-\frac12(\partial\phi_B)^2-V_B(\phi_B),\qquad\phi_B=Z_\phi^{1/2}\phi,\qquad\mathcal L_B=\mathcal L_R+\mathcal L_{\mathrm{ct}}.
$$

The coefficients in $V_B$ are related to the [renormalized](../../../perturbative-quantum-field-theory.md#renormalization) parameters by regulator-dependent redefinitions. The [wave-function renormalization](../../../perturbative-quantum-field-theory.md#wave-function-renormalization) supplies a kinetic [counterterm](../../../perturbative-quantum-field-theory.md#counterterm). In [dimensional regularization](../../../perturbative-quantum-field-theory.md#dimensional-regularization) $d=4-\epsilon$, a quartic coupling has a bare relation of the form $\lambda_B=\mu^\epsilon[\lambda+\delta\lambda(\lambda,\epsilon)]$, with field factors incorporated according to the chosen definition. The bare parameters and bare [correlation functions](../../../critical-phenomenon.md#correlation-function) are held fixed when changing the [renormalization scale](../../../perturbative-quantum-field-theory.md#renormalization-scale).

Even without a physical [mass](../../../classical-mechanics.md#mass), interacting loop subtractions require a reference scale $\mu$ to define the [renormalized](../../../perturbative-quantum-field-theory.md#renormalization) dimensionless coupling and field normalization. Finite logarithms then involve dimensionless combinations such as $\mu|x_r-x_s|$ or $p^2/\mu^2$. This scale is a subtraction convention, not a new physical [mass](../../../classical-mechanics.md#mass) parameter. Its explicit dependence is compensated by the [running coupling](../../../perturbative-quantum-field-theory.md#running-coupling) and field normalization.

Let $G_n=\langle\phi(x_1)\cdots\phi(x_n)\rangle$ at separated points. Its bare counterpart satisfies $G_{B,n}=Z_\phi^{n/2}G_n$. Define

$$
\beta(g)=\left.\mu\frac{dg}{d\mu}\right|_{\mathrm{bare}},\qquad\gamma(g)=\left.\frac12\mu\frac{d\log Z_\phi}{d\mu}\right|_{\mathrm{bare}}.
$$

Differentiating $G_{B,n}$ at fixed bare theory gives

$$
\boxed{\left(\mu\partial_\mu+\beta(g)\partial_g+n\gamma(g)\right)G_n=0.}
$$

This [Callan-Symanzik equation](../../../perturbative-quantum-field-theory.md#callan-symanzik-equation) expresses independence of the arbitrary subtraction scale. The [renormalization-group beta function](../../../perturbative-quantum-field-theory.md#beta-function-physics) describes the compensating coupling change; the [field-renormalization anomalous dimension](../../../critical-phenomenon.md#field-renormalization-anomalous-dimension) describes the compensating rescaling of each insertion. Coincident composite insertions would require their own additional [renormalization](../../../perturbative-quantum-field-theory.md#renormalization), rather than automatically obeying this separated-point equation.

For the two-point function, set $z=p^2/\mu^2$ and $t=\tfrac12\log z$. We consider large positive spacelike $p^2$, with continuation to other momenta as required. The dimensionless [propagator](../../../quantum-field-theory.md#propagator) factor obeys

$$
(-\partial_t+\beta\partial_g+2\gamma)d(e^{2t},g)=0.
$$

Define $\bar g(0)=g$ and $d\bar g/dt=\beta(\bar g)$. The [renormalization-group characteristic solution for a two-point function](../../../perturbative-quantum-field-theory.md#renormalization-group-characteristic-solution-for-a-two-point-function) is

$$
\boxed{d(e^{2t},g)=d(1,\bar g(t))\exp\left\{2\int_0^t\gamma(\bar g(s))\,ds\right\}.}
$$

To verify it, the running-coupling flow has $\beta(g)\partial_g\bar g(t)=\beta(\bar g(t))$. Also, $\beta(g)\partial_g\int_0^t\gamma(\bar g(s))ds=\gamma(\bar g(t))-\gamma(g)$. Applying $\partial_t-\beta(g)\partial_g$ to the displayed expression therefore gives $2\gamma(g)d$, exactly the required differential equation. The boundary value $d(1,g)$ records the [renormalization](../../../perturbative-quantum-field-theory.md#renormalization) condition. This shows how the ultraviolet behaviour is determined by the coupling trajectory and its accumulated [anomalous dimension](../../../critical-phenomenon.md#anomalous-dimension): it can approach zero coupling, a nonzero fixed point, or a finite-scale singularity, depending on $\beta$.

For $\beta=-bg^3$ with $b>0$, direct integration gives

$$
\bar g(t)^2=\frac{g^2}{1+2bg^2t},\qquad2\int_0^t c\bar g(s)^2\,ds=\frac cb\log(1+2bg^2t).
$$

Consequently

$$
\boxed{d(z,g)=d\left(1,\frac{g}{\sqrt{1+bg^2\log z}}\right)\left(1+bg^2\log z\right)^{c/b}.}
$$

For a regular free-theory normalization $d(1,0)=1$, the leading large-$z$ form is $(1+bg^2\log z)^{c/b}$, times corrections from the small [running coupling](../../../perturbative-quantum-field-theory.md#running-coupling). This is [asymptotic freedom](../../../perturbative-quantum-field-theory.md#asymptotic-freedom) with a logarithmic, rather than a fixed-power, [propagator](../../../quantum-field-theory.md#propagator) correction. The hypothetical beta and gamma functions are being used as given; this calculation does not assert that they are the actual beta and gamma functions of an arbitrary quartic scalar theory.

For the second beta function put $B=-b>0$, so $\beta(g)=Bg^3-ag^5$. Its positive nonzero fixed point and linearized slope are

$$
\boxed{g_*^2=\frac{B}{a}=-\frac ba,\qquad\beta^{\prime}(g_*)=-\frac{2B^2}{a}<0.}
$$

For $0<g<g_*$ the coupling increases with momentum, while for $g>g_*$ it decreases; each positive trajectory approaches $g_*$ in the ultraviolet. Negative initial couplings approach $-g_*$ by the odd symmetry of the beta function, with the same limiting squared coupling. The exactly zero trajectory remains zero. Thus the [nonzero ultraviolet fixed point of a cubic-quintic beta function](../../../perturbative-quantum-field-theory.md#nonzero-ultraviolet-fixed-point-of-a-cubic-quintic-beta-function) replaces asymptotic freedom by a finite-coupling ultraviolet limit, with $\bar g(t)-g_*=O(e^{-2B^2t/a})$. If the [anomalous dimension](../../../critical-phenomenon.md#anomalous-dimension) is regular there, the [propagator](../../../quantum-field-theory.md#propagator) factor has fixed-point behaviour $d(z,g)\sim A(g)z^{\gamma(g_*)}$ when its fixed-point boundary value is nonzero. If $\gamma(g)=cg^2$ is retained, the exponent is $\gamma(g_*)=-cb/a$. Trusting this perturbative truncation as a statement about the underlying theory requires $g_*$ to be sufficiently small; the flow result itself follows from the specified beta function.

## 4

↑ **Parent:** [Paper 51](paper-51.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

Without [gauge fixing](../../../relativistic-quantum-field.md#gauge-fixing), gauge-equivalent configurations are integrated repeatedly, and the quadratic gauge-field operator has [zero modes](../../../linear-operator-theory.md#zero-mode) along infinitesimal gauge transformations. It therefore has no inverse with which to define perturbative [propagators](../../../quantum-field-theory.md#propagator). A gauge condition removes these directions locally in the perturbative expansion. The associated [Faddeev-Popov determinant](../../../relativistic-quantum-field.md#faddeev-popov-determinant) can be represented by anticommuting [Faddeev-Popov ghost fields](../../../relativistic-quantum-field.md#faddeev-popov-ghost) and [Faddeev-Popov antighost fields](../../../relativistic-quantum-field.md#faddeev-popov-antighost-field).

First make the normalization explicit. For the fields literally occurring in the [action](../../../classical-mechanics.md#action) with overall $1/g^2$, put

$$
A_\mu=g a_\mu,\qquad c=g\eta,\qquad\bar c=g\bar\eta.
$$

The resulting kinetic terms are canonical, and the interaction terms carry powers of $g$. We use signature $(-,+,+,+)$ and incoming Fourier modes $e^{ipx}$, consistent with the displayed $p^2-i0$ denominators. The quadratic [action](../../../classical-mechanics.md#action) in the canonical fields is

$$
S_2=\frac12\int a_\mu\left[\eta^{\mu\nu}\Box-(1-\xi^{-1})\partial^\mu\partial^\nu\right]a_\nu\,d^dx+\int\bar\eta\Box\eta\,d^dx.
$$

Color indices are diagonal. Introduce the longitudinal and transverse projectors $P_{L,\mu\nu}=p_\mu p_\nu/p^2$ and $P_T=\eta-P_L$. The gauge kinetic matrix is $-p^2(P_T+\xi^{-1}P_L)$, with inverse $-(P_T+\xi P_L)/p^2$. The ghost kinetic operator is $-p^2$. The [Gaussian functional integral](../../../quantum-field-theory.md#gaussian-functional-integral) and [Grassmann integral](../../../quantum-mechanics.md#berezin-integral) therefore give

$$
\boxed{\widetilde\Delta^{\mathrm{can}}_{F\mu\nu}(p)=-\frac1{p^2-i0}\left[\eta_{\mu\nu}-(1-\xi)\frac{p_\mu p_\nu}{p^2-i0}\right],\qquad\widetilde\Delta^{\mathrm{can}}_F(p)=-\frac1{p^2-i0}.}
$$

The longitudinal formula is understood as the Feynman-prescribed inverse of the kinetic operator; away from its poles the projector inversion is ordinary algebra. The [propagators](../../../quantum-field-theory.md#propagator) for the original unrescaled fields are $g^2$ times these expressions. Using $P_Tp=0$ and $P_Lp=p$ gives

$$
\boxed{\widetilde\Delta_{F\mu\nu}(p)p^\nu=\xi p_\mu\widetilde\Delta_F(p),}
$$

with either normalization. This is the [longitudinal gauge propagator contraction](../../../relativistic-quantum-field.md#longitudinal-gauge-propagator-contraction).

The canonical ghost interaction comes directly from the covariant derivative:

$$
\mathcal L_{\bar\eta a\eta}=-g f_{abc}(\partial^\mu\bar\eta_a)a_{\mu b}\eta_c.
$$

For incoming antighost momentum $p$, the derivative supplies $ip^\mu$; the expansion of $e^{iS}$ supplies another $i$. Thus the [ghost-gluon vertex](../../../relativistic-quantum-field.md#ghost-gluon-vertex) is **$gp^\mu f_{abc}$**, as requested. For unrescaled fields its coefficient is instead $p^\mu f_{abc}/g^2$. The printed order-$g$ rule presupposes canonical normalization; keeping the overall $1/g^2$ and an order-$g$ vertex for the same unrescaled variables would mix conventions. Choosing Fourier modes $e^{-ipx}$ instead reverses the vertex sign and must be done consistently for all momentum assignments.

In [Feynman gauge](../../../relativistic-quantum-field.md#feynman-gauge), $\xi=1$, the one-loop ghost two-point graph has one internal ghost line and one internal gauge line joined by two such vertices. The external ghost line is open, so it does not carry a closed ghost-loop minus sign. With an orthonormal adjoint basis, the [structure constants](../../../algebra.md#structure-constant) are totally antisymmetric, and the color product along this line is $f_{adc}f_{cdb}=-C\delta_{ab}$. The two internal [propagators](../../../quantum-field-theory.md#propagator) supply $(-i)^2=-1$, leaving a positive color-and-vertex factor for the amputated insertion. Define

$$
I_d(p)=\frac1i\int\frac{d^dk}{(2\pi)^d}\frac{p\cdot k}{[(p-k)^2-i0][k^2-i0]}.
$$

The amputated insertion is $i\delta_{ab}g^2 I_d(p)C$. Restoring the two external canonical [ghost propagators](../../../relativistic-quantum-field.md#ghost-propagator) gives the one-loop contribution

$$
\boxed{G^{(1)}_{ab}(p)=-i\delta_{ab}\frac{g^2C I_d(p)}{(p^2-i0)^2}.}
$$

The literal unrescaled correlator in the question is $g^2G^{(1)}$, hence of order $g^4$, whereas its tree term is $-i\delta_{ab}g^2/(p^2-i0)$. In $d\ne4$ the dimensionless [renormalized](../../../perturbative-quantum-field-theory.md#renormalization) coupling convention adds $\mu^{4-d}$ multiplying $g^2$ in the canonical loop term.

To evaluate the [Feynman integral](../../../perturbative-quantum-field-theory.md#feynman-integral), combine the denominators with a [Feynman parameter](../../../perturbative-quantum-field-theory.md#feynman-parameter):

$$
\frac1{k^2(p-k)^2}=\int_0^1\frac{d\alpha}{[\alpha k^2+(1-\alpha)(p-k)^2]^2}.
$$

Shift $\ell=k-(1-\alpha)p$. The denominator becomes $[\ell^2+\alpha(1-\alpha)p^2-i0]^2$, and the numerator is $p\cdot\ell+(1-\alpha)p^2$. The odd term vanishes in translation-invariant [dimensional regularization](../../../perturbative-quantum-field-theory.md#dimensional-regularization). For spacelike $p$, a [Wick rotation](../../../perturbative-quantum-field-theory.md#wick-rotation) converts the remaining integral into a Euclidean one and cancels the prefactor $1/i$. The needed radial integral is

$$
\int\frac{d^d\ell_E}{(2\pi)^d}\frac1{(\ell_E^2+M^2)^2}=\frac{\Gamma(2-d/2)}{(4\pi)^{d/2}}(M^2)^{d/2-2}.
$$

Indeed, [spherical coordinates](../../../calculus.md#spherical-coordinate-system) and $u=\ell_E^2/M^2$ leave a beta integral $\int_0^\infty u^{d/2-1}(1+u)^{-2}du=\Gamma(d/2)\Gamma(2-d/2)$; the angular factor cancels $\Gamma(d/2)$. Establish this first in a convergent range and then analytically continue in $d$. Substituting $M^2=\alpha(1-\alpha)p^2$ yields

$$
\boxed{I_d(p)=\frac{(p^2)^{d/2-1}}{(4\pi)^{d/2}}\Gamma(2-d/2)\int_0^1\alpha^{d/2-2}(1-\alpha)^{d/2-1}\,d\alpha.}
$$

This is the printed result, including the factor $1/i$ in its Minkowski-space definition. Equivalently the parameter integral is $B(d/2-1,d/2)$. Symmetry under $k\leftrightarrow p-k$ also gives $I_d(p)$ as $p^2/2$ times the massless scalar bubble, independently checking the numerator factor.

Write $\epsilon=4-d$. Since $\Gamma(\epsilon/2)=2/\epsilon+O(1)$ and the parameter integral tends to $\int_0^1(1-\alpha)d\alpha=1/2$, the pole is

$$
\boxed{I_d(p)\big|_{\mathrm{div}}=\frac{p^2}{16\pi^2\epsilon},\qquad G^{(1)}_{ab}(p)\big|_{\mathrm{div}}=-i\delta_{ab}\frac{g^2C}{16\pi^2\epsilon\,p^2}.}
$$

Here $p$ is off shell and nonzero, separating the ultraviolet pole from massless infrared issues. The unrescaled amplitude has an extra factor $g^2$. The divergence is proportional to the existing ghost kinetic operator, so the [one-loop ghost kinetic counterterm in Feynman gauge](../../../relativistic-quantum-field.md#one-loop-ghost-kinetic-counterterm-in-feynman-gauge) is local:

$$
\boxed{\mathcal L_{\mathrm{ct}}=-\delta Z_c\,\partial^\mu\bar\eta\cdot\partial_\mu\eta,\qquad\delta Z_c=\frac{g^2C}{16\pi^2\epsilon}.}
$$

It inserts $-i\delta Z_cp^2$ into the inverse [propagator](../../../quantum-field-theory.md#propagator), cancelling the divergent insertion $+ig^2CI_d(p)$. With the two external [propagators](../../../quantum-field-theory.md#propagator) attached, its contribution is $+i\delta_{ab}\delta Z_c/p^2$, cancelling the displayed connected amplitude pole. In the original variables the same [action](../../../classical-mechanics.md#action) term is $-\delta Z_c\,\partial\bar c\cdot\partial c/g^2$. If instead one defines dimensional regularization by $d=4-2\epsilon$, the identical counterterm is written $\delta Z_c=g^2C/(32\pi^2\epsilon)$; the factor of two is purely the regulator convention.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2008](../../2008.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
