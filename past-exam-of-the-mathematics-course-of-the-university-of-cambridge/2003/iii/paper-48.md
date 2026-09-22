# Paper 48

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2003/Paper48.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2003/Paper48.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
- [3](#3)
  - [Solution](#3/solution)
  - [i](#3/i)
    - [Solution](#3/i/solution)
  - [ii](#3/ii)
    - [Solution](#3/ii/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)

## 1

↑ **Parent:** [Paper 48](paper-48.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Write the [Hamiltonian operator](../../../quantum-mechanics.md#hamiltonian-quantum-mechanics) as $\widehat H=\widehat p^2/(2m)+V(\widehat q)$, with $[\widehat q,\widehat p]=i$, and define the [quantum-mechanical propagator](../../../quantum-mechanics.md#quantum-mechanical-propagator) by $U(\beta,\alpha;T)=\langle\beta|e^{-iT\widehat H}|\alpha\rangle$. Use $N$ intervals of length $\varepsilon=T/N$, endpoint coordinates $q_0=\alpha,q_N=\beta$, and the [Trotter product formula](../../../numerical-analysis.md#lie-product-formula). Inserting the completeness relations of the [position eigenstates](../../../quantum-mechanics.md#position-eigenstate) between the short-time factors gives

$$
U=\lim_{N\to\infty}\int\prod_{j=1}^{N-1}dq_j\prod_{j=1}^N\langle q_j|e^{-i\varepsilon\widehat p^2/(2m)}e^{-i\varepsilon V(\widehat q)}|q_{j-1}\rangle.
$$

Normalize [momentum eigenstates](../../../quantum-mechanics.md#momentum-eigenstate) by $\langle q|p\rangle=e^{ipq}/\sqrt{2\pi}$. The [Gaussian integral](../../../calculus.md#gaussian-integral) over the intermediate [momentum](../../../classical-mechanics.md#momentum) is

$$
\int\frac{dp}{2\pi}\exp\left(ip(q_j-q_{j-1})-\frac{i\varepsilon p^2}{2m}\right)=\left(\frac{m}{2\pi i\varepsilon}\right)^{1/2}\exp\left(\frac{im(q_j-q_{j-1})^2}{2\varepsilon}\right).
$$

The square-root branch is fixed by continuation from $\operatorname{Im}\varepsilon<0$. Consequently the precise [time-sliced configuration-space path integral](../../../quantum-field-theory.md#time-sliced-configuration-space-path-integral) is

$$
\boxed{U=\lim_{N\to\infty}\left(\frac{m}{2\pi i\varepsilon}\right)^{N/2}\int_{\mathbb R^{N-1}}\prod_{j=1}^{N-1}dq_j\exp\left[i\sum_{j=1}^N\left\{\frac{m(q_j-q_{j-1})^2}{2\varepsilon}-\varepsilon V(q_{j-1})\right\}\right].}
$$

This formula defines the notation $\int\mathcal Dq\,e^{iS[q]}$; it is not an unnormalized infinite product of ordinary integrals. For real time take the boundary value from $T-i\delta$, $\delta>0$, or the corresponding oscillatory-distribution limit. For a self-adjoint, bounded-below [Hamiltonian operator](../../../quantum-mechanics.md#hamiltonian-quantum-mechanics) under the usual product-formula hypotheses, the operator limit supplies the definition even where the coordinate kernel is a distribution. The discrete exponent approaches the [action](../../../classical-mechanics.md#action) with [kinetic term](../../../quantum-field-theory.md#kinetic-term) $m\dot q^2/2$, and the prefactor is part of the [functional measure](../../../quantum-field-theory.md#functional-measure). A different consistent slicing gives the same kernel for this separated kinetic-plus-potential Hamiltonian.

For the [quantum harmonic oscillator](../../../quantum-mechanics.md#quantum-harmonic-oscillator), expand the [action](../../../classical-mechanics.md#action) about a [classical path](../../../quantum-field-theory.md#classical-path) $x$, writing $q=x+\xi$ with homogeneous [Dirichlet boundary conditions](../../../differential-equation.md#dirichlet-boundary-condition) on $\xi$. The only mixed term is

$$
m\int_0^T(\dot x\dot\xi-\omega^2x\xi)\,dt=m[\dot x\xi]_0^T-m\int_0^T(\ddot x+\omega^2x)\xi\,dt=0.
$$

The boundary term vanishes and the [Euler-Lagrange equation](../../../analysis.md#euler-lagrange-equation) sets the remaining integrand to zero. Thus $S[x+\xi]=S[x]+S[\xi]$ exactly, rather than only to quadratic approximation. Translation of each integrated coordinate has unit [Jacobian determinant](../../../calculus.md#jacobian-determinant); in the continuum measure convention of the question this is $\mathcal Dq=\mathcal D\xi$. The [classical-path factorization of a quadratic path integral](../../../quantum-field-theory.md#classical-path-factorization-of-a-quadratic-path-integral) follows:

$$
\boxed{U(\beta,\alpha;T)=e^{iS[x]}F(T),\qquad F(T)=\int_{\xi(0)=\xi(T)=0}\mathcal D\xi\,e^{iS[\xi]}.}
$$

The fluctuation [action](../../../classical-mechanics.md#action), measure and boundary values depend on $T,m,\omega$ but not on $\alpha,\beta$. For real $T$ with $\sin\omega T\ne0$ the boundary-value [classical path](../../../quantum-field-theory.md#classical-path) exists uniquely. At the conjugate times $\omega T=k\pi$, generic endpoints admit no such path and the kernel is a delta distribution; the formula is interpreted by the same regulated boundary limit, not as an ordinary finite prefactor times a nonexistent classical solution.

## 2

↑ **Parent:** [Paper 48](paper-48.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Use a real [scalar field](../../../quantum-field-theory.md#scalar-field) and Minkowski [action](../../../classical-mechanics.md#action) $S[\phi]$, with the vacuum selected by a [Feynman propagator](../../../quantum-field-theory.md#feynman-propagator) pole prescription or adiabatic vacuum boundary conditions. The normalized [correlation functions](../../../critical-phenomenon.md#correlation-function) are

$$
G_n(x_1,\ldots,x_n)=\frac{\int\mathcal D\phi\,\phi(x_1)\cdots\phi(x_n)e^{iS[\phi]}}{\int\mathcal D\phi\,e^{iS[\phi]}}=\langle\Omega|\mathcal T\{\widehat\phi_H(x_1)\cdots\widehat\phi_H(x_n)\}|\Omega\rangle.
$$

Here $|\Omega\rangle$ is the interacting vacuum and $\mathcal T$ denotes [time ordering](../../../perturbative-quantum-field-theory.md#time-ordering). These are the canonical [vacuum expectation values](../../../quantum-field-theory.md#vacuum-expectation-value), rather than unordered products of noncommuting fields. The [functional integral](../../../quantum-field-theory.md#functional-measure) formula assumes a regulated measure and the same vacuum prescription on both sides.

Couple an [external source](../../../perturbative-quantum-field-theory.md#source-quantum-field-theory) $J$ linearly to the [scalar field](../../../quantum-field-theory.md#scalar-field) and choose the [normalized vacuum generating functional](../../../perturbative-quantum-field-theory.md#normalized-vacuum-generating-functional)

$$
Z[J]=\frac{\int\mathcal D\phi\,\exp\left(iS[\phi]+i\int d^dx\,J\phi\right)}{\int\mathcal D\phi\,e^{iS[\phi]}},\qquad Z[0]=1.
$$

Then [functional derivatives](../../../calculus-of-variations.md#functional-derivative) insert the fields:

$$
G_n=\left.i^{-n}\frac{\delta^nZ}{\delta J(x_1)\cdots\delta J(x_n)}\right|_{J=0},\qquad Z[J]=\sum_{n=0}^\infty\frac{i^n}{n!}\int G_n(x_1,\ldots,x_n)\prod_{j=1}^n J(x_j)\,d^dx_j.
$$

In the convention used below, the [connected generating functional](../../../perturbative-quantum-field-theory.md#connected-generating-functional) is

$$
\boxed{Z[J]=e^{iW[J]},\qquad W[J]=-i\log Z[J],\qquad G_n^c=\left.i^{1-n}\frac{\delta^nW}{\delta J(x_1)\cdots\delta J(x_n)}\right|_{J=0}.}
$$

The logarithm removes products of disconnected components. For example the [connected correlation function](../../../critical-phenomenon.md#connected-correlation-function) $G_2^c=G_2-G_1G_1$; at three points one subtracts all three $G_2G_1$ products and adds $2G_1G_1G_1$. Normalization has already removed [vacuum bubbles](../../../perturbative-quantum-field-theory.md#vacuum-feynman-diagram).

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Keep $Z=e^{iW}$, define the mean [scalar field](../../../quantum-field-theory.md#scalar-field) $\varphi(x)=\delta W/\delta J(x)$, and locally invert the source-field relation. The [quantum effective action](../../../perturbative-quantum-field-theory.md#effective-action) is the [Legendre transform](../../../convex-optimization.md#convex-conjugate)

$$
\boxed{\Gamma[\varphi]=W[J]-\int d^dx\,J(x)\varphi(x),\qquad\frac{\delta\Gamma}{\delta\varphi(x)}=-J(x).}
$$

Its value at zero source is expanded around $\varphi_0=\langle\phi\rangle$, which need not vanish. The kernels $\Gamma^{(n)}=\delta^n\Gamma/\delta\varphi^n|_{\varphi_0}$ are the [one-particle-irreducible vertices](../../../perturbative-quantum-field-theory.md#one-particle-irreducible-vertex), with the Minkowski diagram vertex factor $i\Gamma^{(n)}$. A [one-particle-irreducible Feynman diagram](../../../perturbative-quantum-field-theory.md#one-particle-irreducible-feynman-diagram) remains connected after any one internal line is cut. [Amputation of external propagators](../../../perturbative-quantum-field-theory.md#amputation-of-external-propagators) removes the full two-point functions on its external legs. For higher-point connected graphs amputation alone need not remove internal [one-particle-reducible Feynman diagrams](../../../perturbative-quantum-field-theory.md#one-particle-reducible-feynman-diagram); the derivatives of $\Gamma$ select precisely the irreducible kernels.

To derive the three-point relation, use condensed indices that include spacetime integration. Put $D_{ij}=W_{,ij}=iG_{2,ij}^c$ and $K=\Gamma^{(2)}$. Differentiating $\Gamma_{,i}=-J_i$ gives $K_{ia}D_{aj}=-\delta_{ij}$, so $K=-D^{-1}$. A further derivative, using $\delta D_{ab}/\delta\varphi_k=W_{,ab\ell}(D^{-1})_{\ell k}$ and the derivative of an inverse, gives

$$
\Gamma^{(3)}_{ijk}=(D^{-1})_{ia}(D^{-1})_{jb}(D^{-1})_{kc}W_{,abc}.
$$

Since $W^{(3)}=-G_3^c$ and $D^{-1}=-i(G_2^c)^{-1}$, the [three-point amputation in the connected-action convention](../../../perturbative-quantum-field-theory.md#three-point-amputation-in-the-connected-action-convention) is

$$
\boxed{i\Gamma^{(3)}_{ijk}=\int da\,db\,dc\,(G_2^c)^{-1}_{ia}(G_2^c)^{-1}_{jb}(G_2^c)^{-1}_{kc}G_{3,abc}^c.}
$$

Equivalently, attach a full [two-point correlation function](../../../critical-phenomenon.md#two-point-correlation-function) to each leg of $i\Gamma^{(3)}$ to reconstruct $G_3^c$. The connected functions are evaluated at the same zero-source background. The displayed factors of $i$ follow from the declared Minkowski convention; Euclidean generating functionals redistribute these factors.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

For a bosonic quadratic [action](../../../classical-mechanics.md#action) $S_2=\tfrac12\int\phi K\phi$, [completing the square](../../../polynomial.md#completing-the-square) in the [generating functional](../../../perturbative-quantum-field-theory.md#generating-functional) gives $Z_0[J]/Z_0[0]=\exp(-iJK^{-1}J/2)$. Two [functional derivatives](../../../calculus-of-variations.md#functional-derivative) therefore give the [Feynman propagator](../../../quantum-field-theory.md#feynman-propagator) $\Delta=iK^{-1}$, with boundary conditions and a pole prescription included in the inverse. Zero modes must be removed or fixed before an inverse exists.

Take Minkowski metric $\eta=\operatorname{diag}(1,-1,-1,-1)$, Fourier convention $e^{-ikx}$, and the [Yang-Mills field strength](../../../relativistic-quantum-field.md#gauge-field-strength) $F_{\mu\nu}^a=\partial_\mu A_\nu^a-\partial_\nu A_\mu^a+gf^{abc}A_\mu^bA_\nu^c$. The interaction terms do not contribute to the quadratic [action](../../../classical-mechanics.md#action). [Integration by parts](../../../calculus.md#integration-by-parts) in $-F^a_{\mu\nu}F^{a\mu\nu}/4-(\partial\cdot A^a)^2/(2\alpha)$ yields

$$
S_2=\frac12\int d^dx\,A_\mu^a\left[\eta^{\mu\nu}\Box-(1-\alpha^{-1})\partial^\mu\partial^\nu\right]A_\nu^a.
$$

The color kernel is diagonal. For $k^2\ne0$, use the [projectors](../../../vector-space.md#projection-linear-algebra) $P_L^{\mu\nu}=k^\mu k^\nu/k^2$ and $P_T^{\mu\nu}=\eta^{\mu\nu}-P_L^{\mu\nu}$. They obey $P_L^2=P_L$, $P_T^2=P_T$, $P_LP_T=0$, so

$$
K^{ab\mu\nu}(k)=-\delta^{ab}k^2(P_T^{\mu\nu}+\alpha^{-1}P_L^{\mu\nu}),\qquad (K^{-1})_{\mu\nu}^{ab}=-\frac{\delta^{ab}}{k^2}(P_{T\mu\nu}+\alpha P_{L\mu\nu}).
$$

Multiplication explicitly gives the identity on both transverse and longitudinal components. Continuing this inverse with the [Feynman propagator](../../../quantum-field-theory.md#feynman-propagator) prescription gives the [gluon propagator](../../../relativistic-quantum-field.md#gluon-propagator)

$$
\boxed{\Delta_{\mu\nu}^{ab}(x)=\delta^{ab}\int\frac{d^dk}{(2\pi)^d}e^{-ikx}\left[\frac{-i\eta_{\mu\nu}}{k^2+i0}+\frac{i(1-\alpha)k_\mu k_\nu}{(k^2+i0)^2}\right].}
$$

The second term has the causal double-pole prescription. Away from the pole this is the usual $-i\delta^{ab}[\eta_{\mu\nu}-(1-\alpha)k_\mu k_\nu/k^2]/(k^2+i0)$. For $\alpha=1$ it becomes the [Feynman-gauge adjoint propagator](../../../relativistic-quantum-field.md#feynman-gauge-adjoint-propagator); $\alpha\to0$ gives a transverse [covariant Landau gauge](../../../relativistic-quantum-field.md#landau-gauge-quantum-field-theory) [propagator](../../../quantum-field-theory.md#propagator).

**The limit $\alpha\to\infty$ removes [gauge fixing](../../../relativistic-quantum-field.md#gauge-fixing) and has no finite inverse on the full field space.** The longitudinal eigenvalue $-k^2/\alpha$ tends to zero and its inverse diverges. A contraction with conserved external currents kills the longitudinal term, but that does not define a gauge-unfixed [Gaussian integral](../../../calculus.md#gaussian-integral). This massless limit is not the massive-vector unitary-gauge limit: here it exposes the unfixed [gauge orbit](../../../relativistic-quantum-field.md#gauge-orbit) degeneracy.

## 3

↑ **Parent:** [Paper 48](paper-48.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

Take $M^2>0$ initially to avoid an infrared divergence. A [Schwinger parameterization](../../../perturbative-quantum-field-theory.md#schwinger-parameterization) and the Euclidean [Gaussian integral](../../../calculus.md#gaussian-integral) give, in the convergent range $0<\operatorname{Re}d<4$,

$$
\frac1{(k^2+M^2)^2}=\int_0^\infty dt\,t e^{-t(k^2+M^2)},\qquad \int\frac{d^dk}{(2\pi)^d}e^{-tk^2}=(4\pi t)^{-d/2}.
$$

Integration over $t$ supplies the [Gamma function](../../../complex-analysis.md#gamma-function). Its [analytic continuation](../../../complex-analysis.md#analytic-continuation) defines the answer in [dimensional regularization](../../../perturbative-quantum-field-theory.md#dimensional-regularization):

$$
\boxed{I_d(M^2)=\frac{\Gamma(2-d/2)}{(4\pi)^{d/2}}(M^2)^{d/2-2}.}
$$

Use $d=4-\epsilon$ near four dimensions and $d=6-\epsilon$ near six dimensions. The [Gamma function recurrence](../../../complex-analysis.md#gamma-function-recurrence) implies $\Gamma(\epsilon/2)=2/\epsilon+O(1)$ and $\Gamma(-1+\epsilon/2)=-2/\epsilon+O(1)$. Therefore

$$
\boxed{I_{4-\epsilon}(M^2)=\frac{2}{(4\pi)^2\epsilon}+O(1),\qquad I_{6-\epsilon}(M^2)=-\frac{2M^2}{(4\pi)^3\epsilon}+O(1).}
$$

Both are simple poles. Equivalently their residues as functions of $d$ are $-2/(4\pi)^2$ at $d=4$ and $2M^2/(4\pi)^3$ at $d=6$. The negative pole near six dimensions is a feature of [analytic continuation](../../../complex-analysis.md#analytic-continuation); it is not a negative value of the original convergent positive integral. A massless zero-momentum integral is scaleless and cannot be used indiscriminately to extract these ultraviolet poles, because [dimensional regularization](../../../perturbative-quantum-field-theory.md#dimensional-regularization) then combines ultraviolet and infrared contributions.

For the following [Feynman diagrams](../../../perturbative-quantum-field-theory.md#feynman-diagram), specify the Euclidean [action](../../../classical-mechanics.md#action) and additive [counterterms](../../../perturbative-quantum-field-theory.md#counterterm) explicitly so their signs are unambiguous. The four-dimensional interaction is $\mu^\epsilon\lambda\phi^4/4!$, the six-dimensional interaction is $\mu^{\epsilon/2}g\phi^3/3!$, and the common free inverse [scalar propagator](../../../scalar-field-theory.md#scalar-propagator) is $p^2+m^2$. Here $\epsilon=4-d$ or $6-d$, respectively. The factors of $\mu$ give dimensionless renormalized couplings and change no leading pole residues. The cubic Euclidean theory is treated as a formal perturbation expansion about its massive quadratic [scalar field theory](../../../scalar-field-theory.md); its real cubic potential is not bounded below.

<h3 id="3/i">i</h3>

↑ **Parent:** [3](#3)

<h4 id="3/i/solution">Solution</h4>

↑ **Parent:** [I](#3/i)

Let $p$ be the total external Euclidean [momentum](../../../classical-mechanics.md#momentum) crossing one four-point channel. The two internal [scalar propagators](../../../scalar-field-theory.md#scalar-propagator) produce the [scalar bubble integral](../../../perturbative-quantum-field-theory.md#scalar-bubble-integral)

$$
B_d(p)=\int\frac{d^dk}{(2\pi)^d}\frac1{(k^2+m^2)((k+p)^2+m^2)}.
$$

Using the [Feynman parameter](../../../perturbative-quantum-field-theory.md#feynman-parameter) identity $1/(ab)=\int_0^1 dx\,[xa+(1-x)b]^{-2}$ and shifting the loop [momentum](../../../classical-mechanics.md#momentum) yields

$$
\boxed{B_d(p)=\int_0^1dx\,I_d\big(m^2+x(1-x)p^2\big).}
$$

In [phi-fourth theory](../../../scalar-field-theory.md#quartic-interaction) the [bubble diagram](../../../perturbative-quantum-field-theory.md#bubble-diagram) has two quartic vertices and a [symmetry factor](../../../perturbative-quantum-field-theory.md#feynman-diagram-symmetry-factor) $1/2$ from exchanging its two identical internal lines. There are three partitions of four labelled external legs into two pairs, the $s,t,u$ channels. The connected amputated loop diagram has positive coefficient $\lambda^2 B/2$, whereas the Euclidean [one-particle-irreducible vertex](../../../perturbative-quantum-field-theory.md#one-particle-irreducible-vertex) in the effective [action](../../../classical-mechanics.md#action) has the opposite sign. Thus

$$
\Gamma_E^{(4)}(p_1,p_2,p_3,p_4)=\mu^\epsilon(\lambda+\delta\lambda)-\frac{\mu^{2\epsilon}\lambda^2}{2}\big[B_d(p_1+p_2)+B_d(p_1+p_3)+B_d(p_1+p_4)\big]+O(\lambda^3).
$$

One can check this sign without external-line conventions by expanding the one-loop [quantum effective action](../../../perturbative-quantum-field-theory.md#effective-action) $\tfrac12\operatorname{Tr}\log(K+\mu^\epsilon\lambda\phi^2/2)$. Its second logarithmic term is $-\mu^{2\epsilon}\lambda^2\operatorname{Tr}(K^{-1}\phi^2K^{-1}\phi^2)/16$; four field derivatives give precisely the three negative bubble terms above.

The four-dimensional pole of $I_d$ is independent of its mass argument, so each channel contributes $2/[(4\pi)^2\epsilon]$. The divergence of the proper four-point vertex is $-3\lambda^2/[(4\pi)^2\epsilon]$. The [minimal subtraction scheme](../../../perturbative-quantum-field-theory.md#minimal-subtraction-scheme) therefore requires

$$
\boxed{\delta\lambda=\frac{3\lambda^2}{(4\pi)^2\epsilon},\qquad \mathcal L_{E,\mathrm{ct}}^{(4)}=\frac{\mu^\epsilon\delta\lambda}{4!}\phi^4.}
$$

For a Minkowski interaction $-\mu^\epsilon\lambda\phi^4/4!$, the corresponding local interaction [counterterm](../../../perturbative-quantum-field-theory.md#counterterm) is $-\mu^\epsilon\delta\lambda\phi^4/4!$. No momentum-dependent four-point [counterterm](../../../perturbative-quantum-field-theory.md#counterterm) is needed for these logarithmic poles. This calculation concerns the requested four-point bubble contributions; a massive two-point tadpole and vacuum diagrams require their own mass and vacuum-energy subtractions if those functions are also renormalized.

<h3 id="3/ii">ii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#3/ii)

In [phi cubed theory](../../../scalar-field-theory.md#phi-cubed-theory), a two-point [bubble diagram](../../../perturbative-quantum-field-theory.md#bubble-diagram) has two cubic vertices, two internal [scalar propagators](../../../scalar-field-theory.md#scalar-propagator) and [symmetry factor](../../../perturbative-quantum-field-theory.md#feynman-diagram-symmetry-factor) $1/2$. Its connected amputated insertion is $+\mu^\epsilon g^2 B_d(p)/2$. The inverse [scalar propagator](../../../scalar-field-theory.md#scalar-propagator), or quadratic [one-particle-irreducible vertex](../../../perturbative-quantum-field-theory.md#one-particle-irreducible-vertex), therefore receives the negative insertion:

$$
\Gamma_E^{(2)}(p)=p^2+m^2+\delta Z\,p^2+\delta m^2-\frac{\mu^\epsilon g^2}{2}\int_0^1dx\,I_{6-\epsilon}\big(m^2+x(1-x)p^2\big)+O(g^4).
$$

Equivalently, the connected two-point correction is $G_0(p)^2\mu^\epsilon g^2 B_d(p)/2$, and expansion of its inverse changes the sign. The same sign follows from the second term of $\tfrac12\operatorname{Tr}\log(K+\mu^{\epsilon/2}g\phi)$.

Using the six-dimensional residue and $\int_0^1x(1-x)dx=1/6$, the divergent inverse-propagator correction is

$$
\Gamma_{E,\mathrm{div}}^{(2)}(p)=\frac{g^2}{(4\pi)^3\epsilon}\left(m^2+\frac{p^2}{6}\right).
$$

Its [momentum](../../../classical-mechanics.md#momentum) term requires [wave-function renormalization](../../../perturbative-quantum-field-theory.md#wave-function-renormalization), unlike the massive quartic tadpole. The [minimal-subtraction two-point counterterms in cubic scalar theory](../../../scalar-field-theory.md#minimal-subtraction-two-point-counterterms-in-cubic-scalar-theory) are

$$
\boxed{\delta Z=-\frac{g^2}{6(4\pi)^3\epsilon},\qquad\delta m^2=-\frac{g^2m^2}{(4\pi)^3\epsilon},\qquad\mathcal L_{E,\mathrm{ct}}^{(2)}=\frac12\delta Z(\partial\phi)^2+\frac12\delta m^2\phi^2.}
$$

These are additive coefficients in a Lagrangian expressed in terms of the renormalized field. If $\phi_0=Z^{1/2}\phi$, $Z=1+\delta Z$, and the bare mass is separately written $m_0^2=m^2+\Delta m^2$, then $\delta m^2=m^2\delta Z+\Delta m^2$ at this order, so $\Delta m^2=-5g^2m^2/[6(4\pi)^3\epsilon]$. Distinguishing these conventions prevents a spurious disagreement between mass [counterterms](../../../perturbative-quantum-field-theory.md#counterterm). The local Minkowski [counterterms](../../../perturbative-quantum-field-theory.md#counterterm) are $\delta Z(\partial\phi)^2/2-\delta m^2\phi^2/2$. A complete cubic theory also has one-point and three-point subtractions; they are not the specified two-point bubble poles.

## 4

↑ **Parent:** [Paper 48](paper-48.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

A [Berezin integral](../../../quantum-mechanics.md#berezin-integral) over independent [Grassmann variables](../../../linear-algebra.md#grassmann-variable) selects the coefficient containing every variable. Fix the real orientation by $\int d\omega_1\cdots d\omega_{2m}\,\omega_{2m}\cdots\omega_1=1$. For an [antisymmetric matrix](../../../linear-algebra.md#skew-symmetric-matrix) $A$, only the order-$m$ term in the exponential survives:

$$
\frac{(-1)^m}{2^m m!}\left(\sum_{i,j}\omega_iA_{ij}\omega_j\right)^m.
$$

Anticommutation collects its top coefficient into the signed sum over pairings that defines the [Pfaffian](../../../linear-algebra.md#pfaffian). Reversing the order of $2m$ variables gives $(-1)^{m(2m-1)}=(-1)^m$, cancelling the prefactor sign. The [real Grassmann Gaussian integral](../../../quantum-field-theory.md#real-grassmann-gaussian-integral) is therefore

$$
\boxed{\int d\omega_1\cdots d\omega_{2m}\,e^{-\omega^TA\omega/2}=\operatorname{Pf}(A)}
$$

with this orientation, and a fixed sign times this answer with other orientations. In dimension two, write $A_{12}=a$; the exponential is $1-a\omega_1\omega_2=1+a\omega_2\omega_1$, and integration gives $a$. Although $\operatorname{Pf}(A)^2=\det A$, writing a positive square root $\sqrt{\det A}$ would give $|a|$ in this test and would lose the correct sign.

For the complex [Grassmann Gaussian integral](../../../quantum-field-theory.md#grassmann-gaussian-integral), treat $\theta_a$ and $\bar\theta_a$ as independent integration variables. Every surviving top term contains each $\theta$ and each $\bar\theta$ once. Expanding the exponential assigns one matrix entry from every row and column, and anticommutation supplies the permutation sign. Hence

$$
\boxed{\int\prod_{a=1}^n d\theta_a\prod_{a=1}^n d\bar\theta_a\,e^{-\bar\theta^TM\theta}=C_n\det M,}
$$

where $C_n$ is a nonzero constant fixed by the order and normalization of the differentials, independent of $M$. This argument works for singular matrices as well and does not assume that $M$ is Hermitian.

For the explicit $n=2$ check, put $Q=\bar\theta_aM_{ab}\theta_b$. Moving all the $\theta$ variables before the barred ones gives

$$
\frac12Q^2=(-M_{11}M_{22}+M_{12}M_{21})\theta_1\theta_2\bar\theta_1\bar\theta_2.
$$

The linear and constant terms integrate to zero. Thus the integral is a fixed orientation sign times $M_{11}M_{22}-M_{12}M_{21}$, exactly the [determinant](../../../linear-algebra.md#determinant). Choosing the top-monomial integral to be $-1$ gives $C_2=1$.

For the required [real-complex compatibility of Grassmann Gaussian integrals](../../../quantum-field-theory.md#real-complex-compatibility-of-grassmann-gaussian-integrals), let $u_a=\omega_a$ and $v_a=\omega_{n+a}$. Substitution gives

$$
\bar\theta^TM\theta=\frac12\left(u^TMu+v^TMv+i u^TMv-i v^TMu\right)=\frac12(u^TMu+v^TMv).
$$

Indeed $v^TMu=-u^TM^Tv=u^TMv$ because the variables anticommute and $M^T=-M$. The real quadratic matrix is consequently $A=\operatorname{diag}(M,M)$, of size $2n$. The linear change of [Grassmann variables](../../../linear-algebra.md#grassmann-variable) has a constant nonzero [Berezin integration](../../../quantum-mechanics.md#berezin-integral) Jacobian, so it changes only the allowed normalization factor. For even $n$, the two blocks give

$$
\boxed{\operatorname{Pf}(A)=\operatorname{Pf}(M)^2=\det M.}
$$

For odd $n$, $\det M=\det(-M)=(-1)^n\det M$ implies $\det M=0$. Each of the separate $u$ and $v$ quadratic exponentials has only even degree and cannot saturate an odd number of variables, so the real integral vanishes too. This covers the odd case without attempting to define a [Pfaffian](../../../linear-algebra.md#pfaffian) of an odd-dimensional matrix.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Let a [gauge transformation](../../../electromagnetism.md#gauge-transformation) act infinitesimally as $\delta A_\mu^a=(D_\mu\omega)^a$, and define the [Faddeev-Popov operator](../../../relativistic-quantum-field.md#faddeev-popov-operator) by variation of the chosen gauge functional:

$$
\mathcal M^{ab}[A](x,y)=\left.\frac{\delta\mathcal F^a[A^\omega](x)}{\delta\omega^b(y)}\right|_{\omega=0}.
$$

Work in a perturbative [regular gauge slice](../../../relativistic-quantum-field.md#regular-gauge-slice), with boundary conditions that remove residual zero modes and with one local representative of each [gauge orbit](../../../relativistic-quantum-field.md#gauge-orbit). The [Faddeev-Popov gauge-orbit identity](../../../relativistic-quantum-field.md#faddeev-popov-gauge-orbit-identity) is $1=\Delta_{\mathrm{FP}}[A]\int\mathcal D\omega\,\delta[\mathcal F[A^\omega]]$. Inserting it and factoring out the formal gauge-group volume gives

$$
\boxed{Z=\mathcal N\int\mathcal DA\,\delta[\mathcal F[A]]\det\mathcal M[A]\,e^{iS[A]}.}
$$

The functional delta imposes the gauge condition at every point and for every color. The [determinant](../../../linear-algebra.md#determinant) compensates the gauge-orbit Jacobian. For ordinary unoriented real gauge-orbit integration the local Jacobian is $|\det\mathcal M|$; perturbatively its sign is fixed and absorbed into $\mathcal N$, leaving the displayed [determinant](../../../linear-algebra.md#determinant). Multiple global intersections, or a [Gribov ambiguity](../../../relativistic-quantum-field.md#gribov-ambiguity), require more care; the local perturbative formula is not a global uniqueness assertion.

The complex [Grassmann Gaussian integral](../../../quantum-field-theory.md#grassmann-gaussian-integral) now generalizes to spacetime and color indices. Introduce independent anticommuting [Faddeev-Popov ghost fields](../../../relativistic-quantum-field.md#faddeev-popov-ghost) $c^a(x),\bar c^a(x)$ and write

$$
\det\mathcal M[A]=\mathcal N'\int\mathcal D\bar c\,\mathcal Dc\,\exp\left(i\int d^dx\,d^dy\,\bar c^a(x)\mathcal M^{ab}[A](x,y)c^b(y)\right).
$$

The factors $i$ in the [functional determinant](../../../quantum-field-theory.md#functional-determinant) differ from a real exponential only by a regulated, field-independent constant. These [Grassmann fields](../../../quantum-field-theory.md#grassmann-field) are Lorentz scalars in the adjoint color representation; the antighost is independent of the ghost rather than an ordinary complex-conjugate commuting variable. They are unphysical fields, not external observable particles. Representing the [functional determinant](../../../quantum-field-theory.md#functional-determinant) by a local ghost [action](../../../classical-mechanics.md#action) when $\mathcal F$ is local makes ordinary [Feynman rules](../../../perturbative-quantum-field-theory.md#feynman-rule) available. Anticommutation gives the minus sign of a closed ghost loop, enabling cancellation of unphysical gauge contributions and maintaining the gauge identities in perturbation theory.

For example, the linear covariant choice $\mathcal F^a=\partial^\mu A_\mu^a$ gives $\mathcal M^{ab}=\partial^\mu D_\mu^{ab}$, so non-abelian ghost-gauge interactions remain. In an [axial gauge](../../../relativistic-quantum-field.md#axial-gauge) $\mathcal F^a=n^\mu A_\mu^a$ with constant $n$, however,

$$
\mathcal M^{ab}=\delta^{ab}n\cdot\partial+gf^{acb}n\cdot A^c\quad\longrightarrow\quad\delta^{ab}n\cdot\partial
$$

on the exact gauge slice. Its [determinant](../../../linear-algebra.md#determinant) is field-independent, so **axial-gauge ghosts decouple** and contribute only a normalization factor. This statement uses the strict delta-functional constraint; a finite-width Gaussian gauge weight is not the same exact slice.

The disadvantage is that choosing $n$ obscures manifest Lorentz covariance and the [axial-gauge propagator](../../../relativistic-quantum-field.md#axial-gauge-propagator) contains spurious $1/(n\cdot k)$ poles. An [axial-gauge pole prescription](../../../relativistic-quantum-field.md#axial-gauge-pole-prescription) and control of residual transformations satisfying $n\cdot\partial\omega=0$ are necessary; formal decoupling alone does not fix those problems.

**Abelian ghosts do not always decouple.** In a field-independent linear [Lorenz gauge](../../../electromagnetism.md#lorenz-gauge-condition), $\delta A_\mu=\partial_\mu\omega$ gives $\mathcal M=\Box$ and they are free. But the [quadratic Abelian gauge fixing](../../../relativistic-quantum-field.md#quadratic-abelian-gauge-fixing) $\mathcal F[A]=\partial\cdot A+\kappa A_\mu A^\mu$ gives

$$
\delta\mathcal F=(\Box+2\kappa A^\mu\partial_\mu)\omega.
$$

Its [Faddeev-Popov operator](../../../relativistic-quantum-field.md#faddeev-popov-operator) depends on $A$, and the ghost [action](../../../classical-mechanics.md#action) contains $2\kappa\bar c A^\mu\partial_\mu c$. This is an explicit abelian ghost-gauge interaction. Abelianity removes the commutator term in the [gauge transformation](../../../electromagnetism.md#gauge-transformation), not the field dependence of an arbitrary nonlinear gauge condition.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2003](../../2003.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
