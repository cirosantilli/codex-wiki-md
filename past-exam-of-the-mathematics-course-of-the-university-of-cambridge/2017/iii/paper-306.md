# Paper 306

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2017/paper_306.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2017/paper_306.pdf)

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

↑ **Parent:** [Paper 306](paper-306.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Set $\hbar=1$. Work on the strip $0\leq\sigma\leq\pi$ in [conformal gauge](../../../string-theory.md#conformal-gauge), with worldsheet signature $(-,+)$ and target signature $(-,+,\ldots,+)$. In [light-cone gauge in string theory](../../../string-theory.md#light-cone-gauge-in-string-theory), the independent fields are the $d=D-2=24$ transverse coordinates. Put the [Neumann boundary condition](../../../differential-equation.md#neumann-boundary-condition) at $\sigma=0$ and the [Dirichlet boundary condition](../../../differential-equation.md#dirichlet-boundary-condition) at $\sigma=\pi$; reversing the endpoints exchanges cosine and sine modes without changing the spectrum. The fixed endpoint is $X^i(\tau,\pi)=y^i$.

Varying the transverse [Polyakov action](../../../string-theory.md#polyakov-action) gives $(\partial_\tau^2-\partial_\sigma^2)X^i=0$ and the spatial boundary contribution $-(2\pi\alpha')^{-1}\int d\tau\,[X'^i\delta X^i]_0^\pi$. At the free endpoint this vanishes precisely when $X'^i=0$; at the fixed endpoint $\delta X^i=0$. [Separation of variables](../../../partial-differential-equation.md#separation-of-variables) then gives $\cos(r\sigma)$ with $\cos(r\pi)=0$, hence $r=n+\tfrac12$, $n=0,1,\ldots$. These are [Neumann-Dirichlet open-string boundary conditions](../../../string-theory.md#neumann-dirichlet-open-string-boundary-condition). No dynamical transverse [worldsheet zero mode](../../../string-theory.md#worldsheet-zero-mode) survives: a constant solution must equal the prescribed $y^i$, and a linear-in-$\sigma$ solution violates the free-end condition.

Write $X^i-y^i=\sum_{r>0}q_r^i(\tau)\cos(r\sigma)$. The [orthogonality](../../../linear-algebra.md#orthogonal-vectors) relation $\int_0^\pi\cos(r\sigma)\cos(s\sigma)d\sigma=(\pi/2)\delta_{rs}$ reduces the action to independent [harmonic oscillators](../../../classical-mechanics.md#simple-harmonic-motion):

$$
S_\perp=\frac1{8\alpha'}\int d\tau\sum_{i=1}^{24}\sum_{r>0}\bigl((\dot q_r^i)^2-r^2(q_r^i)^2\bigr),\qquad P_r^i=\frac{\dot q_r^i}{4\alpha'}.
$$

The [canonical commutation relations](../../../quantum-mechanics.md#canonical-commutation-relation) $[q_r^i,P_s^j]=i\delta^{ij}\delta_{rs}$ determine normalized [annihilation operators](../../../quantum-mechanics.md#annihilation-operator) at $\tau=0$

$$
a_r^i=\sqrt{\frac r{8\alpha'}}q_r^i+i\sqrt{\frac{2\alpha'}r}P_r^i,\qquad
\boxed{[a_r^i,a_s^{j\dagger}]=\delta^{ij}\delta_{rs},\quad[a_r^i,a_s^j]=[a_r^{i\dagger},a_s^{j\dagger}]=0.}
$$

Thus $q_r^i=\sqrt{2\alpha'/r}\,(a_r^ie^{-ir\tau}+a_r^{i\dagger}e^{ir\tau})$. These formulas derive the quantization from the action rather than import integer-moded open-string rules.

For the usual phased [string oscillators](../../../string-theory.md#string-oscillator), set $\alpha_r^i=-i\sqrt r\,a_r^i$ and $\alpha_{-r}^i=i\sqrt r\,a_r^{i\dagger}$ for $r>0$. Then the [half-integer open-string oscillator](../../../string-theory.md#half-integer-open-string-oscillator) expansion and algebra are

$$
X^i=y^i+i\sqrt{2\alpha'}\sum_{r\in\mathbb Z+1/2}\frac{\alpha_r^i}{r}e^{-ir\tau}\cos(r\sigma),\qquad
\boxed{[\alpha_r^i,\alpha_s^j]=r\delta^{ij}\delta_{r+s,0},\quad\alpha_r^{i\dagger}=\alpha_{-r}^i.}
$$

The corresponding field [momentum](../../../classical-mechanics.md#momentum) density is $\Pi_i=\dot X^i/(2\pi\alpha')$. Completeness of the mixed-boundary [eigenfunctions](../../../linear-operator-theory.md#eigenfunction) gives $[X^i(\sigma),\Pi_j(\sigma')]=i\delta^i_j\delta_{\mathrm{ND}}(\sigma,\sigma')$, where $\delta_{\mathrm{ND}}=(2/\pi)\sum_{r>0}\cos(r\sigma)\cos(r\sigma')$. This is a [distribution](../../../distribution-theory.md#distribution-mathematical-analysis) identity on the mixed-boundary function space, not an unrestricted value at a fixed endpoint with a [Dirichlet boundary condition](../../../differential-equation.md#dirichlet-boundary-condition).

Classically, the transverse [Virasoro algebra](../../../string-theory.md#virasoro-algebra) zero-mode generator is

$$
\boxed{L_{0,\mathrm{cl}}^\perp=\frac12\sum_{i=1}^{24}\sum_{r\in\mathbb Z+1/2}\alpha_{-r}^i\alpha_r^i=\sum_{i=1}^{24}\sum_{r>0}\alpha_{-r}^i\alpha_r^i.}
$$

There is no transverse [momentum](../../../classical-mechanics.md#momentum) term. If the two light-cone directions are common directions with [Neumann boundary conditions](../../../differential-equation.md#neumann-boundary-condition), the full zero-mode constraint adds $\alpha'p_\parallel^2=-2\alpha'p^+p^-$: $L_{0,\mathrm{cl}}=\alpha'p_\parallel^2+L_{0,\mathrm{cl}}^\perp$. This assumption about the longitudinal directions is needed to interpret oscillator levels as target-space masses.

Quantizing the symmetrically ordered transverse generator gives $L_0^\perp=N+E_0$, where the [string level operator](../../../string-theory.md#string-level-operator) is $N=\sum_{i,r>0}r a_r^{i\dagger}a_r^i$. Each [harmonic oscillator](../../../classical-mechanics.md#simple-harmonic-motion) contributes $r/2$ to the [vacuum energy](../../../perturbative-quantum-field-theory.md#vacuum-energy). Use [zeta function regularization](../../../complex-analysis.md#zeta-function-regularization) and the [Riemann zeta function](../../../analytic-number-theory.md#riemann-zeta-function) with the actual half-integer spectrum:

$$
\sum_{n\geq0}(n+\tfrac12)^{-s}=(2^s-1)\zeta_R(s),\qquad
\sum_{r>0}^{\mathrm{reg}}r=(2^{-1}-1)\zeta_R(-1)=\frac1{24}.
$$

Consequently the [Neumann-Dirichlet string zero-point energy](../../../string-theory.md#neumann-dirichlet-string-zero-point-energy) is

$$
\boxed{E_0=\frac{24}{2}\frac1{24}=\frac12,\qquad L_0=\alpha'p_\parallel^2+N+\frac12.}
$$

In the common convention $L_0=\alpha'p_\parallel^2+N-a$, the [normal-ordering constant of a string](../../../string-theory.md#normal-ordering-constant-of-a-string) is $a=-\tfrac12$. This positive shift differs from the $-1$ [vacuum energy](../../../perturbative-quantum-field-theory.md#vacuum-energy) of 24 integer-moded transverse [bosons](../../../quantum-mechanics.md#boson). The difference between those two vacuum energies is $3/2$. To distinguish zero-mode conventions, the [ND twist conformal weight](../../../string-theory.md#bosonic-nd-boundary-changing-conformal-weight) is $1/16$ per transverse boson. With 24 bosons, the plane matter generator is $L_0^{\mathrm{plane}}=\alpha'p_\parallel^2+N+3/2$; its physical open-string condition $L_0^{\mathrm{plane}}-1=0$ is exactly the strip/light-cone constraint $\alpha'p_\parallel^2+N+1/2=0$ used here. The transverse plane and strip constants differ by the [central charge](../../../string-theory.md#central-charge) shift $c_\perp/24=24/24=1$. A common exponential frequency cutoff independently gives $\sum_{r>0}r e^{-\varepsilon r}=\varepsilon^{-2}+1/24+O(\varepsilon^2)$, confirming the finite part and avoiding invalid termwise manipulation of divergent sums.

Let $a_r^i|0\rangle=0$. The [lowest levels of a fully transverse ND bosonic string](../../../string-theory.md#lowest-levels-of-a-fully-transverse-nd-bosonic-string) are

$$
\begin{array}{c|c|c|c}
N&\text{states}&L_0^\perp&\text{multiplicity}\\\hline
0&|0\rangle&1/2&1\\
1/2&a_{1/2}^{i\dagger}|0\rangle&1&24\\
1&a_{1/2}^{i\dagger}a_{1/2}^{j\dagger}|0\rangle&3/2&300
\end{array}
$$

The third level has two $r=1/2$ excitations; there is no $r=1$ oscillator. Its indices are symmetric because the [creation operators](../../../quantum-mechanics.md#creation-operator) commute. With $L_0=0$ and the common longitudinal [momentum](../../../classical-mechanics.md#momentum) convention, the rest energies and masses obey

$$
\boxed{\alpha'M^2=\frac12,\ 1,\ \frac32\quad\text{at the first three levels}.}
$$

At fixed positive $p^+$ the corresponding light-cone energies are $p^-=(N+1/2)/(2\alpha'p^+)$; the table lists excitation levels, not a spectrum that remains discrete if longitudinal [momentum](../../../classical-mechanics.md#momentum) is varied continuously.

The surviving transverse rotations form $SO(24)$. The ground state is a [scalar](../../../vector-space.md#scalar), the next level its [vector](../../../vector-space.md#vector), and the third level the [symmetric square](../../../linear-algebra.md#symmetric-square) of the vector. Separating its trace gives

$$
\boxed{\mathbf1,\qquad\mathbf{24},\qquad\operatorname{Sym}^2(\mathbf{24})=\mathbf{299}\oplus\mathbf1.}
$$

The trace state is proportional to $\sum_i(a_{1/2}^{i\dagger})^2|0\rangle$; subtracting this trace gives the 299-dimensional [symmetric traceless square](../../../linear-algebra.md#symmetric-trace-free-square-of-the-defining-orthogonal-representation).

There is a qualification to the printed “little group”. The [little group with mixed string boundary conditions](../../../special-relativity.md#little-group-with-mixed-string-boundary-conditions) must preserve the endpoints as well as [momentum](../../../classical-mechanics.md#momentum). These [boundary conditions](../../../differential-equation.md#boundary-condition) break the full 26-dimensional [Lorentz group](../../../special-relativity.md#lorentz-group), so the massive states above cannot be classified as representations of the unbroken 26-dimensional massive [little group](../../../special-relativity.md#little-group) $SO(25)$. In a D1–D25 realization the common worldvolume has Lorentz group $SO(1,1)$ and trivial connected massive little group; $SO(24)$ acts on the ND coordinates as an internal rotation group. **The scalar, vector and symmetric trace-free decomposition is under the surviving transverse SO(24), with this boundary-background qualification.**

## 2

↑ **Parent:** [Paper 306](paper-306.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

The conformal condition is a quantum [worldsheet Weyl anomaly](../../../string-theory.md#worldsheet-weyl-anomaly) cancellation, not the classical metric equation of the [Polyakov action](../../../string-theory.md#polyakov-action). Assume a smooth target metric, no antisymmetric background field, and curvature/gradient scales large compared with $\sqrt{\alpha'}$. Use $[\nabla_a,\nabla_b]v^c=R^c{}_{dab}v^d$ and $R_{ab}=R^c{}_{acb}$, consistent with the Ricci-scalar [Weyl transformation](../../../string-theory.md#weyl-transformation) in the hint.

A sign convention in the printed action must be made explicit. With worldsheet signature $(-,+)$, continuation $\tau=-i\tau_E$ and $e^{iS_L}=e^{-S_E}$ sends its negative kinetic term to a positive Euclidean kinetic term, while its positive Lorentzian curvature coupling becomes a negative Euclidean curvature coupling. Define the conventional Euclidean [dilaton](../../../string-theory.md#dilaton) by $\varphi=-\Phi$ for this literal action. Then $S_{E,\mathrm{dil}}=(4\pi)^{-1}\int\sqrt h\,R^{(2)}\varphi$. The [Lorentzian dilaton coupling sign convention](../../../string-theory.md#lorentzian-dilaton-coupling-sign-convention) is therefore important: a convention with a negative Lorentzian curvature coupling would instead use $\varphi=\Phi$ and reverse every term linear in the printed $\Phi$ below.

For completeness, the metric part of the one-loop calculation can be obtained by a geodesic [background field expansion of a string sigma model](../../../string-theory.md#background-field-expansion-of-a-string-sigma-model). Write $X=\exp_{\bar X}Y$. Its quadratic Euclidean action contains

$$
S_E^{(2)}=\frac1{4\pi\alpha'}\int\sqrt h\left(g_{ab}D_\mu Y^aD^\mu Y^b-R_{acbd}Y^aY^b\partial_\mu\bar X^c\partial^\mu\bar X^d\right).
$$

Here $D_\mu Y^a=\partial_\mu Y^a+\Gamma^a{}_{bc}\partial_\mu\bar X^bY^c$. In dimension $2-\varepsilon$, the ultraviolet coincident contraction has pole $\langle Y^aY^b\rangle_{\mathrm{div}}=\alpha'g^{ab}/\varepsilon$ with an infrared regulator. Contracting the curvature term gives a divergence $-(4\pi\varepsilon)^{-1}\int\sqrt h\,R_{cd}\partial\bar X^c\partial\bar X^d$. It is cancelled by the metric [counterterm](../../../perturbative-quantum-field-theory.md#counterterm) $\delta g_{ab}=\alpha'R_{ab}/\varepsilon$, giving the one-loop [sigma-model beta function](../../../string-theory.md#sigma-model-beta-function) $\beta^g_{ab}=\alpha'R_{ab}+O(\alpha'^2)$ before the dilaton improvement. Equivalently its local Euclidean Weyl variation is $-(4\pi)^{-1}\int\sqrt h\,\omega R_{ab}\partial X^a\partial X^b$, with terms proportional to the embedding equations understood as field redefinitions.

Set $\Omega=e^\omega$ in the supplied curvature transformation. On a closed [string worldsheet](../../../string-theory.md#worldsheet), [integration by parts](../../../calculus.md#integration-by-parts) gives

$$
\delta_\omega S_{E,\mathrm{dil}}=-\frac1{2\pi}\int\sqrt h\,\varphi\Box_h\omega=-\frac1{2\pi}\int\sqrt h\,\omega\Box_h\varphi.
$$

The chain rule and leading [string embedding map](../../../string-theory.md#string-embedding-map) equation imply

$$
\Box_h\varphi(X)=\nabla_a\nabla_b\varphi\,h^{\mu\nu}\partial_\mu X^a\partial_\nu X^b+\partial_a\varphi\left(\Box_hX^a+\Gamma^a{}_{bc}\partial X^b\partial X^c\right).
$$

The kinetic embedding equation suffices for extracting the leading metric coefficient. More precisely, the full Euclidean embedding equation makes the parenthesis $(\alpha'/2)R^{(2)}\nabla^a\varphi$, giving a curvature contribution $-(\alpha'/4\pi)\int\sqrt h\,\omega R^{(2)}|\nabla\varphi|^2$ to the Weyl variation. This contributes to the scalar coefficient below rather than to the leading metric tensor coefficient. Combining the curvature [counterterm](../../../perturbative-quantum-field-theory.md#counterterm) anomaly with this variation gives the [leading metric-dilaton Weyl condition](../../../string-theory.md#leading-metric-dilaton-weyl-condition):

$$
\boxed{\overline\beta^g_{ab}=\alpha'\bigl(R_{ab}+2\nabla_a\nabla_b\varphi\bigr)+O(\alpha'^2)=0.}
$$

This is the gravitational equation in the [string frame](../../../string-theory.md#string-frame-metric), rather than an ordinary Einstein equation with a minimally coupled scalar. In terms of the field and signs literally printed in this Lorentzian action it reads

$$
\boxed{R_{ab}-2\nabla_a\nabla_b\Phi=0\quad\text{to leading order}.}
$$

The frequently used $R_{ab}+2\nabla_a\nabla_b\Phi=0$ is obtained if the printed $\Phi$ is identified with the conventional Euclidean dilaton, which requires the opposite Lorentzian curvature-coupling sign. Both conventions describe the same mathematics after $\Phi\mapsto-\Phi$, but one cannot change only the field equation silently. Also, vanishing of this tensor coefficient is the metric part of Weyl invariance; the dilaton curvature coefficient and central-charge condition remain to be checked.

Now derive the scalar consequence without presupposing its integration constant. The [contracted Bianchi identity](../../../general-relativity.md#contracted-bianchi-identity) gives $\nabla^aR_{ab}=\tfrac12\nabla_bR$. The [Ricci identity](../../../general-relativity.md#curvature-commutator-on-a-covariant-tensor) applied to the gradient of a scalar gives

$$
\nabla^a\nabla_a\nabla_b\varphi=\nabla_b\Box_g\varphi+R_{ba}\nabla^a\varphi.
$$

Diverging the metric equation and then substituting $R_{ab}=-2\nabla_a\nabla_b\varphi$ yields

$$
0=\frac12\nabla_bR+2\nabla_b\Box_g\varphi-4\nabla_b\nabla_a\varphi\nabla^a\varphi
=\frac12\nabla_b\bigl(R+4\Box_g\varphi-4|\nabla\varphi|^2\bigr).
$$

Thus the bracket is constant on each connected target component. Its trace equation is $R+2\Box_g\varphi=0$, so the [dilaton equation from contracted Bianchi identity](../../../string-theory.md#dilaton-equation-from-contracted-bianchi-identity) becomes

$$
\boxed{\Box_g\varphi-2|\nabla\varphi|^2=C,\qquad \Box_g\Phi+2|\nabla\Phi|^2=-C.}
$$

The second equation uses the literal printed sign convention. These are nonlinear scalar wave equations analogous to the [Klein-Gordon equation](../../../wave-equation.md#klein-gordon-equation). For the [exponentiated dilaton wave equation](../../../string-theory.md#exponentiated-dilaton-wave-equation), put $F=e^{-2\varphi}=e^{2\Phi}$; differentiating twice gives

$$
\boxed{(\Box_g+2C)F=0.}
$$

Here $\Box_g=\nabla^a\nabla_a$ is the Lorentzian [Laplace-Beltrami operator](../../../differential-geometry.md#laplace-beltrami-operator), and $|\nabla\varphi|^2=g^{ab}\partial_a\varphi\partial_b\varphi$ is a Lorentzian contraction, not necessarily nonnegative.

The Bianchi and Ricci identities alone do not imply $C=0$. The [linear dilaton counterexample to zero integration constant](../../../string-theory.md#linear-dilaton-counterexample-to-zero-integration-constant) is flat target space with $\varphi=q_aX^a$: the tensor equation holds for every constant $q$, while $C=-2q^2$. A non-null $q$ disproves any deduction of the zero-constant scalar equation from that tensor equation alone.

The [leading dilaton Weyl anomaly coefficient](../../../string-theory.md#leading-dilaton-weyl-anomaly-coefficient) is obtained as follows. The matter and reparameterization-ghost [central charges](../../../string-theory.md#central-charge) give the constant $(D-26)/6$. Expanding the curvature coupling along the same geodesic fluctuation gives the quadratic term $\tfrac12\nabla_a\nabla_b\varphi\,Y^aY^b$; its coincident contraction is cancelled by $\delta\varphi=-\alpha'\Box_g\varphi/(2\varepsilon)$, giving the term $-\alpha'\Box_g\varphi/2$. The full embedding-equation contribution identified above supplies $+\alpha'|\nabla\varphi|^2$. Therefore full leading-order bosonic-string Weyl invariance also requires

$$
\overline\beta^\varphi=\frac{D-26}{6}+\alpha'\left(-\frac12\Box_g\varphi+|\nabla\varphi|^2\right)+O(\alpha'^2)=0.
$$

It fixes $C=(D-26)/(3\alpha')$. Hence in the critical $D=26$ theory, or under [boundary conditions](../../../differential-equation.md#boundary-condition) making the constant vanish,

$$
\boxed{\Box_g\varphi-2|\nabla\varphi|^2=0,\qquad \Box_g\Phi+2|\nabla\Phi|^2=0,\qquad\Box_g e^{2\Phi}=0.}
$$

This explains precisely the extra input needed for a zero-mass Klein-Gordon-type equation. In noncritical dimension the corresponding equation has the central-charge-deficit constant, subject to the usual controlled-background assumptions.

## 3

↑ **Parent:** [Paper 306](paper-306.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

Use a genus-zero [Polyakov path integral](../../../string-theory.md#polyakov-path-integral), target signature $(-,+,\ldots,+)$ and all four momenta incoming. Define the [Mandelstam variables](../../../special-relativity.md#mandelstam-variables) by $s=-(p_1+p_2)^2$, $t=-(p_1+p_3)^2$, $u=-(p_1+p_4)^2$. The [string mass-shell condition](../../../string-theory.md#string-mass-shell-condition) is $p_i^2=4/\alpha'$ and [momentum](../../../classical-mechanics.md#momentum) conservation is $\sum_i p_i=0$, so

$$
\boxed{s+t+u=-\frac{16}{\alpha'}.}
$$

The reduced amplitude omits the overall momentum-conservation [Dirac delta distribution](../../../distribution-theory.md#dirac-delta-function) and any conventional overall scattering-matrix phase. Interpret each [tachyon vertex operator](../../../string-theory.md#tachyon-vertex-operator) as normal ordered; self-contractions must not be included.

The [free-boson worldsheet propagator](../../../string-theory.md#free-boson-worldsheet-propagator) is $\langle X^a(z)X^b(w)\rangle=-(\alpha'/2)\eta^{ab}\log|z-w|^2$. [Wick theorem](../../../perturbative-quantum-field-theory.md#wick-s-theorem) then evaluates the normal-ordered exponential correlator as the [Koba-Nielsen factor](../../../string-theory.md#koba-nielsen-factor)

$$
\left\langle\prod_{j=1}^4{:}e^{ip_j\cdot X(z_j)}{:}\right\rangle\propto\prod_{i<j}|z_i-z_j|^{\alpha'p_i\cdot p_j}.
$$

The [worldsheet zero mode](../../../string-theory.md#worldsheet-zero-mode) supplies [momentum](../../../classical-mechanics.md#momentum) conservation. Four vertices give $g_s^4$ and the sphere contributes $g_s^{-2}$ through the [string genus expansion](../../../string-theory.md#string-genus-expansion), leaving $g_s^2$.

The sphere's residual [Möbius transformations](../../../group-theory.md#mobius-transformation) fix three insertion points. In [sphere gauge fixing for four string vertices](../../../string-theory.md#sphere-gauge-fixing-for-four-string-vertices), take $(z_1,z_2,z_3,z_4)=(z,0,1,\infty)$. The [worldsheet ghost fields](../../../string-theory.md#worldsheet-ghost-field), equivalently the [Faddeev-Popov determinant](../../../relativistic-quantum-field.md#faddeev-popov-determinant) for this residual group, supply $|z_{23}z_{24}z_{34}|^2$. At finite $z_4$, this determinant grows as $|z_4|^4$, while the matter correlator decays as $|z_4|^{-4}$ by [momentum](../../../classical-mechanics.md#momentum) conservation and the tachyon [mass](../../../classical-mechanics.md#mass) shell; their product has a finite limit. Equivalently the weight-$(1,1)$ matter operator at infinity is normalized with $|z_4|^4$, while the ghost pair uses the inverse factor. After stripping the fixed-position normalization, only

$$
A^{(4)}=g_s^2\int_{\mathbb C}d^2z\,|z|^{-4-\alpha's/2}|1-z|^{-4-\alpha't/2}
$$

remains. Here choose the standard complex-coordinate measure $d^2z=i\,dz\wedge d\bar z=2\,dx\,dy$. With $dx\,dy$ instead, the reduced normalization must acquire a factor two to give the same requested amplitude. Absolute vertex/sphere normalization is a convention; this choice fixes it consistently with the displayed $2\pi$ prefactor.

Set $a=-1-\alpha's/4$, $b=-1-\alpha't/4$, $c=-1-\alpha'u/4$. Then $a+b+c=1$ and the integrand is $|z|^{2a-2}|1-z|^{2b-2}$. To evaluate the [complex beta integral](../../../complex-analysis.md#complex-beta-integral) first work where $\operatorname{Re}a,\operatorname{Re}b,\operatorname{Re}c>0$. This ensures convergence near $0$, $1$ and infinity. Set $v=1-a$ and $w=1-b$. [Schwinger parameterization](../../../perturbative-quantum-field-theory.md#schwinger-parameterization) gives

$$
|z|^{-2v}|1-z|^{-2w}=\frac1{\Gamma(v)\Gamma(w)}\int_0^\infty d\lambda\,d\rho\,\lambda^{v-1}\rho^{w-1}e^{-\lambda|z|^2-\rho|z-1|^2}.
$$

Completing the square, the $dx\,dy$ [Gaussian integral](../../../calculus.md#gaussian-integral) is $\pi(\lambda+\rho)^{-1}\exp[-\lambda\rho/(\lambda+\rho)]$. Change variables to $q=\lambda+\rho$ and $x=\lambda/q$; their [Jacobian determinant](../../../calculus.md#jacobian-determinant) is $q$. Integrating $q$ gives $\Gamma(v+w-1)[x(1-x)]^{-(v+w-1)}$. The remaining integral is the ordinary [beta function](../../../complex-analysis.md#beta-function) $B(1-w,1-v)=B(b,a)$. Thus

$$
\int_{\mathbb C}dx\,dy\,|z|^{2a-2}|1-z|^{2b-2}
=\pi\frac{\Gamma(a)\Gamma(b)\Gamma(c)}{\Gamma(1-a)\Gamma(1-b)\Gamma(1-c)}.
$$

Restoring $d^2z=2dx\,dy$ and substituting the [Mandelstam variables](../../../special-relativity.md#mandelstam-variables) proves the [Virasoro–Shapiro amplitude](../../../string-theory.md#virasoro-shapiro-amplitude):

$$
\boxed{A^{(4)}=2\pi g_s^2\frac{\Gamma(-1-\alpha's/4)\Gamma(-1-\alpha't/4)\Gamma(-1-\alpha'u/4)}{\Gamma(2+\alpha's/4)\Gamma(2+\alpha't/4)\Gamma(2+\alpha'u/4)}.}
$$

For physical scattering the original position integral generally fails to converge. The formula defines the amplitude by [analytic continuation](../../../complex-analysis.md#analytic-continuation) from the convergence domain, with the desired scattering boundary value at real poles; the convergent integral should not be claimed valid for every physical [momentum](../../../classical-mechanics.md#momentum).

The [gamma function](../../../complex-analysis.md#gamma-function) is a [meromorphic function](../../../isolated-singularity.md#meromorphic-function), with [simple poles](../../../isolated-singularity.md#simple-pole) at nonpositive integers and no zeros, while its reciprocal $1/\Gamma$ is an [entire function](../../../complex-analysis.md#entire-function). Consequently it is a [meromorphic function](../../../isolated-singularity.md#meromorphic-function) of the independent invariants and a [crossing-symmetric scattering amplitude](../../../quantum-mechanics.md#crossing-symmetry): permuting $s,t,u$ leaves it unchanged. Its generic channel poles are

$$
\boxed{s=\frac4{\alpha'}(n-1),\quad n=0,1,2,\ldots,}
$$

and the same tower in $t$ and $u$. They represent the exchanged [bosonic string mass spectrum](../../../string-theory.md#bosonic-string-mass-spectrum): the tachyon, massless states including the graviton, and an infinite sequence of massive closed-string levels. There are no threshold [branch cuts](../../../analysis.md#branch-cut) at this tree order.

A precise check of factorization is the [Virasoro–Shapiro amplitude pole residue](../../../string-theory.md#virasoro-shapiro-amplitude-pole-residue). Near $a=-n$, set $c=1+n-b$ in the nonsingular factor. The [gamma function](../../../complex-analysis.md#gamma-function) recurrence gives

$$
\frac{\Gamma(b)\Gamma(1+n-b)}{\Gamma(1-b)\Gamma(b-n)}=(-1)^n\prod_{j=1}^n(b-j)^2.
$$

Combining this with $\Gamma(a)\sim(-1)^n/[n!(a+n)]$ shows

$$
\operatorname*{Res}_{s=4(n-1)/\alpha'}A^{(4)}=-\frac{8\pi g_s^2}{\alpha'(n!)^2}\prod_{j=1}^n(b-j)^2.
$$

The [residue](../../../analysis.md#residue) is a degree-$2n$ polynomial in $t$, consistent with exchange up to spin $2n$ and [scattering-amplitude factorization](../../../quantum-mechanics.md#scattering-amplitude-factorization). At exceptional kinematics reciprocal Gamma zeros can remove apparent poles. In particular, when both $a$ and $b$ approach nonpositive integers, the zero from $1/\Gamma(a+b)$ cancels the putative double pole, leaving channel simple-pole terms. Thus one must not count products of numerator poles without using $a+b+c=1$.

## 4

↑ **Parent:** [Paper 306](paper-306.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

A [Majorana spinor](../../../relativistic-quantum-field.md#majorana-spinor) equals its [charge conjugation](../../../quantum-field-theory.md#charge-conjugation), $\psi^c=C\bar\psi^{\,T}=\psi$, with conventional phase choices absorbed into $C$. The two-component [worldsheet Majorana fermion](../../../string-theory.md#worldsheet-majorana-fermion) therefore has no independent complex conjugate components; in a Majorana representation its components can be real [Grassmann variables](../../../linear-algebra.md#grassmann-variable). The same condition applies to the constant supersymmetry parameter. Grassmann statistics matter in the variation: replacing the spinors by commuting numerical vectors would give the wrong bilinear interchange signs.

The displayed rigid transformation is understood in flat [conformal gauge](../../../string-theory.md#conformal-gauge). Take $h_{\mu\nu}=\eta_{\mu\nu}=\operatorname{diag}(-1,1)$, $\{\gamma^\mu,\gamma^\nu\}=2\eta^{\mu\nu}$, and choose

$$
\gamma^0=\begin{pmatrix}0&-1\\1&0\end{pmatrix},\qquad
\gamma^1=\begin{pmatrix}0&1\\1&0\end{pmatrix},\qquad\bar\psi=\psi^T\gamma^0.
$$

Here $C=\gamma^0$ is a valid invariant charge-conjugation form: $C^T=-C$ and $(\gamma^\mu)^TC=-C\gamma^\mu$. These concrete matrices make all signs checkable; equivalent Majorana conventions give the same result with their consistently transformed bars.

Let $A=\sqrt{\alpha'/2}$ and $B=1/\sqrt{2\alpha'}$, so $\alpha'B=A$. Suppressing the common factor $-1/(4\pi\alpha')$ in the action, the flat kinetic density is

$$
\mathcal L_0=\partial_\mu X^a\partial^\mu X_a+i\alpha'\bar\psi^a\gamma^\mu\partial_\mu\psi_a.
$$

The rigid variations have $\delta X^a=iA\bar\epsilon\psi^a$ and $\delta\psi^a=B\gamma^\nu\partial_\nu X^a\epsilon$. The supersymmetry variation is even, so its product rule has no extra graded sign. From the [Majorana Grassmann bilinear interchange](../../../relativistic-quantum-field.md#majorana-grassmann-bilinear-interchange) identities,

$$
\delta\bar\psi^a=-B\bar\epsilon\gamma^\nu\partial_\nu X^a,\qquad
\bar\psi^a\epsilon=\bar\epsilon\psi^a,\qquad
\bar\psi^a\gamma^\mu\gamma^\nu\epsilon=\bar\epsilon\gamma^\nu\gamma^\mu\psi^a.
$$

For example the last identity follows by moving the Grassmann-odd parameter through $\psi$, then using $C^T=-C$ and the transpose relations twice. No equation of motion has been used.

The two kinetic variations are

$$
\delta\mathcal L_B=2iA\partial^\mu X_a\bar\epsilon\partial_\mu\psi^a,
$$



$$
\delta\mathcal L_F=-iA\partial_\nu X_a\bar\epsilon\gamma^\nu\gamma^\mu\partial_\mu\psi^a+iA\bar\psi_a\gamma^\mu\gamma^\nu\epsilon\,\partial_\mu\partial_\nu X^a.
$$

The [Clifford algebra](../../../algebra.md#clifford-algebra) turns the first fermionic term plus the bosonic variation into $iA\partial_\nu X_a\bar\epsilon\gamma^\mu\gamma^\nu\partial_\mu\psi^a$. In the second term, commute the [partial derivatives](../../../calculus.md#partial-derivative) and use the same algebra: the antisymmetric gamma product drops out, leaving $iA\Box X_a\bar\epsilon\psi^a$. Together they are precisely the [rigid worldsheet supersymmetry boundary term](../../../string-theory.md#rigid-worldsheet-supersymmetry-boundary-term):

$$
\boxed{\delta\mathcal L_0=\partial_\mu J^\mu,\qquad J^\mu=i\sqrt{\frac{\alpha'}2}\,\partial_\nu X_a\bar\epsilon\gamma^\mu\gamma^\nu\psi^a.}
$$

Therefore $\delta S=-(4\pi\alpha')^{-1}\int_{\partial\Sigma}d\Sigma_\mu\,J^\mu$. It vanishes on a closed or periodic worldsheet, for compactly supported changes, or under compatible supersymmetric endpoint conditions. The local total-derivative identity is off shell; the boundary assumptions are needed to call the integrated action invariant.

The flat-gauge qualification is substantive. On an arbitrary curved worldsheet, spinors need a [zweibein](../../../general-relativity.md#zweibein) and [spin connection](../../../connection-1-form.md#spin-connection) and a constant spinor parameter need not exist. A fully covariant locally supersymmetric action also involves the [worldsheet gravitino](../../../string-theory.md#worldsheet-gravitino); the isolated ordinary-derivative expression does not prove rigid invariance for arbitrary $h_{\mu\nu}$. We have proved the intended rigid symmetry of its flat gauge-fixed action, with the fermionic term inside the same integral and overall normalization. If the displayed last term were read as outside the integral, it would not even define an action.

For phenomenology, [bosonic string theory](../../../string-theory.md#bosonic-string-theory) has no spacetime [fermions](../../../quantum-mechanics.md#fermion) and its usual vacuum contains a [tachyon](../../../physics.md#tachyon). The [spinning string](../../../string-theory.md#spinning-string) has a [Ramond sector](../../../string-theory.md#ramond-sector), whose fermionic zero modes form a spacetime [Clifford algebra](../../../algebra.md#clifford-algebra) and give spacetime spinor states, as well as a [Neveu–Schwarz sector](../../../string-theory.md#neveu-schwarz-sector). In suitable consistent theories the [GSO projection](../../../string-theory.md#gso-projection) removes the tachyonic NS ground state and keeps the appropriate Ramond chirality. The [critical dimension of the RNS superstring](../../../string-theory.md#critical-dimension-of-the-rns-superstring) is 10 rather than 26: $D$ [bosons](../../../quantum-mechanics.md#boson) and $D$ real [fermions](../../../quantum-mechanics.md#fermion) have matter [central charge](../../../string-theory.md#central-charge) $3D/2$ per chiral sector, while the reparameterization and superconformal ghosts contribute $-26+11=-15$, so the total anomaly cancels at $D=10$.

**Suitable GSO-projected superstrings admit spacetime [fermions](../../../quantum-mechanics.md#fermion) and a tachyon-free spectrum, making them more promising for particle physics than the bosonic string.** Rigid [worldsheet supersymmetry](../../../string-theory.md#worldsheet-supersymmetry) alone does not establish a tachyon-free spacetime theory or realistic phenomenology. The projection, consistent sectors and [compactification in string theory](../../../string-theory.md#compactification-in-string-theory) are additional input; spacetime supersymmetry and a realistic four-dimensional spectrum are not automatic consequences of this classical action.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2017](../../2017.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
