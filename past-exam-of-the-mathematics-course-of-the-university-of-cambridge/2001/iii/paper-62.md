# Paper 62

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2001/Paper62.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2001/Paper62.pdf)

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

↑ **Parent:** [Paper 62](paper-62.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Use [canonical quantization](../../../quantum-mechanics.md#canonical-quantization) with $[\hat q,\hat p]=i\hbar$, $\hat p=-i\hbar\partial_q$, and $\hat H=\hat p^2/(2m)+V(\hat q)$. Assume a real [potential energy](../../../classical-mechanics.md#potential-energy) with the regularity and lower-bound conditions needed for a self-adjoint [Hamiltonian](../../../classical-mechanics.md#hamiltonian) and its [Trotter product formula](../../../numerical-analysis.md#lie-product-formula); singular potentials require their domain and limiting prescription to be specified separately. The transition amplitude is $K(\beta,\alpha;T)=\langle\beta|e^{-iT\hat H/\hbar}|\alpha\rangle$.

Take $\delta=T/N$, $q_0=\alpha$, $q_N=\beta$, and choose the left-endpoint [potential energy](../../../classical-mechanics.md#potential-energy) convention. The precise time-sliced [phase-space path integral](../../../quantum-field-theory.md#phase-space-path-integral) is

$$
K_N=\int\prod_{j=1}^{N-1}dq_j\prod_{j=1}^{N}\frac{dp_j}{2\pi\hbar}
\exp\left\{\frac{i}{\hbar}\sum_{j=1}^{N}\left[p_j(q_j-q_{j-1})-\delta\left(\frac{p_j^2}{2m}+V(q_{j-1})\right)\right]\right\}.
$$

The endpoint positions are fixed and the momenta are unconstrained. Its continuum notation is

$$
\boxed{K=\int_{q(0)=\alpha}^{q(T)=\beta}\mathcal Dq\,\mathcal Dp\;
\exp\left[\frac{i}{\hbar}\int_0^T(p\dot q-H(p,q))dt\right],}
$$

where the functional measure means the displayed limit, not an unspecified product of unnormalized measures.

At each slice, complete the square in [momentum](../../../classical-mechanics.md#momentum). With the square-root branch selected by continuation from positive Euclidean time,

$$
\int\frac{dp}{2\pi\hbar}\exp\left[\frac{i}{\hbar}\left(p\Delta q-\frac{\delta p^2}{2m}\right)\right]
=\left(\frac{m}{2\pi i\hbar\delta}\right)^{1/2}
\exp\left[\frac{im(\Delta q)^2}{2\hbar\delta}\right].
$$

Thus the [time-sliced equivalence of phase-space and configuration-space path integrals](../../../quantum-field-theory.md#time-sliced-equivalence-of-phase-space-and-configuration-space-path-integrals) holds already at finite $N$:

$$
K_N=\left(\frac{m}{2\pi i\hbar\delta}\right)^{N/2}
\int\prod_{j=1}^{N-1}dq_j\;
\exp\left\{\frac{i}{\hbar}\sum_{j=1}^{N}\left[\frac{m(q_j-q_{j-1})^2}{2\delta}-\delta V(q_{j-1})\right]\right\}.
$$

This defines the [configuration-space path integral](../../../quantum-field-theory.md#configuration-space-path-integral)

$$
\boxed{K=\int_{q(0)=\alpha}^{q(T)=\beta}\mathcal Dq\;
\exp\left[\frac{i}{\hbar}\int_0^T\left(\frac m2\dot q^2-V(q)\right)dt\right].}
$$

There are $N$ Gaussian prefactors but only $N-1$ coordinate integrations. Omitting that distinction would change the kernel normalization. The paths integrated in the limit need not be differentiable; the kinetic action notation stands for the lattice difference expression.

To identify this with the operator amplitude, normalize $\langle q|p\rangle=(2\pi\hbar)^{-1/2}e^{ipq/\hbar}$. The kernel of one product factor is exactly

$$
\langle q_j|e^{-i\delta\hat p^2/(2m\hbar)}e^{-i\delta V(\hat q)/\hbar}|q_{j-1}\rangle
=\int\frac{dp_j}{2\pi\hbar}\;e^{ip_j(q_j-q_{j-1})/\hbar-i\delta p_j^2/(2m\hbar)-i\delta V(q_{j-1})/\hbar}.
$$

Insert $N-1$ position resolutions of the identity between factors. Their product is precisely $K_N$. The [Trotter product formula](../../../numerical-analysis.md#lie-product-formula) then gives

$$
\left(e^{-iT\hat p^2/(2mN\hbar)}e^{-iTV(\hat q)/(N\hbar)}\right)^N\longrightarrow e^{-iT\hat H/\hbar},
$$

so both functional integrals represent the same canonical kernel. One can define the finite integrals first at $T=-i\tau$, $\tau>0$, where the Gaussian [momentum](../../../classical-mechanics.md#momentum) and coordinate kernels converge, and then continue to the real-time boundary value. Alternatively use an equivalent oscillatory damping prescription. Operator convergence fixes the distributional kernel limit; it need not imply pointwise convergence at every endpoint for every admissible [potential energy](../../../classical-mechanics.md#potential-energy). There is no operator-ordering ambiguity for this separated kinetic-plus-potential [Hamiltonian](../../../classical-mechanics.md#hamiltonian) once the common slicing convention is fixed.

## 2

↑ **Parent:** [Paper 62](paper-62.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

Use [Minkowski spacetime](../../../special-relativity.md#minkowski-spacetime) with signature $(+,-,\ldots,-)$ and $\hbar=1$, with a vacuum time-ordering prescription. At a regulator, define the normalized [generating functional](../../../perturbative-quantum-field-theory.md#generating-functional)

$$
Z[J]=\frac{\int\mathcal D\phi\;e^{i(S[\phi]+\int J\phi)}}{\int\mathcal D\phi\;e^{iS[\phi]}},\qquad Z[0]=1.
$$

The normalized vacuum [correlation functions](../../../critical-phenomenon.md#correlation-function) of a [time-ordered product](../../../perturbative-quantum-field-theory.md#time-ordered-product) are

$$
G_n(x_1,\ldots,x_n)=\left.\frac1{i^n}\frac{\delta^n Z}{\delta J(x_1)\cdots\delta J(x_n)}\right|_{J=0}.
$$

The [connected generating functional](../../../perturbative-quantum-field-theory.md#connected-generating-functional) is

$$
\boxed{W[J]=-i\log Z[J],\qquad
C_n=\left.i^{1-n}\frac{\delta^n W}{\delta J(x_1)\cdots\delta J(x_n)}\right|_{J=0}.}
$$

The logarithm selects connected source diagrams, or equivalently [cumulants](../../../probability-theory.md#cumulant). With the assumed vanishing [one-point function](../../../critical-phenomenon.md#one-point-correlation-function), [derivatives](../../../calculus.md#derivative) of $Z=e^{iW}$ give the [centered four-point cumulant decomposition](../../../perturbative-quantum-field-theory.md#centered-four-point-cumulant-decomposition):

$$
\boxed{G_{1234}=C_{1234}+C_{12}C_{34}+C_{13}C_{24}+C_{14}C_{23}.}
$$

In detail, four differentiations either act on one connected block or form one of three pair partitions. Contributions with blocks of size one vanish. If $W_{ij}$ and $W_{1234}$ denote source [derivatives](../../../calculus.md#derivative) at zero, the same relation is $G_{1234}=iW_{1234}-W_{12}W_{34}-W_{13}W_{24}-W_{14}W_{23}$, since $C_2=-iW_2$ and $C_4=iW_4$.

Let $\varphi(x)=\delta W/\delta J(x)$ be the source-dependent mean field. On a locally invertible source-to-field branch, define the [quantum effective action](../../../perturbative-quantum-field-theory.md#effective-action) by the Minkowski [Legendre transform](../../../convex-optimization.md#convex-conjugate)

$$
\boxed{\Gamma[\varphi]=W[J]-\int d^dx\,J(x)\varphi(x).}
$$

Its variation is $\delta\Gamma=-\int J\delta\varphi$, so $\delta\Gamma/\delta\varphi=-J$. Differentiating the two inverse source-field maps yields the [Minkowski inverse-Hessian relation for an effective action](../../../perturbative-quantum-field-theory.md#minkowski-inverse-hessian-relation-for-an-effective-action):

$$
\boxed{\int d^dz\,\frac{\delta^2\Gamma}{\delta\varphi(x)\delta\varphi(z)}
\frac{\delta^2W}{\delta J(z)\delta J(y)}=-\delta^{(d)}(x-y).}
$$

Thus $\Gamma^{(2)}=-(W^{(2)})^{-1}$. The inverse is understood at the regulator and on a nonsingular fluctuation sector; it is not an assertion that every source-field map is globally invertible.

For a free [real scalar field](../../../scalar-field-theory.md#real-scalar-field), integrate by parts to write

$$
S[\phi]=\frac12\phi A\phi,\qquad A=-\Box-m^2,
\qquad A_\epsilon=A+i\epsilon,
$$

where repeated spacetime variables are integrated. Specify the [propagator](../../../quantum-field-theory.md#propagator) convention explicitly:

$$
\Delta_F(x-y)=\int\frac{d^dp}{(2\pi)^d}\frac{i\,e^{-ip(x-y)}}{p^2-m^2+i0},\qquad \Delta_F=iA_\epsilon^{-1}.
$$

Completing the [Gaussian path integral](../../../quantum-field-theory.md#gaussian-path-integral) around $\phi=-A_\epsilon^{-1}J$ cancels the source-independent [determinant](../../../linear-algebra.md#determinant) between numerator and denominator. Therefore

$$
Z[J]=\exp\left[-\frac i2JA_\epsilon^{-1}J\right],\qquad
\boxed{W[J]=-\frac12JA_\epsilon^{-1}J=\frac i2J\Delta_FJ.}
$$

The positive imaginary term in $A_\epsilon$ damps the oscillatory Gaussian. Together with vacuum projection at the time boundaries, it selects the Feynman poles and the time-ordered, in-out [correlation function](../../../critical-phenomenon.md#correlation-function) rather than a retarded inverse. It can also be obtained by continuation from the Euclidean vacuum integral. A denominator convention without the numerator $i$ redistributes the displayed factors of $i$.

Finally $\varphi=-A_\epsilon^{-1}J$, hence $J=-A_\epsilon\varphi$. Substitution into the [Legendre transform](../../../convex-optimization.md#convex-conjugate) gives the [vacuum-normalized effective action of a free scalar field](../../../perturbative-quantum-field-theory.md#vacuum-normalized-effective-action-of-a-free-scalar-field):

$$
\boxed{\Gamma[\varphi]=\frac12\varphi A_\epsilon\varphi\longrightarrow S[\varphi]\quad(\epsilon\downarrow0).}
$$

All connected functions beyond order two vanish and all proper vertices beyond the classical quadratic kernel vanish. Vacuum normalization fixes the additive constant; without it, the [quantum effective action](../../../perturbative-quantum-field-theory.md#effective-action) equals the classical action up to a field-independent [determinant](../../../linear-algebra.md#determinant) contribution.

## 3

↑ **Parent:** [Paper 62](paper-62.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

For a connected amputated [Feynman diagram](../../../perturbative-quantum-field-theory.md#feynman-diagram), let $L,I,V,E$ denote its independent loops, internal scalar lines, interaction vertices and external lines. Its [superficial degree of divergence](../../../perturbative-quantum-field-theory.md#superficial-degree-of-divergence) counts the simultaneous ultraviolet scaling of all loop momenta: each loop integration contributes $d$ powers and each [scalar propagator](../../../scalar-field-theory.md#scalar-propagator) removes two. A nonderivative interaction adds no numerator powers, so $\Delta=dL-2I$. The graph identities are

$$
nV=2I+E,\qquad L=I-V+1.
$$

The kinetic term gives $[\phi]=(d-2)/2$ and $[\lambda]=d-n(d-2)/2$. Eliminating $I,L$ proves the [monomial scalar interaction power-counting identity](../../../perturbative-quantum-field-theory.md#monomial-scalar-interaction-power-counting-identity):

$$
\boxed{\Delta=d-\frac{d-2}{2}E-[\lambda]V,\qquad\text{order}=\lambda^V.}
$$

For a graph with $C$ connected components the first $d$ is replaced by $dC$, after removing the corresponding overall [momentum](../../../classical-mechanics.md#momentum) delta functions. Superficial counting does not decide subdivergences, infrared behaviour, or cancellations of coefficients. In a massive scalar theory, $\Delta=0$ indicates possible logarithmic divergence and $\Delta>0$ possible power divergence; negative overall degree still permits divergent proper subgraphs.

[Dimensional regularization](../../../perturbative-quantum-field-theory.md#dimensional-regularization) analytically continues the [momentum](../../../classical-mechanics.md#momentum) integration and its angular factors to a complex dimension where a regulated expression is defined, then continues back near the physical dimension. Introduce a scale $\mu$ to keep the renormalized coupling in fixed units. The [minimal subtraction scheme](../../../perturbative-quantum-field-theory.md#minimal-subtraction-scheme) removes only poles in the dimensional regulator, without prescribed finite parts. It differs from [modified minimal subtraction scheme](../../../perturbative-quantum-field-theory.md#modified-minimal-subtraction-scheme), which also absorbs the conventional $\log4\pi-\gamma_E$ combination.

For the cubic calculation, write $g=3!\lambda$, so the interaction is $-g\phi^3/3!$ and the vertex is $-ig$. Use $D=6-2\epsilon$ and the vertex $-ig\mu^\epsilon$. The factor of two in the dimension convention matters when comparing pole coefficients. In six dimensions $[\phi]=2$, $[g]=0$ and a proper two-point graph has $\Delta=2$.

The one-loop [bubble diagram](../../../perturbative-quantum-field-theory.md#bubble-diagram) has [Feynman-diagram symmetry factor](../../../perturbative-quantum-field-theory.md#feynman-diagram-symmetry-factor) two. Define its amputated insertion $B(p)=i\Pi(p)$ explicitly by

$$
B(p)=\frac{(-ig\mu^\epsilon)^2}{2}\int\frac{d^Dk}{(2\pi)^D}
\frac{i}{k^2-m^2+i0}\frac{i}{(k-p)^2-m^2+i0}.
$$

Combine denominators with a [Feynman parameter](../../../perturbative-quantum-field-theory.md#feynman-parameter) $x$ and shift $\ell=k-xp$. With $M_x^2=m^2-x(1-x)p^2$, the dimensionally continued integral gives

$$
B(p)=\frac{ig^2\mu^{2\epsilon}}{2(4\pi)^{D/2}}\Gamma(2-D/2)
\int_0^1dx\,(M_x^2-i0)^{D/2-2}.
$$

This identity follows by [Wick rotation](../../../perturbative-quantum-field-theory.md#wick-rotation) and a [Schwinger parameterization](../../../perturbative-quantum-field-theory.md#schwinger-parameterization), giving the angular Gaussian factor $(4\pi)^{-D/2}$ and the remaining gamma integral. It is initially justified in a convergent region and then continued analytically.

Here $\Gamma(\epsilon-1)=-1/\epsilon+O(1)$ and $\int_0^1x(1-x)dx=1/6$. Thus the [one-loop two-point divergence in six-dimensional cubic scalar theory](../../../scalar-field-theory.md#one-loop-two-point-divergence-in-six-dimensional-cubic-scalar-theory) is

$$
\boxed{B_{\rm div}(p)=-\frac{ig^2}{2(4\pi)^3\epsilon}\left(m^2-\frac{p^2}{6}\right)
=-\frac{18i\lambda^2}{(4\pi)^3\epsilon}\left(m^2-\frac{p^2}{6}\right).}
$$

Writing $\Delta_0(p)=i/(p^2-m^2+i0)$, the proper-bubble contribution to the [propagator](../../../quantum-field-theory.md#propagator) is

$$
\boxed{(\Delta_0B\Delta_0)_{\rm div}
=\frac{ig^2(m^2-p^2/6)}{2(4\pi)^3\epsilon(p^2-m^2+i0)^2}.}
$$

With the defined $B=i\Pi$, resummation gives $i/(p^2-m^2+\Pi+i0)$. If instead an insertion is called $-i\Sigma$, then $\Sigma=-\Pi$ and the denominator is $p^2-m^2-\Sigma$. These naming conventions must not reverse the calculated graph.

For example, the [minimal-subtraction two-point counterterms in cubic scalar theory](../../../scalar-field-theory.md#minimal-subtraction-two-point-counterterms-in-cubic-scalar-theory) can be written

$$
\mathcal L_{\rm ct}=\frac12\delta Z(\partial\phi)^2-\frac12\delta m^2\phi^2,
\qquad
\boxed{\delta Z=-\frac{g^2}{12(4\pi)^3\epsilon},\quad
\delta m^2=-\frac{g^2m^2}{2(4\pi)^3\epsilon}.}
$$

Their insertion $i(\delta Zp^2-\delta m^2)$ cancels the bubble pole. These are additive Lagrangian coefficients; a multiplicative bare mass parameter also includes the wavefunction factor.

There is a vacuum convention to specify because a cubic interaction does not preserve a zero mean field automatically. If no [tadpole subtraction](../../../perturbative-quantum-field-theory.md#tadpole-subtraction) or background shift is imposed, a connected [two-point function](../../../critical-phenomenon.md#two-point-correlation-function) also has a one-particle-reducible one-loop graph with both external legs at one cubic vertex and a [tadpole diagram](../../../perturbative-quantum-field-theory.md#tadpole-diagram) attached to its third leg. For $m>0$, the amputated one-point [tadpole diagram](../../../perturbative-quantum-field-theory.md#tadpole-diagram) is

$$
T_1=\frac{-ig\mu^\epsilon}{2}\int\frac{d^Dk}{(2\pi)^D}\frac{i}{k^2-m^2+i0},
\qquad (T_1)_{\rm div}=-\frac{igm^4}{4(4\pi)^3\epsilon}.
$$

This uses $\Gamma(\epsilon-2)=1/(2\epsilon)+O(1)$. Its mean-field pole is $v_{\rm div}=\Delta_0(0)(T_1)_{\rm div}=-gm^2/[4(4\pi)^3\epsilon]$. The [tadpole contribution to a cubic-theory two-point function](../../../perturbative-quantum-field-theory.md#tadpole-contribution-to-a-cubic-theory-two-point-function) is therefore

$$
B_{{\rm tad},\rm div}=(-ig)v_{\rm div}=\frac{ig^2m^2}{4(4\pi)^3\epsilon}.
$$

In that unshifted convention, the total connected one-loop [propagator](../../../quantum-field-theory.md#propagator) pole is

$$
\boxed{\Delta_{{\rm conn},\rm div}^{(1)}(p)
=\frac{ig^2(m^2/2-p^2/6)}{2(4\pi)^3\epsilon(p^2-m^2+i0)^2}.}
$$

A linear [counterterm](../../../perturbative-quantum-field-theory.md#counterterm) imposing $\langle\phi\rangle=0$ cancels the attached [tadpole diagram](../../../perturbative-quantum-field-theory.md#tadpole-diagram), leaving the usual proper-bubble result above. [Vacuum bubbles](../../../perturbative-quantum-field-theory.md#vacuum-feynman-diagram) cancel by normalization. A disconnected product $\langle\phi\rangle^2$ belongs to the unconnected [two-point function](../../../critical-phenomenon.md#two-point-correlation-function) and has two [tadpole diagram](../../../perturbative-quantum-field-theory.md#tadpole-diagram) loops, so it is outside the requested connected one-loop [propagator](../../../quantum-field-theory.md#propagator) correction. In the massless theory, isolated [tadpole diagrams](../../../perturbative-quantum-field-theory.md#tadpole-diagram) are scaleless and vanish in [dimensional regularization](../../../perturbative-quantum-field-theory.md#dimensional-regularization); an infrared-safe nonzero external scale is still needed to distinguish ultraviolet poles from scaleless integrals.

## 4

↑ **Parent:** [Paper 62](paper-62.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

Choose Hermitian generators $T^a$ of the gauge [Lie algebra](../../../lie-algebra.md), with $[T^a,T^b]=if^{abc}T^c$, and write $A_\mu=A_\mu^aT^a$. For the usual compact gauge algebra choose $\operatorname{tr}(T^aT^b)=\delta^{ab}/2$. More generally use a nondegenerate invariant [symmetric bilinear form](../../../linear-algebra.md#symmetric-bilinear-form) on the algebra in place of this trace contraction; a completely arbitrary component metric would not give gauge invariance.

A matter vector is useful to fix conventions: with $\psi'=U(x)\psi$ and $D_\mu=\partial_\mu-igA_\mu$, require $D_\mu'\psi'=U D_\mu\psi$. Acting on an arbitrary vector gives the [Yang-Mills gauge transformation](../../../relativistic-quantum-field.md#yang-mills-gauge-transformation)

$$
\boxed{A_\mu'=UA_\mu U^{-1}+\frac{i}{g}U\partial_\mu U^{-1},\qquad
D_\mu'=U D_\mu U^{-1}.}
$$

For $U=1+ig\theta+O(\theta^2)$ this becomes

$$
\delta A_\mu=D_\mu\theta=\partial_\mu\theta-ig[A_\mu,\theta],\qquad
(D_\mu\theta)^a=\partial_\mu\theta^a+gf^{abc}A_\mu^b\theta^c.
$$

Here the second $D_\mu$ denotes the induced [derivative](../../../calculus.md#derivative) in the [Adjoint representation](../../../lie-algebra.md#adjoint-representation-of-a-lie-algebra).

Define the curvature by $[D_\mu,D_\nu]=-igF_{\mu\nu}$. Expanding the [commutator](../../../lie-algebra.md#commutator) derives

$$
F_{\mu\nu}=\partial_\mu A_\nu-\partial_\nu A_\mu-ig[A_\mu,A_\nu],\qquad
F_{\mu\nu}^a=\partial_\mu A_\nu^a-\partial_\nu A_\mu^a+gf^{abc}A_\mu^bA_\nu^c.
$$

Since [commutators](../../../lie-algebra.md#commutator) of the transformed [derivatives](../../../calculus.md#derivative) conjugate, $F_{\mu\nu}'=UF_{\mu\nu}U^{-1}$. Cyclicity of the trace proves the [invariant bilinear-form construction of a Yang-Mills action](../../../relativistic-quantum-field.md#invariant-bilinear-form-construction-of-a-yang-mills-action):

$$
\boxed{\mathcal L_{\rm YM}=-\frac12\operatorname{tr}(F_{\mu\nu}F^{\mu\nu})
=-\frac14F_{\mu\nu}^aF^{a\mu\nu}.}
$$

For a general invariant form $h$, the corresponding proof is $h([\theta,X],Y)+h(X,[\theta,Y])=0$, applied to the two curvature factors. No matter field is required in this pure-gauge Lagrangian.

Introduce the adjoint [Faddeev-Popov ghost](../../../relativistic-quantum-field.md#faddeev-popov-ghost) $c^a$ and antighost $\bar c^a$, independent Grassmann-odd scalar fields of [ghost numbers](../../../relativistic-quantum-field.md#ghost-number) $+1$ and $-1$, together with the Grassmann-even [Nakanishi-Lautrup field](../../../relativistic-quantum-field.md#nakanishi-lautrup-field) $b^a$ of [ghost number](../../../relativistic-quantum-field.md#ghost-number) zero. The bar labels the independent antighost, not an additional propagating complex-conjugate matter field. Choose a left [BRST symmetry](../../../relativistic-quantum-field.md#brst-symmetry) differential:

$$
\boxed{sA_\mu^a=(D_\mu c)^a,\qquad
sc^a=-\frac g2f^{abc}c^bc^c,\qquad
s\bar c^a=b^a,\qquad sb^a=0.}
$$

It is an odd derivation: $s(XY)=(sX)Y+(-1)^{|X|}X(sY)$ for homogeneous [Grassmann parity](../../../linear-algebra.md#grassmann-parity) $|X|$. The two relevant properties are $s\mathcal L_{\rm YM}=0$ and off-shell nilpotence $s^2=0$. The first is gauge invariance with parameter replaced by the ghost, and the second follows from the [Lie algebra](../../../lie-algebra.md)'s graded Jacobi identities. Thus

$$
s(\mathcal L_{\rm YM}+s\Psi)=s\mathcal L_{\rm YM}+s^2\Psi=0.
$$

Algebraically this holds for any $\Psi$; a physical gauge-fixing addition uses an odd [gauge-fixing fermion](../../../relativistic-quantum-field.md#gauge-fixing-fermion) of [ghost number](../../../relativistic-quantum-field.md#ghost-number) $-1$ so that $s\Psi$ is even and has [ghost number](../../../relativistic-quantum-field.md#ghost-number) zero.

For [BRST-exact covariant gauge fixing](../../../relativistic-quantum-field.md#brst-exact-covariant-gauge-fixing), choose

$$
\Psi=\bar c^a\left(\partial^\mu A_\mu^a+\frac12b^a\right).
$$

The [graded Leibniz rule](../../../commutative-algebra.md#graded-leibniz-rule) supplies the essential minus sign:

$$
s\Psi=b^a\partial^\mu A_\mu^a+\frac12b^ab^a-\bar c^a\partial^\mu(D_\mu c)^a.
$$

Use [Gaussian gauge fixing with an auxiliary field](../../../relativistic-quantum-field.md#gaussian-gauge-fixing-with-an-auxiliary-field) to integrate $b$. Pointwise,

$$
b^aF^a+\frac12(b^a)^2=\frac12(b^a+F^a)^2-\frac12(F^a)^2,
\qquad F^a=\partial^\mu A_\mu^a.
$$

Translation of the regulated oscillatory Gaussian leaves only a field-independent normalization. The remaining Lagrangian is therefore

$$
\boxed{\mathcal L_{\rm YM}-\frac12(\partial^\mu A_\mu^a)^2
-\bar c^a\partial_\mu(D^\mu c)^a.}
$$

This is covariant [Feynman gauge](../../../relativistic-quantum-field.md#feynman-gauge), with gauge parameter one. Eliminating $b$ need not retain manifest off-shell nilpotence in the reduced field variables; the original auxiliary-field action gives the off-shell [BRST symmetry](../../../relativistic-quantum-field.md#brst-symmetry) formulation.

Finally, the ungauge-fixed quadratic [momentum](../../../classical-mechanics.md#momentum) kernel is

$$
Q_{\mu\nu}^{ab}(p)=\delta^{ab}(-p^2\eta_{\mu\nu}+p_\mu p_\nu),\qquad
Q_{\mu\nu}^{ab}p^\nu=0.
$$

Gauge directions are null vectors, so there is no inverse defining a vector [propagator](../../../quantum-field-theory.md#propagator), and the functional integral also counts an infinite [gauge orbit](../../../relativistic-quantum-field.md#gauge-orbit) volume. The added gauge-fixing term cancels the longitudinal part, leaving $Q_{\mu\nu}^{ab}=-\delta^{ab}p^2\eta_{\mu\nu}$. With the vacuum prescription, the [propagators](../../../quantum-field-theory.md#propagator) are

$$
\boxed{\langle A_\mu^a A_\nu^b\rangle(p)=-\frac{i\delta^{ab}\eta_{\mu\nu}}{p^2+i0},\qquad
\langle c^a\bar c^b\rangle(p)=\frac{i\delta^{ab}}{p^2+i0}.}
$$

The ghost action represents the [Faddeev-Popov determinant](../../../relativistic-quantum-field.md#faddeev-popov-determinant) and supplies ghost-vector vertices; closed ghost loops have the fermionic minus sign. Expanding the cubic and quartic Yang-Mills terms and this ghost interaction now defines consistent perturbative [Feynman rules](../../../perturbative-quantum-field-theory.md#feynman-rule). Physical mass-shell poles remain, whereas the gauge degeneracy has been removed. Possible global gauge-fixing obstructions and boundary zero modes are separate from the perturbative inverse around the trivial vacuum.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2001](../../2001.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
