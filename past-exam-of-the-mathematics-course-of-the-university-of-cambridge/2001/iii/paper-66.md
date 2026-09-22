# Paper 66

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2001/Paper66.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2001/Paper66.pdf)

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
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)

## 1

↑ **Parent:** [Paper 66](paper-66.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

In [conformal gauge](../../../string-theory.md#conformal-gauge), variation of the flat-background [Polyakov action](../../../string-theory.md#polyakov-action) gives the bulk [wave equation](../../../wave-equation.md) and the endpoint term

$$
\delta S_{\partial}=-\frac1{2\pi\alpha'}\int d\tau\,\left[\partial_\sigma X_\mu\,\delta X^\mu\right]_{\sigma=0}^{\sigma=\pi}.
$$

For each endpoint and target-space direction, two basic choices make this term vanish. A [Neumann boundary condition](../../../differential-equation.md#neumann-boundary-condition) allows arbitrary $\delta X^\mu$ and requires $\partial_\sigma X^\mu=0$. A [Dirichlet boundary condition](../../../differential-equation.md#dirichlet-boundary-condition) fixes $X^\mu$ at the endpoint, hence $\delta X^\mu=0$; for a fixed endpoint location its time derivative also vanishes. Thus

$$
\boxed{\text{Neumann: }\partial_\sigma X^\mu=0;\qquad
\text{Dirichlet: }X^\mu|_{\partial\Sigma}=y^\mu.}
$$

Both are consistent with the [principle of stationary action](../../../classical-mechanics.md#principle-of-stationary-action) and zero energy flux through a stationary endpoint. Different directions can use different conditions. Background two-form or boundary gauge fields can modify tangential conditions into mixed ones; the displayed alternatives are the basic flat, unforced choices.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

The common [Neumann boundary conditions](../../../differential-equation.md#neumann-boundary-condition) define a $(p+1)$-dimensional timelike [worldvolume](../../../string-theory.md#worldvolume): one time direction and $p$ spatial directions. The remaining [Dirichlet boundary conditions](../../../differential-equation.md#dirichlet-boundary-condition) fix its transverse position. An open string therefore ends on a [D-brane](../../../string-theory.md#d-brane) of spatial dimension $p$, a D$p$-brane. For the critical [bosonic string theory](../../../string-theory.md#bosonic-string-theory) there are $25-p$ transverse directions.

If the Dirichlet constants agree at the two endpoints, both ends lie on the same planar [D-brane](../../../string-theory.md#d-brane). If they differ, the string stretches between two parallel [D-branes](../../../string-theory.md#d-brane) with the same orientation but different positions. **Neumann directions are tangent to the brane; Dirichlet directions are transverse to it.** The brane is dynamical: tangential massless open-string polarizations supply a gauge field, while transverse ones describe its displacement, as in [worldvolume fields from open-string massless states](../../../string-theory.md#worldvolume-fields-from-open-string-massless-states). The unprojected bosonic brane also has a [tachyon](../../../physics.md#tachyon); the boundary-condition interpretation does not make that ground state supersymmetrically stable.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

A supersymmetric type-II [D-brane](../../../string-theory.md#d-brane) carries a [Ramond–Ramond potential](../../../string-theory.md#ramond-ramond-potential) charge and saturates the corresponding generalized [BPS bound in supersymmetry](../../../supersymmetry.md#bps-bound-in-supersymmetry): its [brane tension](../../../string-theory.md#brane-tension) equals the charge-dependent central/tensorial-charge bound in the relevant normalization. It is therefore a [BPS state](../../../supersymmetry.md#bps-state), preserving sixteen of the thirty-two spacetime [supercharges](../../../supersymmetry.md#supersymmetry-generator). Identical parallel branes with the same orientation impose the same supersymmetry projector. This statement does not apply to arbitrary unstable non-BPS branes or to the bosonic branes of the preceding parts.

One direct demonstration of the [parallel D-brane no-force identity](../../../string-theory.md#parallel-d-brane-no-force-identity) is the annulus vacuum amplitude. For separation $r$, its oscillator-dependent part is proportional to

$$
\mathcal A(r)\propto V_{p+1}\int_0^\infty\frac{dt}{2t}(8\pi^2\alpha't)^{-(p+1)/2}
e^{-r^2t/(2\pi\alpha')}
\frac{f_3(q)^8-f_4(q)^8-f_2(q)^8}{f_1(q)^8},\qquad q=e^{-\pi t}.
$$

Here

$$
\begin{aligned}
f_1(q)&=q^{1/12}\prod_{n\ge1}(1-q^{2n}),&
f_2(q)&=\sqrt2\,q^{1/12}\prod_{n\ge1}(1+q^{2n}),\\
f_3(q)&=q^{-1/24}\prod_{n\ge1}(1+q^{2n-1}),&
f_4(q)&=q^{-1/24}\prod_{n\ge1}(1-q^{2n-1}).
\end{aligned}
$$

The first two terms describe the projected [Neveu–Schwarz sector](../../../string-theory.md#neveu-schwarz-sector), and the last is the oppositely signed [Ramond sector](../../../string-theory.md#ramond-sector) contribution. The [Jacobi abstruse identity](../../../modular-function.md#jacobi-abstruse-identity) gives $f_3^8-f_4^8-f_2^8=0$ for every $t$. Therefore

$$
\boxed{\mathcal A(r)=0,\qquad -\frac{dV(r)}{dr}=0.}
$$

In the closed-string channel, attractive [graviton](../../../quantum-theory.md#graviton) and [dilaton](../../../string-theory.md#dilaton) exchange cancel repulsive [Ramond–Ramond potential](../../../string-theory.md#ramond-ramond-potential) exchange. The classical probe calculation in the [D-brane supergravity solution](../../../string-theory.md#d-brane-supergravity-solution) gives the same cancellation. The common supersymmetry allows separation to remain a flat modulus; relative angles, reversed RR charge or supersymmetry-breaking backgrounds can remove this protection. For a brane–antibrane pair the RR interaction reverses and does not cancel the NS-NS attraction. The charge and half-supersymmetry interpretation is established in [Dirichlet-Branes and Ramond-Ramond Charges](https://arxiv.org/abs/hep-th/9510017).

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

For $N$ parallel type-II [D-branes](../../../string-theory.md#d-brane), an oriented open string has endpoint labels $i,j$, its [Chan-Paton factors](../../../string-theory.md#chan-paton-factor). At coincidence, the massless states form $N\times N$ matrices, giving adjoint fields of $U(N)$. Tangential polarizations produce the [Yang-Mills theory](../../../relativistic-quantum-field.md#yang-mills-theory) gauge field; transverse polarizations produce $9-p$ adjoint [scalar fields](../../../quantum-field-theory.md#scalar-field). The leading low-energy action is the dimensional reduction of [ten-dimensional super Yang-Mills theory](../../../supersymmetry.md#ten-dimensional-super-yang-mills-theory) to $p+1$ dimensions. Expanding the [Dirac-Born-Infeld action](../../../string-theory.md#dirac-born-infeld-action) gives the gauge and scalar kinetic terms, while dimensional reduction supplies the [Hermitian commutator potential in D-brane Yang-Mills theory](../../../string-theory.md#hermitian-commutator-potential-in-d-brane-yang-mills-theory):

$$
V=-\frac1{4g_{\rm YM}^2}\sum_{I,J}\operatorname{Tr}[\phi^I,\phi^J]^2\ge0.
$$

The sign is important: for Hermitian $\phi$, the commutator is anti-Hermitian. Zero potential requires commuting scalars, whose simultaneous eigenvalues are brane positions through the [D-brane scalar-position normalization](../../../string-theory.md#d-brane-scalar-position-normalization)

$$
Y_i^I=2\pi\alpha'\langle\phi_i^I\rangle.
$$

This makes the [Higgs mechanism](../../../standard-model.md#higgs-mechanism) geometrical. Separating branes gives masses to strings joining different positions; bringing them together gives [Coincident-D-brane gauge enhancement](../../../string-theory.md#coincident-d-brane-gauge-enhancement).

Two parallel [D3-branes](../../../string-theory.md#d3-brane) in [type IIB superstring theory](../../../string-theory.md#type-iib-superstring-theory) give [four-dimensional N=4 super Yang-Mills theory](../../../supersymmetry.md#four-dimensional-n-4-super-yang-mills-theory) with gauge group $U(2)$, containing a gauge field, six real adjoint [scalar fields](../../../quantum-field-theory.md#scalar-field) and four adjoint [Weyl fermions](../../../relativistic-quantum-field.md#weyl-spinor). On its [Coulomb branch](../../../supersymmetry.md#coulomb-branch), choose

$$
\langle\phi^I\rangle=\frac1{2\pi\alpha'}\begin{pmatrix}Y_1^I&0\\0&Y_2^I\end{pmatrix}.
$$

For distinct position vectors, $U(2)$ breaks to $U(1)\times U(1)$. The off-diagonal vector multiplets are the two orientations of a string joining the branes, and

$$
\boxed{m_W=\frac{|Y_1-Y_2|}{2\pi\alpha'}.}
$$

The same mass follows from the scalar covariant-derivative term, $m_W^2=\sum_I(\phi_1^I-\phi_2^I)^2$. The overall $U(1)$ describes center-of-mass motion; the relative $SU(2)$ sector is Higgsed to its Cartan $U(1)$. At coincidence the off-diagonal states become massless and the full $U(2)$ gauge symmetry is restored.

<h3 id="1/e">e</h3>

↑ **Parent:** [1](#1)

<h4 id="1/e/solution">Solution</h4>

↑ **Parent:** [E](#1/e)

A [D-brane](../../../string-theory.md#d-brane) is a localized RR-charged source whose long-distance fields solve [supergravity](../../../supersymmetry.md#supergravity). The extremal charged $p$-brane solutions carry the same RR charges, [brane tension](../../../string-theory.md#brane-tension) and preserved supersymmetry as the open-string construction. For the standard asymptotically flat cases $p<7$, the [D-brane supergravity solution](../../../string-theory.md#d-brane-supergravity-solution) in the [string frame](../../../string-theory.md#string-frame-metric) is

$$
ds_s^2=H^{-1/2}ds^2(\mathbb R^{1,p})+H^{1/2}dy_\perp^2,\qquad
e^\Phi=g_sH^{(3-p)/4},\qquad H=1+\frac Q{r^{7-p}}.
$$

The function $H$ is a positive [harmonic function](../../../partial-differential-equation.md#harmonic-function) away from the source, in $9-p$ transverse dimensions. In an electric gauge, $C_{0\cdots p}=g_s^{-1}(H^{-1}-1)$, with its orientation chosen to match the source. Magnetic branes use the dual flux; for the [D3-brane](../../../string-theory.md#d3-brane), the five-form includes both electric and magnetic pieces and is self-dual. [Killing spinors](../../../supersymmetry.md#killing-spinor) obey one brane projector, leaving sixteen supersymmetries. Aligned multicenter harmonic functions describe several branes with no static binding force.

To check this identification directly, insert an equally oriented static probe into the solution. Put $\mu_p=(2\pi)^{-p}\alpha'^{-(p+1)/2}$, so the asymptotic tension is $\mu_p/g_s$. The induced-volume factor is $H^{-(p+1)/4}$; combined with $e^{-\Phi}$, its [DBI action](../../../string-theory.md#dirac-born-infeld-action) density is $-\mu_p g_s^{-1}H^{-1}$. Its [Wess-Zumino brane coupling](../../../string-theory.md#wess-zumino-brane-coupling) contributes $+\mu_p g_s^{-1}(H^{-1}-1)$. Hence the total static Lagrangian density is the constant $-\mu_p/g_s$, independently of position. This gives the [parallel D-brane no-force identity](../../../string-theory.md#parallel-d-brane-no-force-identity) in the spacetime description.

The supergravity background is the back-reacted, coarse long-distance description, while the boundary-condition description exposes the light open-string degrees of freedom. Controlled use of supergravity requires curvature small in string units and suitable local coupling. Singular cores and the special codimension-two or domain-wall cases are not automatically resolved by the elementary harmonic ansatz.

## 2

↑ **Parent:** [Paper 66](paper-66.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

A $(p+1)$-form [gauge potential](../../../relativistic-quantum-field.md#gauge-field) $A_{p+1}$ couples electrically to a spatial $p$-brane through the [Wess-Zumino brane coupling](../../../string-theory.md#wess-zumino-brane-coupling)

$$
S_{\rm charge}=e\int_{\Sigma_{p+1}}X^*A_{p+1}.
$$

The [worldvolume](../../../string-theory.md#worldvolume) dimension supplies exactly the degree required for integration. Under $A\mapsto A+d\Lambda$, the change is $e\int_{\partial\Sigma}X^*\Lambda$, so a closed worldvolume is gauge invariant; an open one needs suitable endpoint couplings. If $F_{p+2}=dA_{p+1}$ has an ordinary dual potential, $*F$ has degree $d-p-2$ and the dual potential degree $d-p-3$. Thus the [electric and magnetic dimensions of a form-coupled brane](../../../string-theory.md#electric-and-magnetic-dimensions-of-a-form-coupled-brane) are

$$
\boxed{p_{\rm electric}=p,\qquad p_{\rm magnetic}=d-p-4.}
$$

Electric charge is measured by $\int_{S^{d-p-2}}*F$, magnetic charge by $\int_{S^{p+2}}F$, on spheres linking the corresponding objects. Flux normalization, and possible Chern-Simons modifications of charge definitions, must be fixed in interacting backgrounds; this is the basic linear form-field dictionary.

In ten dimensions the common NS-NS fields are the [graviton](../../../quantum-theory.md#graviton) $g_{\mu\nu}$, [Kalb–Ramond field](../../../string-theory.md#kalb-ramond-field) $B_2$, and [dilaton](../../../string-theory.md#dilaton) $\Phi$. Their on-shell bosonic polarizations are $35,28,1$, respectively. The graviton count is $10(10-3)/2=35$, and a massless $k$-form has $\binom8k$ transverse polarizations. The RR fields distinguish the two theories:

| Theory | RR potentials and physical polarizations | Total bosons | Fermions and chiralities |
| --- | --- | --- | --- |
| [Type IIA superstring theory](../../../string-theory.md#type-iia-superstring-theory) | $C_1:8$, $C_3:56$ | $35+28+1+8+56=128$ | Two opposite-chirality Majorana-Weyl [gravitini](../../../supersymmetry.md#gravitino); two opposite-chirality Majorana-Weyl [dilatini](../../../supersymmetry.md#dilatino) |
| [Type IIB superstring theory](../../../string-theory.md#type-iib-superstring-theory) | $C_0:1$, $C_2:28$, $C_4:35$ with self-dual $F_5$ | $35+28+1+1+28+35=128$ | Two same-chirality Majorana-Weyl [gravitini](../../../supersymmetry.md#gravitino); two same-chirality Majorana-Weyl [dilatini](../../../supersymmetry.md#dilatino) of the opposite chirality to the gravitini |

Each gravitino has $56$ physical polarizations, and each dilatino $8$, giving $128$ fermions in either theory. In IIA the two supersymmetry sectors have opposite ten-dimensional chiralities, and the dilatino in each sector has chirality opposite to its gravitino. In IIB both gravitini can be designated positive-chirality and both dilatini negative-chirality. The self-duality of the IIB five-form halves the unconstrained four-form count $\binom84=70$ to $35$. These are the [massless type IIA spectrum](../../../string-theory.md#massless-type-iia-spectrum) and [massless type IIB spectrum](../../../string-theory.md#massless-type-iib-spectrum), not raw component counts.

The [Neveu–Schwarz two-form](../../../string-theory.md#neveu-schwarz-two-form) couples electrically to the [fundamental string](../../../string-theory.md#fundamental-string) and magnetically to the [NS5-brane](../../../string-theory.md#ns5-brane) in both theories. IIA $C_1$ couples electrically to a [D0-brane](../../../string-theory.md#d0-brane) and magnetically to a [D6-brane](../../../string-theory.md#d6-brane); $C_3$ couples electrically to a [D2-brane](../../../string-theory.md#d2-brane) and magnetically to a [D4-brane](../../../string-theory.md#d4-brane). The magnetic descriptions use dual seven-form and five-form potentials, not extra independent polarizations. In IIB, $C_2$ gives [D1-brane](../../../string-theory.md#d1-brane) and [D5-brane](../../../string-theory.md#d5-brane) charges, while self-dual $C_4$ gives the self-dual [D3-brane](../../../string-theory.md#d3-brane). The scalar $C_0$ couples to a Euclidean [D-instanton](../../../string-theory.md#d-instanton), whose magnetic partner is the [D7-brane](../../../string-theory.md#d7-brane). Momentum and, after circle compactification, [Kaluza-Klein monopole](../../../physics.md#kaluza-klein-monopole) charge come from the metric sector.

The full brane inventory also involves nonpropagating top-form potentials. A [D8-brane](../../../string-theory.md#d8-brane) is an IIA domain-wall source for [Romans mass](../../../supersymmetry.md#romans-mass) $F_0$, described dually by a nine-form potential; it is not generated by the propagating $C_1,C_3$ massless spectrum alone. A space-filling IIB [D9-brane](../../../string-theory.md#d9-brane) has a ten-form coupling and requires appropriate global RR-charge consistency. Such fields add no ordinary massless polarizations. This distinction avoids confusing the list of propagating particles with all possible charged extended objects.

For [T-duality](../../../string-theory.md#t-duality), compactify a spatial coordinate with $X^9\sim X^9+2\pi R$. Closed strings have integer momentum $n$ and winding $w$, with

$$
p_L=\frac nR+\frac{wR}{\alpha'},\qquad p_R=\frac nR-\frac{wR}{\alpha'}.
$$

The map

$$
\boxed{R'=\frac{\alpha'}R,\qquad n'=w,\qquad w'=n}
$$

leaves $p_L$ unchanged and reverses $p_R$. Equivalently, it reverses $X_R^9$ while keeping $X_L^9$, and reverses the corresponding right-moving worldsheet fermion to preserve worldsheet supersymmetry. Multiplication of the right Ramond ground-state spinor by $\Gamma^9$ reverses its ten-dimensional chirality. Left and right Ramond projections therefore change from opposite chirality to equal chirality, or conversely:

$$
\boxed{\text{IIA on }S_R^1\quad\longleftrightarrow\quad\text{IIB on }S_{\alpha'/R}^1.}
$$

The zero-mode mass contribution $(n/R)^2+(wR/\alpha')^2$ and the oscillator spectrum are unchanged. The [Buscher dilaton shift](../../../string-theory.md#buscher-dilaton-shift) gives $g_s'=g_s\sqrt{\alpha'}/R$, which preserves the nine-dimensional gravitational coupling proportional to $g_s^2/R$. The mixed metric and two-form components along the circle are exchanged; RR potentials with a circle leg map to one lower degree and those without it to one higher degree, in the corresponding gauge-covariant description.

For open strings, the derivative relations $\partial_\tau\widetilde X=\partial_\sigma X$ and $\partial_\sigma\widetilde X=\partial_\tau X$ exchange [Neumann boundary conditions](../../../differential-equation.md#neumann-boundary-condition) with [Dirichlet boundary conditions](../../../differential-equation.md#dirichlet-boundary-condition). Consequently a wrapped D$p$-brane becomes a D$(p-1)$-brane, while a transverse one becomes a wrapped D$(p+1)$-brane. The even-dimensional IIA branes and odd-dimensional IIB branes therefore transform consistently with the closed-string chirality flip; transverse positions and compact gauge [Wilson lines](../../../relativistic-quantum-field.md#wilson-line) are exchanged.

## 3

↑ **Parent:** [Paper 66](paper-66.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

Retain only fields independent of the circle coordinate $y$, with coordinate period $2\pi r_0$. Use the [string-frame metric](../../../string-theory.md#string-frame-metric) $g_{\mu\nu}$ and the [circle reduction of eleven-dimensional supergravity](../../../supersymmetry.md#circle-reduction-of-eleven-dimensional-supergravity) ansatz

$$
ds_{11}^2=e^{-2\Phi/3}g_{\mu\nu}dx^\mu dx^\nu+e^{4\Phi/3}(dy-C_1)^2,\qquad
A_3=C_3+B_2\wedge dy.
$$

The minus sign in the fibre one-form is a convention chosen to give the usual $\widetilde F_4=dC_3-C_1\wedge H_3$ below; changing the sign of $C_1$ consistently changes no physics. The metric supplies the ten-dimensional graviton, [dilaton](../../../string-theory.md#dilaton) and RR one-form, while the eleven-dimensional three-form supplies the [Kalb–Ramond field](../../../string-theory.md#kalb-ramond-field) and RR three-form. Define

$$
\eta=dy-C_1,\quad F_2=dC_1,\quad H_3=dB_2,\quad G_4=dC_3,\quad
\widetilde F_4=G_4-C_1\wedge H_3.
$$

Then $F_4^{(11)}=\widetilde F_4+H_3\wedge\eta$. In particular $d\widetilde F_4=-F_2\wedge H_3$, the reduced [Bianchi identity](../../../fiber-bundle.md#bianchi-identity). The field strength, not bare $dC_3$ alone, is the gauge-covariant horizontal component.

For the gravitational term, the block determinant gives

$$
\sqrt{-G}=e^{-8\Phi/3}\sqrt{-g}.
$$

A useful two-step curvature calculation first removes the overall factor $e^{-2\Phi/3}$. The intermediate metric $d\bar s^2=ds_s^2+e^{2\Phi}\eta^2$ has

$$
\bar R=R[g]-\frac14e^{2\Phi}F_{2,\mu\nu}F_2^{\mu\nu}-2\nabla^2\Phi-2(\nabla\Phi)^2,
\qquad \bar\nabla^2\Phi=\nabla^2\Phi+(\nabla\Phi)^2.
$$

The eleven-dimensional conformal-curvature identity then gives

$$
R[G]=e^{2\Phi/3}\left[\bar R+\frac{20}3\bar\nabla^2\Phi-10(\bar\nabla\Phi)^2\right].
$$

Combining the terms yields

$$
\sqrt{-G}R[G]=\sqrt{-g}\left\{
e^{-2\Phi}\left[R+\frac{14}3\nabla^2\Phi-\frac{16}3(\nabla\Phi)^2\right]
-\frac14F_{2,\mu\nu}F_2^{\mu\nu}\right\}.
$$

Integration by parts gives $\int\sqrt{-g}e^{-2\Phi}\nabla^2\Phi=2\int\sqrt{-g}e^{-2\Phi}(\nabla\Phi)^2$ modulo boundary terms. Therefore the [Einstein-Hilbert action](../../../general-relativity.md#einstein-hilbert-action) produces

$$
\sqrt{-g}\left[e^{-2\Phi}(R+4(\nabla\Phi)^2)-\frac14F_{2,\mu\nu}F_2^{\mu\nu}\right].
$$

This explicitly derives both the string-frame dilaton kinetic coefficient and the RR one-form kinetic term.

Use the normalized form norm $|F_k|^2=F_{\mu_1\cdots\mu_k}F^{\mu_1\cdots\mu_k}/k!$, interpreting the printed four-form square in this convention. The horizontal and fibre pieces are orthogonal in the $\eta$ basis. Four horizontal inverse metrics contribute $e^{8\Phi/3}$ to $|\widetilde F_4|_{11}^2$. Three horizontal inverse metrics and one fibre inverse metric contribute $e^{2\Phi/3}$ to $|H_3\wedge\eta|_{11}^2$. Thus

$$
\sqrt{-G}|F_4^{(11)}|^2=\sqrt{-g}\left[|\widetilde F_4|^2+e^{-2\Phi}|H_3|^2\right].
$$

The NS-NS three-form has the same $e^{-2\Phi}$ prefactor as gravity; the RR kinetic terms do not have it in the [string frame](../../../string-theory.md#string-frame-metric).

Finally reduce the topological term using the coordinate decomposition, which makes its signs transparent. The part of $A_3\wedge F_4^{(11)}\wedge F_4^{(11)}$ containing exactly one $dy$ is

$$
\left[B_2\wedge G_4\wedge G_4+2C_3\wedge G_4\wedge H_3\right]\wedge dy.
$$

The purely horizontal eleven-form vanishes on the ten-dimensional base. Since

$$
d(C_3\wedge B_2\wedge G_4)=B_2\wedge G_4\wedge G_4-C_3\wedge H_3\wedge G_4,
$$

integration over the base turns the bracket into $3B_2\wedge G_4\wedge G_4$, modulo the displayed exact term. The [reduction of the eleven-dimensional Chern-Simons term](../../../supersymmetry.md#reduction-of-the-eleven-dimensional-chern-simons-term) therefore gives $-\tfrac12\int B_2\wedge G_4\wedge G_4$.

Absorbing the coordinate circumference into $\kappa_{10}^2=\kappa_{11}^2/(2\pi r_0)$, the complete bosonic massless [type IIA supergravity](../../../supersymmetry.md#type-iia-supergravity) action in these conventions is

$$
\boxed{\begin{aligned}
S_{10}=\frac1{2\kappa_{10}^2}\Bigg\{&\int d^{10}x\sqrt{-g}\left[
e^{-2\Phi}\left(R+4(\nabla\Phi)^2-\frac12|H_3|^2\right)
-\frac12|F_2|^2-\frac12|\widetilde F_4|^2\right]\\
&-\frac12\int B_2\wedge G_4\wedge G_4\Bigg\}.
\end{aligned}}
$$

Dropping boundary terms assumes appropriate boundary conditions; nontrivial flux bundles may require patchwise potentials. Higher circle modes and higher-derivative corrections are excluded by this low-energy zero-mode reduction. No Romans-mass term arises from the ordinary ansatz.

The [M-theory origin of type IIA D-branes](../../../string-theory.md#m-theory-origin-of-type-iia-d-branes) follows by momentum, wrapping and magnetic geometry:

| IIA object | Eleven-dimensional origin | Charge interpretation |
| --- | --- | --- |
| [D0-brane](../../../string-theory.md#d0-brane) | Momentum along the M-circle, or its gravitational wave solution | Electric charge of the circle vector $C_1$ |
| [D2-brane](../../../string-theory.md#d2-brane) | Unwrapped [M2-brane](../../../string-theory.md#m2-brane) | Electric charge of $C_3$ |
| [D4-brane](../../../string-theory.md#d4-brane) | [M5-brane](../../../string-theory.md#m5-brane) wrapped once around the circle | Magnetic charge dual to $C_3$ |
| [D6-brane](../../../string-theory.md#d6-brane) | [Kaluza-Klein monopole](../../../physics.md#kaluza-klein-monopole) with the M-circle as its Taub–NUT fibre | Magnetic charge of $C_1$ |

An [M2-brane](../../../string-theory.md#m2-brane) wrapped around the circle gives the [fundamental string](../../../string-theory.md#fundamental-string), and an unwrapped [M5-brane](../../../string-theory.md#m5-brane) gives the [NS5-brane](../../../string-theory.md#ns5-brane). These are NS objects rather than D-branes. In physical string/Planck units, the [M-theory circle duality](../../../string-theory.md#m-theory-circle-duality) relations are

$$
R_{11}=g_s\ell_s,\qquad\ell_p^3=g_s\ell_s^3,\qquad\ell_s^2=\alpha'.
$$

They involve the physical asymptotic radius, distinguished from the arbitrary coordinate period used in the reduction ansatz. For example, $m_{D0}=1/(g_s\ell_s)=1/R_{11}$ is one momentum quantum. With $T_{M2}=1/[(2\pi)^2\ell_p^3]$ and $T_{M5}=1/[(2\pi)^5\ell_p^6]$,

$$
T_{D2}=T_{M2},\qquad
T_{D4}=2\pi R_{11}T_{M5}=\frac1{(2\pi)^4g_s\ell_s^5},\qquad
T_{F1}=2\pi R_{11}T_{M2}=\frac1{2\pi\ell_s^2}.
$$

The [D6-brane](../../../string-theory.md#d6-brane) is purely gravitational in eleven dimensions, rather than an elementary six-dimensional membrane; the circle-fibration magnetic charge gives its ten-dimensional interpretation.

A [D8-brane](../../../string-theory.md#d8-brane) is the important qualification. It sources the zero-form flux of [massive type IIA supergravity](../../../supersymmetry.md#massive-type-iia-supergravity) and is not obtained as an ordinary wrapped M2/M5 or Kaluza-Klein object of the undeformed circle reduction above. Its extended/generalized lifts are outside this simple dictionary. The massless-circle interpretation of the other branes is developed in [Four Lectures on M-theory](https://arxiv.org/abs/hep-th/9612121).

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2001](../../2001.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
