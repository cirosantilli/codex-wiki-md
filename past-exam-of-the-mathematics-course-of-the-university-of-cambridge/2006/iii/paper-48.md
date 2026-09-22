# Paper 48

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2006/Paper48.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2006/Paper48.pdf)

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

↑ **Parent:** [Paper 48](paper-48.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Use [Minkowski spacetime](../../../special-relativity.md#minkowski-spacetime) with $g_{\mu\nu}=\operatorname{diag}(1,-1,-1,-1)$ and units $\hbar=c=1$. The transformation rotates the two components in their internal plane. In particular,

$$
\delta(\phi_1^2+\phi_2^2)=2\alpha(\phi_1\phi_2-\phi_2\phi_1)=0,
\qquad
\delta\bigl(\partial_\mu\phi_1\partial^\mu\phi_1+\partial_\mu\phi_2\partial^\mu\phi_2\bigr)=0.
$$

Thus both terms in the [Lagrangian density](../../../quantum-field-theory.md#lagrangian-density) are invariant: this is an [internal rotation symmetry of two real scalar fields](../../../scalar-field-theory.md#internal-rotation-symmetry-of-two-real-scalar-fields), rather than a transformation of spacetime. The equal masses are essential to this symmetry.

The [Noether theorem](../../../calculus-of-variations.md#noether-theorem) gives the [Noether current](../../../quantum-field-theory.md#noether-current)

$$
j^\mu=\sum_{k=1}^2\frac{\partial\mathcal L}{\partial(\partial_\mu\phi_k)}\frac{\delta\phi_k}{\alpha}
=\phi_2\partial^\mu\phi_1-\phi_1\partial^\mu\phi_2.
$$

Indeed, the cross terms in its divergence cancel, and the two [Klein-Gordon equations](../../../wave-equation.md#klein-gordon-equation) imply

$$
\partial_\mu j^\mu=\phi_2\Box\phi_1-\phi_1\Box\phi_2
=-m^2\phi_2\phi_1+m^2\phi_1\phi_2=0.
$$

For fields decaying sufficiently at spatial infinity, there is no outward current flux. The conserved [Noether charge](../../../quantum-field-theory.md#noether-charge) is therefore

$$
\boxed{Q=\int d^3x\,(\phi_2\dot\phi_1-\phi_1\dot\phi_2).}
$$

In [canonical quantization](../../../quantum-mechanics.md#canonical-quantization), the [canonical momenta](../../../classical-mechanics.md#canonical-momentum) are $\pi_k=\dot\phi_k$, with equal-time [canonical commutation relations](../../../quantum-mechanics.md#canonical-commutation-relation)

$$
[\phi_k(\mathbf x),\pi_l(\mathbf y)]=i\delta_{kl}\delta^3(\mathbf x-\mathbf y),
\qquad [\phi_k,\phi_l]=[\pi_k,\pi_l]=0.
$$

Consequently $Q=\int d^3x\,(\pi_1\phi_2-\pi_2\phi_1)$. Operators of different components commute, so this expression is [Hermitian](../../../hilbert-space.md#hermitian-operator) without an ordering correction. Write $\int_{\mathbf p}=\int d^3p/(2\pi)^3$, $E_{\mathbf p}=\sqrt{\mathbf p^2+m^2}$ and $a_{k\mathbf p}=a^k_{\mathbf p}$. Substituting the oscillator expansions and using the [Dirac delta function](../../../distribution-theory.md#dirac-delta-function) from the spatial integral gives

$$
Q=-\frac i2\int_{\mathbf p}\left[
(a_{1\mathbf p}-a_{1,-\mathbf p}^{\dagger})(a_{2,-\mathbf p}+a_{2\mathbf p}^{\dagger})
-(a_{2\mathbf p}-a_{2,-\mathbf p}^{\dagger})(a_{1,-\mathbf p}+a_{1\mathbf p}^{\dagger})
\right].
$$

The terms with two [annihilation operators](../../../quantum-mechanics.md#annihilation-operator) cancel after $\mathbf p\mapsto-\mathbf p$; the terms with two [creation operators](../../../quantum-mechanics.md#creation-operator) cancel in the same way. In the remaining terms use

$$
[a_{k\mathbf p},a_{l\mathbf q}^{\dagger}]=(2\pi)^3\delta_{kl}\delta^3(\mathbf p-\mathbf q).
$$

There is no [commutator](../../../lie-algebra.md#commutator) constant between the distinct components. The result is already in [normal ordering](../../../perturbative-quantum-field-theory.md#normal-ordering):

$$
\boxed{Q=-i\int_{\mathbf p}\bigl(a_{2\mathbf p}^{\dagger}a_{1\mathbf p}-a_{1\mathbf p}^{\dagger}a_{2\mathbf p}\bigr).}
$$

For the [charged oscillator basis of a scalar doublet](../../../scalar-field-theory.md#charged-oscillator-basis-of-a-scalar-doublet), compute

$$
[Q,a_{1\mathbf p}^{\dagger}]=-ia_{2\mathbf p}^{\dagger},\qquad
[Q,a_{2\mathbf p}^{\dagger}]=ia_{1\mathbf p}^{\dagger},\qquad
b_{\pm\mathbf p}^{\dagger}=\frac{a_{1\mathbf p}^{\dagger}\mp ia_{2\mathbf p}^{\dagger}}{\sqrt2}.
$$

It follows that $[Q,b_{\pm\mathbf p}^{\dagger}]=\pm b_{\pm\mathbf p}^{\dagger}$. The [Fock vacuum](../../../quantum-field-theory.md#fock-vacuum) satisfies $Q|0\rangle=0$, so **$b_{+\mathbf p}^{\dagger}|0\rangle$ has charge $+1$, and $b_{-\mathbf p}^{\dagger}|0\rangle$ has charge $-1$**. To obtain a normalized [one-particle state](../../../quantum-field-theory.md#one-particle-state), replace the sharp momentum by $\int_{\mathbf p}f(\mathbf p)b_{\pm\mathbf p}^{\dagger}|0\rangle$, where $\int_{\mathbf p}|f(\mathbf p)|^2=1$. The charge is unchanged. Equivalently,

$$
Q=\int_{\mathbf p}(b_{+\mathbf p}^{\dagger}b_{+\mathbf p}-b_{-\mathbf p}^{\dagger}b_{-\mathbf p}).
$$

The generator convention is $\delta\phi_k=i\alpha[Q,\phi_k]$, which reproduces the original rotation signs.

For [stability of a two-scalar quartic potential](../../../scalar-field-theory.md#stability-of-a-two-scalar-quartic-potential), the relevant [potential energy](../../../classical-mechanics.md#potential-energy) density is

$$
V=\frac{m^2}{2}(\phi_1^2+\phi_2^2)+V_4,\qquad
V_4=\lambda(\phi_1^2-\phi_2^2)^2+2(\lambda+\mu)\phi_1^2\phi_2^2.
$$

Along either axis boundedness requires $\lambda\ge0$; along $\phi_1=\phi_2$ it requires $\lambda+\mu\ge0$. Conversely the displayed sum is nonnegative whenever both conditions hold. With $m^2>0$ the origin is then the unique global minimum, including the equality cases. Hence the stable-vacuum conditions are

$$
\boxed{\lambda\ge0,\qquad\mu\ge-\lambda.}
$$

Strict positivity of the quartic term away from the origin would instead require $\lambda>0$ and $\mu>-\lambda$. That stronger condition is unnecessary for a positive mass term. If $m=0$, the same non-strict conditions give boundedness, but the equality cases have flat directions and do not give an isolated [classical vacuum](../../../quantum-field-theory.md#classical-vacuum).

Finally, the interaction changes the variation of the [potential energy](../../../classical-mechanics.md#potential-energy) by

$$
\delta V_4=4\alpha(\lambda-\mu)\phi_1\phi_2(\phi_1^2-\phi_2^2).
$$

The interacting [Euler-Lagrange equations](../../../analysis.md#euler-lagrange-equation) consequently give

$$
\partial_\mu j^\mu=-4(\lambda-\mu)\phi_1\phi_2(\phi_1^2-\phi_2^2).
$$

Thus the same [Noether charge](../../../quantum-field-theory.md#noether-charge) is conserved for all field configurations precisely when **$\mu=\lambda$**. Then $V_4=\lambda(\phi_1^2+\phi_2^2)^2$ preserves the [internal rotation symmetry of two real scalar fields](../../../scalar-field-theory.md#internal-rotation-symmetry-of-two-real-scalar-fields); imposing stability additionally requires $\lambda\ge0$.

## 2

↑ **Parent:** [Paper 48](paper-48.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

Fix the [phi-fourth theory](../../../scalar-field-theory.md#quartic-interaction) convention $\mathcal L_{\mathrm{int}}=-\lambda\phi^4/4!$, with mostly-minus [Minkowski spacetime](../../../special-relativity.md#minkowski-spacetime) and $\hbar=c=1$. Define the [scattering amplitude](../../../quantum-mechanics.md#scattering-amplitude) by stripping the overall momentum-conserving delta function from $S-1=i\mathcal M$. If instead the coupling is defined by $\mathcal L_{\mathrm{int}}=-\lambda\phi^4$, every vertex coupling below must be replaced by $24\lambda$; the question does not specify this factorial convention.

The momentum-space [Feynman rules](../../../perturbative-quantum-field-theory.md#feynman-rule) are a [Feynman propagator](../../../quantum-field-theory.md#feynman-propagator) $i/(k^2-m^2+i0)$ for each internal scalar line, a [Feynman vertex](../../../perturbative-quantum-field-theory.md#interaction-vertex) $-i\lambda$ with four scalar legs, and [four-momentum conservation](../../../special-relativity.md#four-momentum-conservation) at each vertex. Integrate each independent [loop momentum](../../../perturbative-quantum-field-theory.md#loop-momentum) with $d^4\ell/(2\pi)^4$ and divide by the [Feynman-diagram symmetry factor](../../../perturbative-quantum-field-theory.md#feynman-diagram-symmetry-factor). For an amputated [scattering amplitude](../../../quantum-mechanics.md#scattering-amplitude) there are no external propagators; external states have the usual relativistic normalization. Sum the connected diagrams and all inequivalent assignments of the labelled external momenta. The overall delta function is $(2\pi)^4\delta^4(\sum p_{\mathrm{in}}-\sum p_{\mathrm{out}})$.

These [Feynman rules](../../../perturbative-quantum-field-theory.md#feynman-rule) follow by expanding the [Dyson series](../../../perturbative-quantum-field-theory.md#dyson-series) $T\exp(i\int d^4x\,\mathcal L_{\mathrm{int}})$ and applying the [Wick theorem](../../../perturbative-quantum-field-theory.md#wick-s-theorem) to the free-field correlation functions. A [Wick contraction](../../../perturbative-quantum-field-theory.md#wick-contraction) gives the free [Feynman propagator](../../../quantum-field-theory.md#feynman-propagator); the $4!$ ways of contracting a vertex cancel its factorial denominator. The expansion's $1/V!$ cancels permutations of identical interaction insertions, while any remaining automorphisms give the [Feynman-diagram symmetry factor](../../../perturbative-quantum-field-theory.md#feynman-diagram-symmetry-factor). [Fourier transformation](../../../analysis.md#fourier-transform) produces momentum conservation, and the [LSZ reduction formula](../../../perturbative-quantum-field-theory.md#lsz-reduction-formula) amputates external propagators to obtain the [scattering amplitude](../../../quantum-mechanics.md#scattering-amplitude).

For [six-point amplitudes in phi-fourth theory](../../../scalar-field-theory.md#six-point-amplitudes-in-phi-fourth-theory), an original pair of diagrams is:

<a id="2/image-tree-and-one-loop-triangle-contributions-to-two-to-four-scalar-scattering"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-48-scattering-diagrams.png)

**[Figure 1](#2/image-tree-and-one-loop-triangle-contributions-to-two-to-four-scalar-scattering). Tree and one-loop triangle contributions to two-to-four scalar scattering**.

In the [tree-level Feynman diagram](../../../perturbative-quantum-field-theory.md#tree-level-feynman-diagram), let the internal [four-momentum](../../../special-relativity.md#four-momentum) be $r=p_1+p_2-q_1=q_2+q_3+q_4$. The labelled diagram has [symmetry factor](../../../perturbative-quantum-field-theory.md#feynman-diagram-symmetry-factor) one, so its contribution is

$$
i\mathcal M_{\mathrm{tree}}=(-i\lambda)^2\frac{i}{r^2-m^2+i0},\qquad
\boxed{\mathcal M_{\mathrm{tree}}=-\frac{\lambda^2}{r^2-m^2+i0}.}
$$

This is one channel. The full tree [scattering amplitude](../../../quantum-mechanics.md#scattering-amplitude) sums the ten unordered partitions of the six labelled external legs into two groups of three, since $\binom63/2=10$.

For the one-loop [triangle Feynman diagram](../../../perturbative-quantum-field-theory.md#triangle-feynman-diagram), set $P=p_1+p_2$, $Q_{12}=q_1+q_2$, $Q_{34}=q_3+q_4$, so $P=Q_{12}+Q_{34}$. A consistent routing has denominators

$$
D_0=\ell^2-m^2+i0,\qquad D_1=(\ell-P)^2-m^2+i0,\qquad D_2=(\ell-Q_{34})^2-m^2+i0.
$$

With the external labels held fixed, no nontrivial graph automorphism remains, so again the [symmetry factor](../../../perturbative-quantum-field-theory.md#feynman-diagram-symmetry-factor) is one. The contribution is

$$
\boxed{i\mathcal M_{\triangle}=(-i\lambda)^3\int\frac{d^4\ell}{(2\pi)^4}\frac{i^3}{D_0D_1D_2}
=\lambda^3\int\frac{d^4\ell}{(2\pi)^4}\frac1{D_0D_1D_2}.}
$$

There are other labelled assignments and other one-loop topologies in the full [scattering amplitude](../../../quantum-mechanics.md#scattering-amplitude); the displayed expression belongs to the particular drawn diagram.

One can also express this [scalar triangle Feynman integral](../../../perturbative-quantum-field-theory.md#scalar-triangle-feynman-integral) using [Feynman parameters](../../../perturbative-quantum-field-theory.md#feynman-parameter). With $x+y+z=1$, completing the square in $xD_0+yD_1+zD_2$ gives

$$
\Delta=m^2-xyP^2-xzQ_{34}^2-yzQ_{12}^2.
$$

The identity $1/(D_0D_1D_2)=2\int_{x,y,z\ge0}dx\,dy\,dz\,\delta(1-x-y-z)/(xD_0+yD_1+zD_2)^3$ and the shifted momentum integral yield

$$
\int\frac{d^4\ell}{(2\pi)^4}\frac1{D_0D_1D_2}
=-\frac{i}{16\pi^2}\int_{x,y,z\ge0}\frac{dx\,dy\,dz\,\delta(1-x-y-z)}{\Delta-i0}.
$$

Thus $\mathcal M_{\triangle}=-\lambda^3/(16\pi^2)$ times the displayed parameter integral. It is ultraviolet finite in four dimensions, although physical threshold singularities must retain the [Feynman i-epsilon prescription](../../../quantum-field-theory.md#feynman-i-epsilon-prescription).

For the [fixed-target production threshold](../../../special-relativity.md#fixed-target-production-threshold), the incoming [four-momenta](../../../special-relativity.md#four-momentum) are $(E,\mathbf p)$ and $(m,\mathbf0)$, with $E=\sqrt{m^2+|\mathbf p|^2}$. Their [invariant mass](../../../special-relativity.md#invariant-mass) obeys

$$
s=(p_1+p_2)^2=2m^2+2mE.
$$

In the centre-of-momentum frame, four final particles have total energy at least $4m$, attained when all four are at rest in that frame. Therefore $s\ge16m^2$, equivalently $E\ge7m$, and

$$
\boxed{|\mathbf p|\ge4\sqrt3\,m.}
$$

This is the kinematic threshold for $m>0$. Exactly at equality the final [phase space](../../../classical-mechanics.md#phase-space) has zero volume; a nonzero production rate requires a strict inequality.

## 3

↑ **Parent:** [Paper 48](paper-48.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

Let the masses of $\Phi$ and $\phi$ be $M$ and $\mu$, respectively. Write their external [four-momenta](../../../special-relativity.md#four-momentum) as $P=k_1+k_2$, with $P^2=M^2$ and $k_1^2=k_2^2=\mu^2$. The condition $M>2\mu$ opens the two-body decay [phase space](../../../classical-mechanics.md#phase-space). Use mostly-minus [Minkowski spacetime](../../../special-relativity.md#minkowski-spacetime), the [Dirac propagator](../../../quantum-field-theory.md#dirac-propagator) $i(\not k+m)/(k^2-m^2+i0)$, and the convention that an amputated connected diagram contributes $i\mathcal M$.

There is no tree-level three-scalar [Feynman vertex](../../../perturbative-quantum-field-theory.md#interaction-vertex) in the displayed interaction. The leading [decay amplitude](../../../relativistic-quantum-field.md#decay-amplitude) has one $\Phi$ [Yukawa interaction](../../../standard-model.md#yukawa-interaction) and two $\phi$ [Yukawa interactions](../../../standard-model.md#yukawa-interaction), so is of order $Gg^2$. The [Yukawa fermion triangle](../../../perturbative-quantum-field-theory.md#yukawa-fermion-triangle) is:

<a id="3/image-fermion-triangle-for-scalar-decay-with-its-loop-momentum-routing-and-yukawa-vertex-factors"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-48-fermion-triangle.png)

**[Figure 2](#3/image-fermion-triangle-for-scalar-decay-with-its-loop-momentum-routing-and-yukawa-vertex-factors). Fermion triangle for scalar decay with its loop-momentum routing and Yukawa vertex factors**.

The two inequivalent cyclic orderings around the [fermion loop](../../../perturbative-quantum-field-theory.md#fermion-loop) are related by reversal and interchange of $k_1,k_2$. They give equal integrals: reversing all internal [four-momenta](../../../special-relativity.md#four-momentum) leaves the masses and denominators unchanged, and the scalar [gamma matrix trace identities](../../../algebra.md#gamma-matrix-trace-identities) below give the same numerator. Both must be included. The [closed fermion loop sign](../../../perturbative-quantum-field-theory.md#closed-fermion-loop-sign) supplies $-1$, and each ordering has the product

$$
(-1)(-iG)(-ig)^2i^3=-Gg^2.
$$

There is no extra $1/2!$ in the [decay amplitude](../../../relativistic-quantum-field.md#decay-amplitude). Such a factor belongs to integration over the identical-particle final [phase space](../../../classical-mechanics.md#phase-space) when calculating a decay rate.

Route $a=\ell$, $b=\ell+k_1$, $c=\ell-k_2$ and define $D_a=a^2-m^2+i0$, and similarly for $D_b,D_c$. A regulated leading [decay amplitude](../../../relativistic-quantum-field.md#decay-amplitude) is

$$
\boxed{i\mathcal M_{\mathrm{loop}}=-2Gg^2\mu_R^{2\epsilon}
\int\frac{d^{4-2\epsilon}\ell}{(2\pi)^{4-2\epsilon}}
\frac{\operatorname{tr}[(\not a+m)(\not b+m)(\not c+m)]}{D_aD_bD_c}.}
$$

Here [dimensional regularization](../../../perturbative-quantum-field-theory.md#dimensional-regularization) preserves translation of the [loop momentum](../../../perturbative-quantum-field-theory.md#loop-momentum), and $\mu_R$ is its reference mass scale. Factors $\mu_R^{2\epsilon}$ account for the loop's dimension; dimensionally continued couplings can equivalently carry these powers. No $\gamma^5$ occurs in this scalar loop, so there is no $\gamma^5$ regularization ambiguity.

Using [gamma matrix trace identities](../../../algebra.md#gamma-matrix-trace-identities), traces with an odd number of [gamma matrices](../../../algebra.md#gamma-matrices) vanish, while $\operatorname{tr}1=4$ and $\operatorname{tr}(\gamma^\mu\gamma^\nu)=4g^{\mu\nu}$. Thus the numerator simplifies completely to

$$
\begin{aligned}
N&=4m\bigl[m^2+a\cdot b+a\cdot c+b\cdot c\bigr]\\
&=4m\bigl[m^2+3\ell^2+2\ell\cdot(k_1-k_2)-k_1\cdot k_2\bigr],
\qquad k_1\cdot k_2=\frac{M^2-2\mu^2}{2}.
\end{aligned}
$$

For a reduction to standard scalar integrals, disregard the vanishing infinitesimals only in the numerator. Since $D_a+D_b+D_c=3\ell^2+2\ell\cdot(k_1-k_2)+2\mu^2-3m^2$ up to those infinitesimals,

$$
N=4m\left[D_a+D_b+D_c+4m^2-\mu^2-\frac{M^2}{2}\right].
$$

Define the scalar bubble and [scalar triangle Feynman integral](../../../perturbative-quantum-field-theory.md#scalar-triangle-feynman-integral) by

$$
B(s)=\mu_R^{2\epsilon}\int\frac{d^{4-2\epsilon}\ell}{(2\pi)^{4-2\epsilon}}
\frac1{(\ell^2-m^2+i0)((\ell+q)^2-m^2+i0)},\quad q^2=s,
\qquad
C=\mu_R^{2\epsilon}\int\frac{d^{4-2\epsilon}\ell}{(2\pi)^{4-2\epsilon}}\frac1{D_aD_bD_c}.
$$

Cancelling each denominator in turn gives two bubbles with external invariant $\mu^2$ and one with invariant $M^2$. Therefore

$$
\boxed{i\mathcal M_{\mathrm{loop}}=-8mGg^2\left[2B(\mu^2)+B(M^2)+\left(4m^2-\mu^2-\frac{M^2}{2}\right)C\right].}
$$

This explicitly displays the complete [gamma matrix](../../../algebra.md#gamma-matrices) trace simplification, the two loop orientations and the overall phase convention.

There is a [renormalization](../../../perturbative-quantum-field-theory.md#renormalization) qualification to this answer. For $m\ne0$ the loop is logarithmically divergent; retaining just the unregulated four-dimensional integral would not specify a finite physical [decay amplitude](../../../relativistic-quantum-field.md#decay-amplitude). To see the divergence, a [Feynman parameter](../../../perturbative-quantum-field-theory.md#feynman-parameter) and a shifted [loop momentum](../../../perturbative-quantum-field-theory.md#loop-momentum) give

$$
B(s)=\frac{i}{16\pi^2}\left[\frac1{\bar\epsilon}-\int_0^1dx\,\log\frac{m^2-x(1-x)s-i0}{\mu_R^2}\right]+O(\epsilon),
\qquad \frac1{\bar\epsilon}=\frac1\epsilon-\gamma_E+\log(4\pi).
$$

The [scalar triangle Feynman integral](../../../perturbative-quantum-field-theory.md#scalar-triangle-feynman-integral) is ultraviolet finite. Hence

$$
\mathcal M_{\mathrm{loop,div}}=-\frac{24mGg^2}{16\pi^2\bar\epsilon}.
$$

A [cubic counterterm from a Yukawa fermion triangle](../../../perturbative-quantum-field-theory.md#cubic-counterterm-from-a-yukawa-fermion-triangle), $\mathcal L_{\mathrm{ct}}=-\delta h\,\Phi\phi^2/2$, contributes $-\delta h$ to $\mathcal M$ and cancels the pole with $\delta h_{\mathrm{div}}=-24mGg^2/(16\pi^2\bar\epsilon)$. This is an instance of [counterterm closure of a massive Yukawa theory](../../../perturbative-quantum-field-theory.md#counterterm-closure-of-a-massive-yukawa-theory). After subtraction the physical answer is $\mathcal M=-h_R+\mathcal M_{\mathrm{loop,ren}}$, where a [renormalization condition](../../../perturbative-quantum-field-theory.md#renormalization-condition) fixes the finite cubic coupling $h_R$. The displayed interaction alone does not supply that condition. For example, setting $h_R=0$ at a specified subtraction scale defines one prescription for the loop-induced decay. The regulated expressions above remain the lowest-order loop answer without such extra data. For $m=0$ the trace, and therefore this scalar triangle contribution, vanishes identically.

Now take the [Hermitian](../../../hilbert-space.md#hermitian-operator) [pseudoscalar Yukawa interaction](../../../standard-model.md#pseudoscalar-yukawa-interaction) with the sign printed in the PDF. Varying with respect to the [Dirac adjoint](../../../relativistic-quantum-field.md#dirac-adjoint) gives the [Dirac equation](../../../relativistic-quantum-field.md#dirac-equation)

$$
\boxed{(i\gamma^\mu\partial_\mu-m-g\phi+iG\Phi\gamma^5)\psi=0.}
$$

Varying with respect to $\psi$ and integrating by parts gives the [adjoint Dirac equation](../../../relativistic-quantum-field.md#adjoint-dirac-equation)

$$
i(\partial_\mu\bar\psi)\gamma^\mu+(m+g\phi)\bar\psi-iG\Phi\bar\psi\gamma^5=0.
$$

The factor $i$ in the coupling matters: $\bar\psi\gamma^5\psi$ is anti-Hermitian, so this factor makes the interaction [Hermitian](../../../hilbert-space.md#hermitian-operator) for real $G$.

For the [axial-current divergence for scalar and pseudoscalar backgrounds](../../../relativistic-quantum-field.md#axial-current-divergence-for-scalar-and-pseudoscalar-backgrounds), set $S=m+g\phi$ and $H=G\Phi$. The two equations are equivalently

$$
\gamma^\mu\partial_\mu\psi=-iS\psi-H\gamma^5\psi,\qquad
(\partial_\mu\bar\psi)\gamma^\mu=iS\bar\psi+H\bar\psi\gamma^5.
$$

In the divergence of the [axial current](../../../relativistic-quantum-field.md#axial-current), use $\{\gamma^5,\gamma^\mu\}=0$ and $(\gamma^5)^2=1$:

$$
\begin{aligned}
\partial_\mu(\bar\psi\gamma^\mu\gamma^5\psi)
&=(\partial_\mu\bar\psi)\gamma^\mu\gamma^5\psi
-\bar\psi\gamma^5\gamma^\mu\partial_\mu\psi\\
&=(iS\bar\psi+H\bar\psi\gamma^5)\gamma^5\psi
-\bar\psi\gamma^5(-iS\psi-H\gamma^5\psi).
\end{aligned}
$$

Thus

$$
\boxed{\partial_\mu j_5^\mu=2i(m+g\phi)\bar\psi\gamma^5\psi+2G\Phi\bar\psi\psi.}
$$

This is the classical field-equation identity requested here. It includes explicit breaking by both backgrounds; it is not a claim that a renormalized quantum [axial current](../../../relativistic-quantum-field.md#axial-current) has no [chiral anomaly](../../../relativistic-quantum-field.md#chiral-anomaly) when gauge interactions are present.

## 4

↑ **Parent:** [Paper 48](paper-48.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

In [quantum electrodynamics](../../../perturbative-quantum-field-theory.md#quantum-electrodynamics), [gauge invariance](../../../relativistic-quantum-field.md#gauge-invariance) connects local phase freedom, electric-charge conservation and the restrictions on [photon](../../../quantum-mechanics.md#photon) interactions. For definiteness take

$$
\mathcal L=-\frac14F_{\mu\nu}F^{\mu\nu}+\bar\psi(i\gamma^\mu D_\mu-m)\psi,\qquad
D_\mu=\partial_\mu+ieA_\mu,\qquad
F_{\mu\nu}=\partial_\mu A_\nu-\partial_\nu A_\mu.
$$

The [gauge transformation](../../../electromagnetism.md#gauge-transformation)

$$
\psi\mapsto e^{-ie\alpha(x)}\psi,\qquad
\bar\psi\mapsto\bar\psi e^{ie\alpha(x)},\qquad
A_\mu\mapsto A_\mu+\partial_\mu\alpha
$$

has $D_\mu\psi\mapsto e^{-ie\alpha}D_\mu\psi$: the derivative of the local phase cancels the added [gauge potential](../../../relativistic-quantum-field.md#gauge-field). Also $F_{\mu\nu}$ is unchanged because mixed partial derivatives commute. Consequently every term in the [Lagrangian density](../../../quantum-field-theory.md#lagrangian-density) is invariant. This derives the [minimal electromagnetic coupling of a Dirac field](../../../perturbative-quantum-field-theory.md#minimal-electromagnetic-coupling-of-a-dirac-field), including the interaction $-e\bar\psi\gamma^\mu\psi A_\mu$. A [fermion](../../../quantum-mechanics.md#fermion) mass is compatible with the symmetry, whereas a local Proca [photon](../../../quantum-mechanics.md#photon) mass $m_\gamma^2A_\mu A^\mu/2$ is not.

The classical [Maxwell equations](../../../electromagnetism.md#maxwell-equations) are $\partial_\mu F^{\mu\nu}=j^\nu$, with $j^\nu=e\bar\psi\gamma^\nu\psi$. Taking a divergence gives $\partial_\nu j^\nu=0$ because $F^{\mu\nu}$ is antisymmetric. The same conservation law follows directly from the charged [Dirac equation](../../../relativistic-quantum-field.md#dirac-equation) and its adjoint. For vanishing flux at spatial infinity, $Q=\int d^3x\,j^0$ is conserved. [Gauss law](../../../electromagnetism.md#gauss-s-law) identifies this charge with the electric flux through a surrounding surface. Particle-antiparticle creation is allowed, but its net [electric charge](../../../electromagnetism.md#electric-charge) is zero.

Local [gauge invariance](../../../relativistic-quantum-field.md#gauge-invariance) is also a redundancy in the potentials, rather than an extra propagating degree of freedom. The [canonical momentum](../../../classical-mechanics.md#canonical-momentum) of $A_0$ vanishes, and its field equation enforces the [Gauss law constraint in gauge theory](../../../relativistic-quantum-field.md#gauss-law-constraint-in-gauge-theory), $\boldsymbol\nabla\cdot\mathbf E=j^0$. After imposing the constraint and quotienting gauge freedom, a massless [photon](../../../quantum-mechanics.md#photon) has **two transverse physical polarizations**. [Gauge transformations](../../../electromagnetism.md#gauge-transformation) vanishing at the boundary identify equivalent descriptions; constant phase transformations at infinity can act on charged states and generate their conserved charge. This distinction explains why gauge redundancy and [electric charge](../../../electromagnetism.md#electric-charge) are compatible.

In perturbative [QED](../../../perturbative-quantum-field-theory.md#quantum-electrodynamics), the quadratic [photon](../../../quantum-mechanics.md#photon) operator cannot be inverted before [gauge fixing](../../../relativistic-quantum-field.md#gauge-fixing). Adding $-(\partial_\mu A^\mu)^2/(2\xi)$ gives the [covariant gauge](../../../relativistic-quantum-field.md#covariant-gauge) propagator

$$
D_{\mu\nu}(k)=\frac{-i}{k^2+i0}\left[g_{\mu\nu}-(1-\xi)\frac{k_\mu k_\nu}{k^2+i0}\right].
$$

This propagator contains longitudinal and timelike components, but these are not external physical [photon](../../../quantum-mechanics.md#photon) states. A [Gupta-Bleuler null-state quotient](../../../relativistic-quantum-field.md#gupta-bleuler-null-state-quotient), or the equivalent [BRST](../../../relativistic-quantum-field.md#brst-symmetry) construction, removes them. In linear [Lorenz gauge](../../../electromagnetism.md#lorenz-gauge-condition), $\delta(\partial_\mu A^\mu)=\Box\alpha$, so the [Faddeev-Popov determinant](../../../relativistic-quantum-field.md#faddeev-popov-determinant) is independent of $A_\mu$ and the [Faddeev-Popov ghost fields](../../../relativistic-quantum-field.md#faddeev-popov-ghost) decouple. This last statement concerns the linear gauge; Abelian [gauge groups](../../../relativistic-quantum-field.md#gauge-group) alone do not guarantee decoupling in a nonlinear gauge condition.

At the quantum level, the vector symmetry gives a [Ward identity](../../../perturbative-quantum-field-theory.md#ward-identity). One way to obtain it is to change variables by a localized phase in a time-ordered correlation function containing $\psi(y)$ and $\bar\psi(z)$. The action variation becomes a current divergence; the two field insertions contribute opposite contact terms, since their charges are opposite. [Fourier transformation](../../../analysis.md#fourier-transform) turns the divergence into the [photon](../../../quantum-mechanics.md#photon) momentum, and amputating the external [fermion](../../../quantum-mechanics.md#fermion) propagators turns the two contact terms into the difference of their inverse propagators. With the charge removed from the proper vertex and the overall propagator factor $i$ removed from its inverse, the result is the [proper-vertex Ward-Takahashi identity in QED](../../../perturbative-quantum-field-theory.md#proper-vertex-ward-takahashi-identity-in-qed)

$$
\boxed{k_\mu\Gamma^\mu(p+k,p)=S^{-1}(p+k)-S^{-1}(p).}
$$

At tree level this is simply $k_\mu\gamma^\mu=(\not p+\not k-m)-(\not p-m)$. Between on-shell external spinors, the inverse propagators vanish, so the full physical [scattering amplitude](../../../quantum-mechanics.md#scattering-amplitude) satisfies $k_\mu\mathcal M^\mu=0$. Therefore replacing a [photon polarization vector](../../../quantum-mechanics.md#photon-polarization-vector) by $\varepsilon_\mu+c k_\mu$ leaves the amplitude unchanged. The identity applies to the complete required sum of diagrams, not necessarily each diagram separately. It also ensures cancellation of the gauge parameter from physical observables when all terms at the chosen perturbative order are included.

For the [photon](../../../quantum-mechanics.md#photon) two-point function, the [Ward identity](../../../perturbative-quantum-field-theory.md#ward-identity) implies transverse [photon vacuum polarization](../../../perturbative-quantum-field-theory.md#photon-vacuum-polarization):

$$
k_\mu\Pi^{\mu\nu}(k)=0,\qquad
\Pi^{\mu\nu}(k)=(k^2g^{\mu\nu}-k^\mu k^\nu)\Pi(k^2).
$$

Thus ultraviolet subtraction renormalizes the gauge-invariant kinetic term, rather than requiring a local photon-mass [counterterm](../../../perturbative-quantum-field-theory.md#counterterm). Perturbative unbroken [QED](../../../perturbative-quantum-field-theory.md#quantum-electrodynamics) retains a massless [photon](../../../quantum-mechanics.md#photon). Transversality by itself would not exclude a nonlocal massless pole in a different theory; the assertion here includes the perturbative [QED](../../../perturbative-quantum-field-theory.md#quantum-electrodynamics) setting.

Taking $k\to0$ in the proper-vertex identity gives $\Gamma^\mu(p,p)=\partial S^{-1}(p)/\partial p_\mu$. Matching the divergent coefficients of the derivative and vertex terms yields the [Ward identity for QED renormalization constants](../../../perturbative-quantum-field-theory.md#ward-identity-for-qed-renormalization-constants), $Z_1=Z_2$, in a gauge-preserving prescription. If $\psi_0=\sqrt{Z_2}\psi$ and $A_0=\sqrt{Z_3}A$, comparison of the interaction coefficients gives

$$
e_0=\mu_R^\epsilon\frac{Z_1}{Z_2\sqrt{Z_3}}e
=\mu_R^\epsilon Z_3^{-1/2}e\qquad(d=4-2\epsilon).
$$

Hence **[charge renormalization](../../../perturbative-quantum-field-theory.md#charge-renormalization) is fixed by [photon](../../../quantum-mechanics.md#photon) [wave-function renormalization](../../../perturbative-quantum-field-theory.md#wave-function-renormalization)**. [Gauge invariance](../../../relativistic-quantum-field.md#gauge-invariance) constrains [counterterms](../../../perturbative-quantum-field-theory.md#counterterm) and relates renormalizations; it does not make the [electric charge](../../../electromagnetism.md#electric-charge) independent of scale.

The [Soft photon theorem](../../../perturbative-quantum-field-theory.md#soft-photon-theorem) gives another physical manifestation. Attaching a [photon](../../../quantum-mechanics.md#photon) of small momentum $k$ to the external charged legs gives the leading factor

$$
\mathcal M_{\mathrm{soft}}=e\mathcal M_{\mathrm{hard}}\sum_i\eta_iQ_i\frac{p_i\cdot\varepsilon}{p_i\cdot k}+O(k^0),
$$

where $Q_i$ is charge in units of $e$ and $\eta_i=+1$ for outgoing and $-1$ for incoming legs. Replacing $\varepsilon$ by $k$ makes this factor proportional to $\sum_i\eta_iQ_i$, which vanishes by [electric charge conservation](../../../electromagnetism.md#charge-conservation). Massless [photons](../../../quantum-mechanics.md#photon) also cause [infrared divergences](../../../quantum-field-theory.md#infrared-divergence); physical inclusive measurements combine unresolved real emission with virtual corrections, rather than treating either contribution alone as an observable.

Finally, the vector gauge symmetry of a Dirac [fermion](../../../quantum-mechanics.md#fermion) in [QED](../../../perturbative-quantum-field-theory.md#quantum-electrodynamics) is anomaly-free, so it can be maintained by regularization and [renormalization](../../../perturbative-quantum-field-theory.md#renormalization). This must be distinguished from the [axial current](../../../relativistic-quantum-field.md#axial-current): its divergence has explicit mass terms, as in Question 3, and can additionally have a quantum [chiral anomaly](../../../relativistic-quantum-field.md#chiral-anomaly). Conservation of the gauge current does not imply axial-current conservation. The resulting picture is that [gauge invariance](../../../relativistic-quantum-field.md#gauge-invariance) simultaneously organizes the physical [photon](../../../quantum-mechanics.md#photon) states, enforces electric-charge conservation and ties together amplitudes and ultraviolet subtractions.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2006](../../2006.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
