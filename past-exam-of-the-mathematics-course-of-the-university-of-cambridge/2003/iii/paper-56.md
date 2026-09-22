# Paper 56

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2003/Paper56.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2003/Paper56.pdf)

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

↑ **Parent:** [Paper 56](paper-56.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

The [positive energy theorem](../../../general-relativity.md#positive-energy-theorem) concerns the total gravitational energy of isolated systems, rather than a pointwise gravitational energy density. Its standard asymptotically flat form is

$$
\boxed{E_{\rm ADM}\geq |\mathbf P_{\rm ADM}|.}
$$

Here are the hypotheses used in a spinorial proof. Take smooth, complete, three-dimensional [initial data in general relativity](../../../general-relativity.md#initial-data-in-general-relativity) $(\Sigma,h,k)$ with a [spin structure](../../../riemannian-geometry.md#spin-structure), no inner boundary, and finitely many asymptotically Euclidean ends. Assume the usual differentiable falloff $h_{ij}-\delta_{ij}=O(r^{-1})$, $\partial h=O(r^{-2})$, $k_{ij}=O(r^{-2})$, with sufficiently decaying further derivatives and integrable matter densities. The [Hamiltonian constraint](../../../numerical-relativity.md#hamiltonian-constraint) and [momentum constraint](../../../numerical-relativity.md#momentum-constraint) must hold, and the matter must satisfy the [dominant energy condition](../../../general-relativity.md#dominant-energy-condition). These hypotheses exclude a naked singularity or an unaccounted boundary flux from the argument. An oriented three-manifold admits a [spin structure](../../../riemannian-geometry.md#spin-structure); in higher dimensions the spinorial proof needs this as an additional assumption. Work in signature $(-+++)$ and units $G=c=1$.

Let $n$ be the future unit normal, choose $k_{ij}=-g(\nabla_i n,e_j)$, and define $\mu=T_{ab}n^an^b$ and $J_i=-T_{ab}n^ae_i^b$. With this convention the [Hamiltonian constraint](../../../numerical-relativity.md#hamiltonian-constraint) and [momentum constraint](../../../numerical-relativity.md#momentum-constraint) read

$$
R(h)+(\operatorname{tr}k)^2-|k|^2=16\pi\mu,
\qquad D^j(k_{ij}-h_{ij}\operatorname{tr}k)=8\pi J_i.
$$

The [dominant energy condition](../../../general-relativity.md#dominant-energy-condition) implies $\mu\geq |J|_h$. The asymptotic charges are the [ADM energy](../../../general-relativity.md#arnowitt-deser-misner-energy) and [ADM momentum](../../../general-relativity.md#adm-momentum),

$$
E=\frac1{16\pi}\lim_{r\to\infty}\int_{S_r}(\partial_jh_{ij}-\partial_ih_{jj})s^i\,dS,
\qquad P_i=\frac1{8\pi}\lim_{r\to\infty}\int_{S_r}(k_{ij}-h_{ij}\operatorname{tr}k)s^j\,dS.
$$

These are boundary charges; a sign condition on $\mu$ alone does not visibly determine their sign.

Choose [gamma matrices](../../../algebra.md#gamma-matrices) obeying $\{\gamma^a,\gamma^b\}=2g^{ab}$, with spatial matrices Hermitian and $\gamma^{\hat0}$ anti-Hermitian. The relevant derivative is the [Sen spinor connection](../../../general-relativity.md#sen-spinor-connection), not just the intrinsic [spin connection](../../../connection-1-form.md#spin-connection):

$$
\nabla_i\epsilon=D_i^{(3)}\epsilon-\frac12k_{ij}\gamma^j\gamma^{\hat0}\epsilon,
\qquad \mathcal D\epsilon=\gamma^i\nabla_i\epsilon.
$$

The symmetric [extrinsic curvature](../../../differential-geometry.md#extrinsic-curvature) makes $\mathcal D=\gamma^iD_i^{(3)}-\tfrac12(\operatorname{tr}k)\gamma^{\hat0}$. This is an [elliptic differential operator](../../../distribution-theory.md#elliptic-differential-operator) with the ordinary spatial [Dirac operator](../../../riemannian-geometry.md#dirac-operator) as principal part. Solve the [Witten spinor equation](../../../general-relativity.md#witten-spinor-equation) $\mathcal D\epsilon=0$, with $\epsilon\to\epsilon_\infty$ constant at the end under consideration and zero asymptotic constants at any other ends.

The central algebraic ingredient is the [Witten-Nester identity](../../../general-relativity.md#witten-nester-identity). Define $\bar\epsilon=-\epsilon^\dagger\gamma^{\hat0}$, the future-directed [Dirac current](../../../quantum-field-theory.md#dirac-current) $K^a=\bar\epsilon\gamma^a\epsilon$, and the [Nester two-form](../../../general-relativity.md#nester-two-form)

$$
B^{ab}=\bar\epsilon\gamma^{abc}\nabla_c\epsilon-\overline{\nabla_c\epsilon}\gamma^{abc}\epsilon,
\qquad b^i=n_aB^{ai}.
$$

In an orthonormal frame $K^0=|\epsilon|^2$. Since $-\gamma^{\hat0}\gamma^i q_i$ is Hermitian with eigenvalues $\pm1$ for any unit spatial vector $q$, $|\mathbf K|\leq K^0$. Thus the [Dirac current](../../../quantum-field-theory.md#dirac-current) is future causal. Differentiate the [Nester two-form](../../../general-relativity.md#nester-two-form) by the product rule. The antisymmetric second-derivative terms reduce using the [spinor curvature identity](../../../connection-1-form.md#spinor-curvature-identity)

$$
[\nabla_a,\nabla_b]\epsilon=\frac14R_{ab cd}\gamma^{cd}\epsilon.
$$

The [Clifford algebra](../../../algebra.md#clifford-algebra) and the first [Bianchi identity](../../../fiber-bundle.md#bianchi-identity) turn the curvature contraction into the [Einstein tensor](../../../general-relativity.md#einstein-tensor). The spatial derivative terms give the difference of two squares. Projecting onto $\Sigma$ therefore gives

$$
D_i b^i=2\bigl(|\nabla_i\epsilon|^2-|\mathcal D\epsilon|^2\bigr)+G_{ab}n^aK^b
=2\bigl(|\nabla_i\epsilon|^2-|\mathcal D\epsilon|^2\bigr)+8\pi T_{ab}n^aK^b.
$$

The constraints are exactly the normal components of the [Einstein field equations](../../../general-relativity.md#einstein-field-equations) needed here. Moreover,

$$
T_{ab}n^aK^b=\mu K^0-J_iK^i\geq(\mu-|J|)K^0\geq0.
$$

For a solution of the [Witten spinor equation](../../../general-relativity.md#witten-spinor-equation), both terms left in this divergence are nonnegative.

There is an essential analytic step: an asymptotically constant [spinor field](../../../riemannian-geometry.md#spinor-field) solving the [Witten spinor equation](../../../general-relativity.md#witten-spinor-equation) must actually exist. Extend the chosen constant smoothly from infinity to a field $\epsilon_0$. Then $\mathcal D\epsilon_0=O(r^{-2})$ is square-integrable. For compactly supported fields $\eta$, the same [Witten-Nester identity](../../../general-relativity.md#witten-nester-identity) has zero boundary flux and gives

$$
\|\mathcal D\eta\|_2^2=\|\nabla\eta\|_2^2+4\pi\int_\Sigma T_{ab}n^aK^b[\eta]\,dV\geq\|\nabla\eta\|_2^2.
$$

The asymptotically Euclidean [Hardy inequality in Euclidean space](../../../sobolev-space.md#hardy-inequality-in-euclidean-space), local elliptic estimates and this identity supply the coercive estimate in the weighted first-order [Sobolev space](../../../sobolev-space.md) of decaying corrections. One way to see why a compact-region error cannot spoil coercivity is to assume the estimate fails and take a normalized sequence whose [Dirac operator](../../../riemannian-geometry.md#dirac-operator) tends to zero. Local compactness and the estimate on the ends produce a decaying homogeneous solution. Integrating the identity with cutoffs shows that such a solution is parallel for the [Sen spinor connection](../../../general-relativity.md#sen-spinor-connection). A parallel field tending to zero at infinity is zero, contradicting its normalization. The end estimates exclude escape of the normalized sequence to infinity.

More constructively, on this completed correction space solve

$$
\int_\Sigma\langle\mathcal D\eta,\mathcal D\chi\rangle\,dV
=-\int_\Sigma\langle\mathcal D\epsilon_0,\mathcal D\chi\rangle\,dV
$$

for every compactly supported $\chi$, using the [Lax-Milgram theorem](../../../functional-analysis.md#lax-milgram-theorem). Set $\epsilon=\epsilon_0+\eta$. Since $\mathcal D$ is formally skew-adjoint in the positive spatial spinor inner product, the residual $\xi=\mathcal D\epsilon$ is a square-integrable weak solution of $\mathcal D\xi=0$. Elliptic regularity makes it smooth. Cutoff integration of the identity excludes a nonzero square-integrable homogeneous solution: it would be parallel, whereas a nonzero parallel field has nonzero limiting norm on an asymptotically Euclidean end and cannot be square-integrable. Hence $\xi=0$. Weighted elliptic estimates then give the required asymptotic decay of $\eta$. This supplies [elliptic existence of a Witten spinor](../../../general-relativity.md#elliptic-existence-of-a-witten-spinor), rather than assuming it from the sign of a formal integral.

Finally integrate the [Witten-Nester identity](../../../general-relativity.md#witten-nester-identity) over $\Sigma$. The [ADM boundary term of the Nester two-form](../../../general-relativity.md#adm-boundary-term-of-the-nester-two-form) is

$$
\lim_{r\to\infty}\int_{S_r}b^is_i\,dS=8\pi(EK^0_\infty-P_iK^i_\infty).
$$

To identify this boundary term, expand the asymptotic [spin connection](../../../connection-1-form.md#spin-connection) to first order in $h-\delta$. Its flux is half of $(\partial_jh_{ij}-\partial_ih_{jj})s^iK^0_\infty$; the [extrinsic curvature](../../../differential-geometry.md#extrinsic-curvature) contribution is $-(k_{ij}-h_{ij}\operatorname{tr}k)s^jK^i_\infty$. Their coefficients give precisely the two charges displayed above. The derivative of the decaying spinor correction has zero leading integrated flux by antisymmetry, and the higher-order terms vanish with the falloff. Thus

$$
EK^0_\infty-P_iK^i_\infty
=\frac1{4\pi}\int_\Sigma|\nabla\epsilon|^2\,dV+
\int_\Sigma T_{ab}n^aK^b\,dV\geq0.
$$

Choose a normalized asymptotic [spinor field](../../../riemannian-geometry.md#spinor-field) that is an eigenvector with eigenvalue $+1$ of $-\gamma^{\hat0}\gamma^i q_i$. Then $K^0_\infty=1$ and $\mathbf K_\infty=q$. Choosing $q=\mathbf P/|\mathbf P|$ proves $E\geq|\mathbf P|$; if $\mathbf P=0$, any such choice gives $E\geq0$. This is positivity in every asymptotic frame, not only the zero-momentum case.

The zero-energy rigidity also follows from the vanishing integrals. If $E=0$, then $\mathbf P=0$ and the construction for a basis of asymptotic spinors produces a basis of parallel fields. Their [spinor curvature identity](../../../connection-1-form.md#spinor-curvature-identity) forces the spatially pulled-back spacetime curvature to vanish; the nonnegative matter terms vanish too. The resulting [Gauss–Codazzi equations](../../../second-fundamental-form.md#gauss-codazzi-equations) are those of a hypersurface in [Minkowski spacetime](../../../special-relativity.md#minkowski-spacetime), and its vacuum development is flat. Completeness and the ordinary Euclidean asymptotic end rule out a nontrivial flat quotient. The initial hypersurface need not have $k=0$: a curved spacelike slice of [Minkowski spacetime](../../../special-relativity.md#minkowski-spacetime) also has zero [ADM energy](../../../general-relativity.md#arnowitt-deser-misner-energy). **The proof works by converting an asymptotic energy charge into a nonnegative bulk integral, with the spinor equation and its existence supplying the crucial bridge.**

## 2

↑ **Parent:** [Paper 56](paper-56.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

Use units $G=\hbar=c=k_B=1$ and put $\ell=\sqrt{3/\Lambda}$. The [static patch of de Sitter spacetime](../../../general-relativity.md#static-patch-of-de-sitter-spacetime) has radial factor $f=1-r^2/\ell^2$. A [Wick rotation](../../../perturbative-quantum-field-theory.md#wick-rotation) $t=-i\tau$ makes its radial-time metric positive:

$$
ds_E^2=f\,d\tau^2+\frac{dr^2}{f}+r^2d\Omega_2^2.
$$

Near the [cosmological horizon](../../../general-relativity.md#cosmological-horizon), write $r=\ell-\rho^2/(2\ell)$. Then $f=\rho^2/\ell^2+O(\rho^4)$ and

$$
ds_E^2=d\rho^2+\rho^2d(\tau/\ell)^2+\ell^2d\Omega_2^2+O(\rho^2)
$$

in the radial-time directions. Thus $\tau/\ell$ must be an angle of period $2\pi$. A larger integer multiple would give a conical excess rather than a smooth origin. The [Euclidean black-hole regularity condition](../../../general-relativity.md#euclidean-black-hole-regularity-condition) gives

$$
\boxed{\beta=2\pi\ell=2\pi\sqrt{3/\Lambda},\qquad T=\beta^{-1}=\frac1{2\pi}\sqrt{\Lambda/3}.}
$$

This [de Sitter horizon temperature](../../../general-relativity.md#de-sitter-horizon-temperature) uses the time normalization at $r=0$, where $t$ is [proper time](../../../special-relativity.md#proper-time); static observers at other radii see the corresponding [Tolman temperature law](../../../thermodynamics.md#tolman-ehrenfest-relation) redshift.

Vary the gravitational [Euclidean action](../../../perturbative-quantum-field-theory.md#euclidean-action) with respect to $g^{ab}$. The identities $\delta\sqrt g=-\tfrac12\sqrt g\,g_{ab}\delta g^{ab}$ and the integrated variation of the [scalar curvature](../../../second-fundamental-form.md#scalar-curvature) yield, after discarding the assumed boundary term,

$$
\delta I_E=-\frac1{16\pi}\int\sqrt g\,\left(R_{ab}-\frac12Rg_{ab}+\Lambda g_{ab}\right)\delta g^{ab}\,d^4x.
$$

The resulting vacuum [Einstein field equations](../../../general-relativity.md#einstein-field-equations) are therefore

$$
\boxed{R_{ab}-\frac12Rg_{ab}+\Lambda g_{ab}=0.}
$$

Tracing in four dimensions gives $R=4\Lambda$, and substitution gives $R_{ab}=\Lambda g_{ab}$.

The smooth Euclidean geometry is compact. Explicitly, in Euclidean five-space use

$$
X_0=\sqrt{\ell^2-r^2}\cos(\tau/\ell),\quad
X_1=\sqrt{\ell^2-r^2}\sin(\tau/\ell),\quad
(X_2,X_3,X_4)=r\,\mathbf n,\quad |\mathbf n|=1.
$$

These obey $\sum X_A^2=\ell^2$ and induce precisely the above metric, so $0\leq r\leq\ell$ with the identified Euclidean time covers a round four-sphere once. Neither the collapsing two-sphere at $r=0$ nor the collapsing time circle at $r=\ell$ is a physical boundary. Since $\sqrt g=r^2\sin\theta$, its volume and on-shell [Euclidean action](../../../perturbative-quantum-field-theory.md#euclidean-action) are

$$
\operatorname{Vol}=\beta\,4\pi\int_0^\ell r^2dr=\frac{8\pi^2\ell^4}{3}=\frac{24\pi^2}{\Lambda^2},
\qquad
\boxed{I_E=-\frac{2\Lambda}{16\pi}\operatorname{Vol}=-\frac{3\pi}{\Lambda}.}
$$

The semiclassical [partition function](../../../statistical-physics.md#canonical-partition-function) is $Z\simeq e^{-I_E}$, and $I_E=\beta F=\beta E-S$ follows from the [free energy](../../../thermodynamics.md#thermodynamic-free-energy) relation $F=E-TS$. With the stipulated zero internal energy,

$$
\boxed{S=-I_E=\frac{3\pi}{\Lambda}=\frac{A_H}{4},\qquad A_H=4\pi\ell^2.}
$$

Thus the [Euclidean de Sitter action and entropy](../../../general-relativity.md#euclidean-de-sitter-action-and-entropy) reproduce the [Bekenstein-Hawking entropy](../../../general-relativity.md#bekenstein-hawking-entropy) of the [cosmological horizon](../../../general-relativity.md#cosmological-horizon) without a boundary contribution. Restoring constants, $S=k_Bc^3A_H/(4G\hbar)$.

## 3

↑ **Parent:** [Paper 56](paper-56.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

Take $M>0$ and write $f=1-2M/r$. Integrating $dr_*/dr=f^{-1}$ gives the [Schwarzschild tortoise coordinate](../../../general-relativity.md#schwarzschild-tortoise-coordinate)

$$
r_*=r+2M\log\left|\frac r{2M}-1\right|.
$$

The advanced and retarded [Eddington-Finkelstein coordinates](../../../general-relativity.md#eddington-finkelstein-coordinates) are respectively $v=t+r_*$ and $u=t-r_*$. Substituting $dt=dv-dr/f$ or $dt=du+dr/f$ gives

$$
\boxed{ds^2=-f\,dv^2+2\,dv\,dr+r^2d\Omega_2^2,}
\qquad
\boxed{ds^2=-f\,du^2-2\,du\,dr+r^2d\Omega_2^2.}
$$

Both radial-time blocks have determinant $-1$ and smooth coefficients at $r=2M$. Consequently the [Schwarzschild event horizon](../../../general-relativity.md#schwarzschild-event-horizon) is a coordinate singularity of the original chart, not a degeneracy of the geometry. The [Kretschmann scalar](../../../general-relativity.md#kretschmann-scalar) $48M^2/r^6$ is finite there, while it diverges at $r=0$. Angular coordinate degeneracies at the polar axes are removed separately by ordinary sphere charts.

The [Ingoing Eddington-Finkelstein coordinates](../../../general-relativity.md#ingoing-eddington-finkelstein-coordinates) extend the right exterior through its future [black hole](../../../general-relativity.md#black-hole) horizon. Radial [null geodesics](../../../special-relativity.md#null-geodesic) obey either $dv=0$ or $dr/dv=f/2$. Inside $r=2M$, the latter also moves towards smaller $r$ as $v$ increases, and the future-directed ingoing family has decreasing $r$. Thus neither family can escape to the exterior. The future horizon is the boundary separating points that can send signals to future [null infinity](../../../general-relativity.md#null-infinity) from those that cannot. The retarded chart extends through the past horizon instead. Reversing the time orientation gives the [white hole](../../../general-relativity.md#white-hole): future-directed signals can leave it, but exterior signals cannot enter it. These are distinct branches in the eternal extension; the white-hole branch need not occur in a spacetime formed by collapse.

For a simultaneous extension through both branches, start in the right exterior and define the [Kruskal–Szekeres coordinates](../../../general-relativity.md#kruskal-szekeres-coordinates)

$$
U=-e^{-u/(4M)},\qquad V=e^{v/(4M)}.
$$

Their product and the extended metric are

$$
\boxed{UV=\left(1-\frac r{2M}\right)e^{r/(2M)},\qquad
 ds^2=-\frac{32M^3}{r}e^{-r/(2M)}\,dU\,dV+r^2d\Omega_2^2.}
$$

Indeed $du=-4M\,dU/U$ and $dv=4M\,dV/V$ transform $-f\,du\,dv$ into the displayed expression. The function of $r$ on the right of the product relation has derivative $-r e^{r/(2M)}/(4M^2)$, nonzero at $r=2M$, so $r$ is a smooth function of $UV$ across zero. The coefficient of $dU\,dV$ there is $-16M^2/e$, finite and nonzero. Allowing either sign of $U,V$ therefore gives the regular maximal extension with $UV<1$ and $r>0$.

With $T_K=(V+U)/2$ and $X_K=(V-U)/2$, the radial metric is a positive multiple of $-dT_K^2+dX_K^2$. The two exterior regions have $(U,V)=(-,+)$ and $(+,-)$. The future interior, or [black hole](../../../general-relativity.md#black-hole) region, has $(+,+)$; the past interior, or [white hole](../../../general-relativity.md#white-hole) region, has $(-,-)$. The [Killing horizons](../../../general-relativity.md#killing-horizon) are $U=0$ and $V=0$, meeting on the [bifurcation surface](../../../general-relativity.md#bifurcation-surface) at $U=V=0$.

For the [Penrose diagram](../../../general-relativity.md#penrose-diagram), compactify the null variables before forming time and space:

$$
\bar U=\arctan U,\qquad \bar V=\arctan V,\qquad
T=\frac{\bar V+\bar U}{2},\qquad X=\frac{\bar V-\bar U}{2}.
$$

This [Schwarzschild conformal compactification](../../../general-relativity.md#schwarzschild-conformal-compactification) preserves radial null directions because $dU\,dV=\sec^2\bar U\sec^2\bar V\,(dT^2-dX^2)$. The ranges $|\bar U|,|\bar V|<\pi/2$ bound the diagram, and $UV<1$ cuts off its future and past tips. On $UV=1$ with $U,V>0$, $\bar U+\bar V=\pi/2$, so the future [curvature singularity](../../../general-relativity.md#curvature-singularity) is $T=\pi/4$. The past [curvature singularity](../../../general-relativity.md#curvature-singularity) is similarly $T=-\pi/4$. Both have $|X|<\pi/4$ and are spacelike. The horizon lines remain $T=\pm X$.

<a id="3/image-penrose-diagram-of-maximally-extended-schwarzschild-spacetime-with-two-exteriors-black-and-white-hole-interiors-horizons-and-conformal-infinities"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-56-schwarzschild-penrose.png)

**[Figure 1](#3/image-penrose-diagram-of-maximally-extended-schwarzschild-spacetime-with-two-exteriors-black-and-white-hole-interiors-horizons-and-conformal-infinities). Penrose diagram of maximally extended Schwarzschild spacetime, with two exteriors, black and white hole interiors, horizons and conformal infinities**.

Each point of this radial [Penrose diagram](../../../general-relativity.md#penrose-diagram) represents a two-sphere, except at limiting boundaries. Each exterior has its own future and past [null infinity](../../../general-relativity.md#null-infinity), $\mathscr I^+$ and $\mathscr I^-$. For example in the right exterior, $V\to\infty$ at fixed $U<0$ gives $\mathscr I^+$, whereas $U\to-\infty$ at fixed $V>0$ gives $\mathscr I^-$. Its [spacelike infinity](../../../general-relativity.md#spacelike-infinity) is $(T,X)=(0,\pi/2)$; its future and past [timelike infinity](../../../general-relativity.md#timelike-infinity) are the vertices $(\pi/4,\pi/4)$ and $(-\pi/4,\pi/4)$. The left exterior has the reflected counterparts. These conformal boundary points are ideal endpoints, not finite-distance spacetime events; the physical affine or proper parameters of escaping geodesics diverge.

The horizons are regular null surfaces, while the horizontal $r=0$ boundaries are genuine [curvature singularities](../../../general-relativity.md#curvature-singularity). The central point represents the regular [bifurcation surface](../../../general-relativity.md#bifurcation-surface), not a singularity. Future-directed radial causal curves have nondecreasing $U,V$, so a curve cannot go from one exterior to the other: changing the requisite signs would require one null variable to decrease. Crossing a future horizon instead leads towards the future singularity. **The maximal extension has two causally disconnected exteriors, a future black-hole region and a past white-hole region.**

## 4

↑ **Parent:** [Paper 56](paper-56.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

Let $f(r)=1-2M/r+Q^2/r^2$. A positive-radius horizon requires a root of $r^2-2Mr+Q^2=0$, giving

$$
r_\pm=M\pm\sqrt{M^2-Q^2}.
$$

For the usual asymptotically flat [Reissner-Nordstrom spacetime](../../../general-relativity.md#reissner-nordstrom-spacetime), the black-hole conditions are

$$
\boxed{M>0,\qquad M\geq |Q|.}
$$

The strict inequality gives a nonextremal outer [event horizon](../../../general-relativity.md#event-horizon) at $r_+$; equality gives an [extremal black hole](../../../general-relativity.md#extremal-black-hole). If $M<|Q|$ with $M>0$, there is no horizon and the central [curvature singularity](../../../general-relativity.md#curvature-singularity) is naked. Nonpositive $M$ cannot supply a positive-radius black-hole horizon; $M=Q=0$ is [Minkowski spacetime](../../../special-relativity.md#minkowski-spacetime). For $Q=0$, the zero root $r_-=0$ is the singularity, not an additional regular horizon.

In the static coordinates the vector $k=\partial_t$ has constant components and every metric component is independent of $t$. Its [Lie derivative](../../../differential-form.md#lie-derivative-of-a-differential-form) therefore satisfies

$$
(\mathcal L_k g)_{ab}=k^c\partial_cg_{ab}+g_{cb}\partial_ak^c+g_{ac}\partial_bk^c=0.
$$

For the torsion-free [Levi-Civita connection](../../../general-relativity.md#levi-civita-connection), $\mathcal L_k g=2\nabla_{(a}k_{b)}$, proving the [Killing equation](../../../general-relativity.md#killing-equation) directly. This also normalizes the [Killing vector field](../../../general-relativity.md#killing-vector-field) to unit time translation at infinity.

At $r=r_+$, $k^2=-f=0$. Use the regular advanced chart $v=t+r_*$ with $dr_*/dr=f^{-1}$, in which

$$
ds^2=-f\,dv^2+2\,dv\,dr+r^2d\Omega_2^2,\qquad k=\partial_v.
$$

On the horizon, $k_a=(dr)_a$. Thus the [Killing vector field](../../../general-relativity.md#killing-vector-field) is both null and normal to the horizon, and its orbits generate that [Killing horizon](../../../general-relativity.md#killing-horizon). The normal lines of a [null hypersurface](../../../general-relativity.md#null-hypersurface) are [null geodesics](../../../special-relativity.md#null-geodesic), possibly with nonaffine parameter. To see this without assuming a separate geodesic property, the [Killing equation](../../../general-relativity.md#killing-equation) gives

$$
k^a\nabla_a k_b=-k^a\nabla_b k_a=-\frac12\nabla_b(k^2)=\frac12f'(r)(dr)_b.
$$

Restriction to the future horizon therefore gives

$$
k^a\nabla_a k_b=\frac12f'(r_+)k_b.
$$

The acceleration is proportional to the tangent, which is exactly the [geodesic equation](../../../riemannian-geometry.md#geodesic-equation) with a nonaffine parameter. An affinely parametrized tangent can be obtained by rescaling $k$ along each generator; that rescaled vector need not itself extend to a spacetime [Killing vector field](../../../general-relativity.md#killing-vector-field). At a nonextremal [bifurcation surface](../../../general-relativity.md#bifurcation-surface), $k$ vanishes, so a nonzero generator tangent must be described in a regular affine parametrization there.

On the past branch, use the retarded chart with radial-time cross term $-2\,du\,dr$. Now $k_a=-(dr)_a$ at the horizon, so the same calculation yields the opposite signed nonaffinity. Since $r_+$ is constant and the spacetime is spherically symmetric, $f'(r_+)/2$ is constant over the future horizon. This gives the two signs in the horizon relation without assuming their value beforehand.

Factor $f=(r-r_+)(r-r_-)/r^2$. Its derivative at the outer horizon gives the [Reissner-Nordstrom horizon surface gravity](../../../general-relativity.md#reissner-nordstrom-horizon-surface-gravity)

$$
\boxed{\kappa=\frac12 f'(r_+)=\frac{r_+-r_-}{2r_+^2}
=\frac{\sqrt{M^2-Q^2}}{\left(M+\sqrt{M^2-Q^2}\right)^2}.}
$$

It is positive for $M>|Q|$, and at $Q=0$ reduces to the [Schwarzschild surface gravity](../../../general-relativity.md#schwarzschild-surface-gravity) $1/(4M)$. For $M=|Q|>0$, the root is double and $\kappa=0$. Thus **the horizon remains present when its surface gravity vanishes**: it is a [degenerate Killing horizon](../../../general-relativity.md#degenerate-killing-horizon), and $k$ itself has affine parametrization along its nonzero horizon generators. The strictly positive-constant description applies only to the nonextremal case; the zero value is the legitimate extremal limit.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2003](../../2003.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
