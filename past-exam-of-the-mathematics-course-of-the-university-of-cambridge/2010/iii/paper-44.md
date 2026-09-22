# Paper 44

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2010/Paper44.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2010/Paper44.pdf)

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

↑ **Parent:** [Paper 44](paper-44.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Use target-space signature $(-,+,+,+)$ and [conformal gauge](../../../string-theory.md#conformal-gauge) $g_{ab}=e^{2\omega}\operatorname{diag}(-1,1)$. Dots and primes denote differentiation with respect to $\tau$ and $\sigma$. Varying the [Polyakov action](../../../string-theory.md#polyakov-action) with respect to the [string embedding map](../../../string-theory.md#string-embedding-map) gives the [wave equation](../../../wave-equation.md); varying the [worldsheet metric](../../../string-theory.md#worldsheet-metric) sets the [worldsheet stress tensor](../../../string-theory.md#worldsheet-stress-energy-tensor) to zero. Explicitly,

$$
\boxed{\ddot X^\mu-X^{\mu\prime\prime}=0,\qquad \dot X^2+X'^2=0,\qquad \dot X\cdot X'=0.}
$$

With $\sigma^\pm=\tau\pm\sigma$ and $\partial_\pm=\tfrac12(\partial_\tau\pm\partial_\sigma)$, the two [Virasoro constraints](../../../string-theory.md#virasoro-constraint) are $(\partial_+X)^2=(\partial_-X)^2=0$.

A fixed spatial circle would sweep out a cylindrical [string worldsheet](../../../string-theory.md#worldsheet). In static coordinates its [string embedding map](../../../string-theory.md#string-embedding-map) is $X=(t,R\cos\theta,R\sin\theta,0)$ and its [induced worldsheet metric](../../../string-theory.md#induced-worldsheet-metric) is $\operatorname{diag}(-1,R^2)$. The radial part of the [Nambu–Goto equations of motion](../../../string-theory.md#nambu-goto-equations-of-motion) is proportional to $R^{-2}\partial_\theta^2(R\cos\theta,R\sin\theta)=-(\cos\theta,\sin\theta)/R$, which is nonzero. Thus a nonzero-radius cylinder cannot solve the equations. Motion of labels around this same cylinder is a [worldsheet diffeomorphism](../../../string-theory.md#worldsheet-diffeomorphism) and cannot alter this conclusion.

The familiar [pulsating circular string](../../../string-theory.md#pulsating-circular-string) makes the obstruction particularly explicit. Put $X^0=\kappa\tau$ and $X^1+iX^2=r(\tau)e^{i\sigma}$. The [wave equation](../../../wave-equation.md) and [Virasoro constraints](../../../string-theory.md#virasoro-constraint) reduce to

$$
\ddot r+r=0,\qquad \dot r^2+r^2=\kappa^2.
$$

A constant $r=R\ne0$ violates the first equation. Even rotating the labels, $X^1+iX^2=Re^{i(\sigma+\Omega\tau)}$, cannot help: the [wave equation](../../../wave-equation.md) requires $\Omega^2=1$, whereas $\dot X\cdot X'=R^2\Omega$ requires $\Omega=0$.

Nor does a rigid rotation of the circular plane rescue the usual circular ansatz in three spatial dimensions. Write its spatial part as $A(\tau)\cos\sigma+B(\tau)\sin\sigma$, with $A^2=B^2=R^2$ and $A\cdot B=0$. The [wave equation](../../../wave-equation.md) gives $\ddot A=-A$ and $\ddot B=-B$. The constant norms give $A\cdot\dot A=B\cdot\dot B=0$ and $\dot A^2=\dot B^2=R^2$. The mixed [Virasoro constraint](../../../string-theory.md#virasoro-constraint), together with the derivative of $A\cdot B=0$, gives $\dot A\cdot B=A\cdot\dot B=0$. Differentiating $A\cdot B$ twice gives $\dot A\cdot\dot B=0$. This would require four mutually orthogonal nonzero spatial vectors in $\mathbb R^3$. This obstruction is specific to the stated spatial dimension; a [rigid circular string in four spatial dimensions](../../../string-theory.md#rigid-circular-string-in-four-spatial-dimensions) has more room.

To express the [Virasoro constraints](../../../string-theory.md#virasoro-constraint) in modes, extend the [string oscillators](../../../string-theory.md#string-oscillator) by

$$
\alpha_0^\mu=\widetilde\alpha_0^\mu=\sqrt{\frac{\alpha'}2}\,p^\mu.
$$

Differentiating the two chiral expansions gives $\partial_-X^\mu=\sqrt{\alpha'/2}\sum_n\alpha_n^\mu e^{-in\sigma^-}$ and the corresponding expression with tildes for $\partial_+X$. Equating every [Fourier coefficient](../../../fourier-series.md#fourier-coefficient) of their squares to zero yields

$$
L_m=\frac12\sum_{n\in\mathbb Z}\alpha_{m-n}\cdot\alpha_n=0,\qquad \widetilde L_m=\frac12\sum_{n\in\mathbb Z}\widetilde\alpha_{m-n}\cdot\widetilde\alpha_n=0\quad(m\in\mathbb Z).
$$

Reality of the [string embedding map](../../../string-theory.md#string-embedding-map) means $\alpha_{-n}=\alpha_n^*$ and $\widetilde\alpha_{-n}=\widetilde\alpha_n^*$. In particular, define the classical [string level operators](../../../string-theory.md#string-level-operator) by $N=\sum_{n>0}\alpha_{-n}\cdot\alpha_n$ and $\widetilde N=\sum_{n>0}\widetilde\alpha_{-n}\cdot\widetilde\alpha_n$. The zero-mode [Virasoro constraints](../../../string-theory.md#virasoro-constraint) become

$$
0=L_0=\frac{\alpha'}4p^2+N,\qquad 0=\widetilde L_0=\frac{\alpha'}4p^2+\widetilde N.
$$

Consequently the classical [bosonic string mass spectrum](../../../string-theory.md#bosonic-string-mass-spectrum) is

$$
\boxed{M^2=-p^2=\frac{4N}{\alpha'}=\frac{4\widetilde N}{\alpha'},\qquad N=\widetilde N.}
$$

The equality of the two levels is [closed-string level matching](../../../string-theory.md#closed-string-level-matching). There is no [string intercept](../../../string-theory.md#normal-ordering-constant-of-a-string) here: that shift comes from quantum [normal ordering](../../../perturbative-quantum-field-theory.md#normal-ordering), not from these classical equations.

For the [compact boson](../../../string-theory.md#compact-boson), closed-string periodicity permits a winding number $w\in\mathbb Z$, so $X^3(\sigma+2\pi)-X^3(\sigma)=2\pi wR$. Let $q$ be the momentum in this direction. Its zero-mode expansion and the corresponding chiral momenta are

$$
X^3=x^3+\alpha' q\tau+wR\sigma+\text{oscillators},\qquad p_L^3=q+\frac{wR}{\alpha'},\qquad p_R^3=q-\frac{wR}{\alpha'}.
$$

Thus replace the equal left and right zero modes by $\widetilde\alpha_0^3=\sqrt{\alpha'/2}\,p_L^3$ and $\alpha_0^3=\sqrt{\alpha'/2}\,p_R^3$; the nonzero [string oscillators](../../../string-theory.md#string-oscillator) remain integer-moded. Classically $q$ is continuous. Quantizing the [compact boson](../../../string-theory.md#compact-boson) makes momentum wavefunctions single-valued around its circle, giving $q=n/R$ with $n\in\mathbb Z$.

If $k^a$, $a=0,1,2$, is the noncompact momentum and $M^2=-k^ak_a$, the two zero-mode [Virasoro constraints](../../../string-theory.md#virasoro-constraint) give

$$
M^2=\left(q+\frac{wR}{\alpha'}\right)^2+\frac{4\widetilde N}{\alpha'}=\left(q-\frac{wR}{\alpha'}\right)^2+\frac{4N}{\alpha'}.
$$

Averaging and subtracting gives the [momentum and winding modes](../../../string-theory.md#momentum-and-winding-modes) and [compact-circle closed-string level matching](../../../string-theory.md#compact-circle-closed-string-level-matching) formulas

$$
\boxed{M^2=q^2+\frac{w^2R^2}{\alpha'^2}+\frac{2(N+\widetilde N)}{\alpha'},\qquad \widetilde N-N+qwR=0.}
$$

The latter becomes $\widetilde N-N+nw=0$ on imposing quantum momentum quantization. The sign follows from assigning tildes to the left mover $\sigma^+$.

An explicit [winding-supported circular string](../../../string-theory.md#winding-supported-circular-string), valid classically for every $R>0$, is

$$
\boxed{X^0=2R\tau,\quad X^1=R\cos(\sigma+\tau),\quad X^2=R\sin(\sigma+\tau),\quad X^3=R(\sigma-\tau)\pmod{2\pi R}.}
$$

The noncompact projection is a circle of constant radius. Every coordinate obeys the [wave equation](../../../wave-equation.md). Its compact winding is $w=1$, and a direct calculation gives

$$
\dot X^2=-2R^2,\qquad X'^2=2R^2,\qquad \dot X\cdot X'=R^2-R^2=0.
$$

Thus both [Virasoro constraints](../../../string-theory.md#virasoro-constraint) hold and the [induced worldsheet metric](../../../string-theory.md#induced-worldsheet-metric) is $2R^2\operatorname{diag}(-1,1)$, not a degenerate cylinder. The compact motion cancels the mixed stress that spoiled rotation of labels in flat space. Here $q=-R/\alpha'$, $N=0$ and $\widetilde N=R^2/\alpha'$ satisfy the classical [compact-circle closed-string level matching](../../../string-theory.md#compact-circle-closed-string-level-matching) condition. Requiring this particular classical momentum to equal an individual quantum eigenvalue would impose an additional radius-dependent condition; that is not required to construct the classical solution.

## 2

↑ **Parent:** [Paper 44](paper-44.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

Use the free-boson [operator product expansion](../../../string-theory.md#operator-product-expansion)

$$
X^\mu(z,\bar z)X^\nu(w,\bar w)\sim-\frac{\alpha'}2\eta^{\mu\nu}\log|z-w|^2.
$$

Write $E_p=:e^{ip\cdot X}:$ and $\epsilon=z-w$. The needed [Wick contractions](../../../perturbative-quantum-field-theory.md#wick-contraction) are $\partial X^\mu(z)\partial X^\nu(w)\sim-\alpha'\eta^{\mu\nu}/(2\epsilon^2)$ and $\partial X^\mu(z)E_p(w)\sim-i\alpha'p^\mu E_p(w)/(2\epsilon)$. For $V_\zeta=\zeta_\mu:\partial X^\mu E_p:$, the cross double contraction in the [worldsheet stress tensor](../../../string-theory.md#worldsheet-stress-energy-tensor) has a cubic pole: either of its two derivatives can contract with the derivative in $V_\zeta$, while the other contracts with $E_p$. Including the factor $-1/\alpha'$ gives

$$
T(z)V_\zeta(w)\sim-\frac{i\alpha'}2\frac{p\cdot\zeta}{\epsilon^3}E_p(w)+\frac{1+\alpha'p^2/4}{\epsilon^2}V_\zeta(w)+\frac1\epsilon\partial V_\zeta(w).
$$

A [primary operator](../../../string-theory.md#primary-field) has no cubic pole. Hence **the first vertex is primary precisely when**

$$
\boxed{p\cdot\zeta=0,\qquad h=1+\alpha'p^2/4.}
$$

The antiholomorphic [conformal weight](../../../string-theory.md#conformal-weight) is $\bar h=\alpha'p^2/4$. Primarity alone puts no [mass-shell condition](../../../string-theory.md#string-mass-shell-condition) on $p$.

For $W_\zeta=\zeta_{\mu\nu}:\partial X^\mu\bar\partial X^\nu E_p:$, the holomorphic cubic pole is $-i\alpha'p^\mu\zeta_{\mu\nu}:\bar\partial X^\nu E_p:/(2\epsilon^3)$. The antiholomorphic [operator product expansion](../../../string-theory.md#operator-product-expansion) gives the analogous pole involving $p^\nu\zeta_{\mu\nu}$. Thus the [transversality of derivative-exponential primary vertices](../../../string-theory.md#transversality-of-derivative-exponential-primary-vertices) requires

$$
\boxed{p^\mu\zeta_{\mu\nu}=0,\qquad p^\nu\zeta_{\mu\nu}=0,\qquad (h,\bar h)=(1+\alpha'p^2/4,1+\alpha'p^2/4).}
$$

There is no trace-free requirement for primarity. A physical [integrated string vertex operator](../../../string-theory.md#integrated-string-vertex-operator) must additionally have [conformal weights](../../../string-theory.md#conformal-weight) $(1,1)$; for this vertex that gives $p^2=0$.

Now keep the [fermionic signs](../../../perturbative-quantum-field-theory.md#fermionic-sign) in the real chiral [Majorana fermion](../../../relativistic-quantum-field.md#majorana-spinor) calculation. Contracting the external $\psi(w)$ through $:\psi(z)\partial\psi(z):$ gives

$$
:\psi(z)\partial\psi(z):\,\psi(w)\sim-\frac{\partial\psi(z)}{\epsilon}-\frac{\psi(z)}{\epsilon^2}.
$$

Multiplying by $-1/2$ and Taylor expanding $\psi(z)$ at $w$ produces

$$
T(z)\psi(w)\sim\frac{\psi(w)}{2\epsilon^2}+\frac{\partial\psi(w)}\epsilon.
$$

This proves that $\psi$ is a [primary operator](../../../string-theory.md#primary-field) with **weight $h_\psi=1/2$**. To find the [central charge](../../../string-theory.md#central-charge), in $T(z)T(w)$ the two double-contraction pairings contribute, before the overall factor $1/4$,

$$
-\langle\psi(z)\psi(w)\rangle\langle\partial\psi(z)\partial\psi(w)\rangle=\frac2{\epsilon^4},\qquad \langle\psi(z)\partial\psi(w)\rangle\langle\partial\psi(z)\psi(w)\rangle=-\frac1{\epsilon^4}.
$$

The single [Wick contractions](../../../perturbative-quantum-field-theory.md#wick-contraction) give $2T(w)/\epsilon^2+\partial T(w)/\epsilon$, so

$$
T(z)T(w)\sim\frac1{4\epsilon^4}+\frac{2T(w)}{\epsilon^2}+\frac{\partial T(w)}\epsilon.
$$

Comparing the leading term with $c/(2\epsilon^4)$ proves **$c_\psi=1/2$**, as in the [free chiral Majorana fermion conformal field theory](../../../string-theory.md#free-chiral-majorana-fermion-conformal-field-theory).

With four embedding bosons and the ordinary reparameterization [bc ghost system](../../../string-theory.md#bc-system), cancellation of the [worldsheet Weyl anomaly](../../../string-theory.md#worldsheet-weyl-anomaly) in each chirality requires

$$
4+\frac{N_f}2-26=0,\qquad\boxed{N_f=44.}
$$

Thus there are **44 real left-moving and 44 real right-moving fermions**, equivalently 44 two-dimensional nonchiral [Majorana fermions](../../../relativistic-quantum-field.md#majorana-spinor). These are [internal free fermions in a four-dimensional bosonic string](../../../string-theory.md#internal-free-fermions-in-a-four-dimensional-bosonic-string). Adding internal matter to the bosonic string does not introduce local [worldsheet supersymmetry](../../../string-theory.md#worldsheet-supersymmetry) or its superghosts.

For the requested polynomial [string vertex operators](../../../string-theory.md#string-vertex-operator), work in the unprojected [Neveu–Schwarz sector](../../../string-theory.md#neveu-schwarz-sector). A full model also chooses spin structures and a consistent projection, which the central-charge condition alone does not specify. If the holomorphic and antiholomorphic oscillator contributions to the [conformal weights](../../../string-theory.md#conformal-weight) are $\ell_L,\ell_R$, physicality requires

$$
\ell_L+\frac{\alpha'p^2}4=\ell_R+\frac{\alpha'p^2}4=1,\qquad M^2=\frac4{\alpha'}(\ell_L-1),\qquad \ell_L=\ell_R.
$$

Therefore only equal levels at most one can contribute to the requested nonpositive [bosonic string mass spectrum](../../../string-theory.md#bosonic-string-mass-spectrum).

With zero fermion insertions, level zero gives the [tachyon vertex operator](../../../string-theory.md#tachyon-vertex-operator) $E_p$, a scalar with $M^2=-4/\alpha'$. Level one gives the [massless closed-string vertex operator](../../../string-theory.md#massless-closed-string-vertex-operator) $\zeta_{\mu\nu}:\partial X^\mu\bar\partial X^\nu E_p:$, with the transverse conditions above and the [string-state gauge redundancy](../../../string-theory.md#string-state-gauge-redundancy) that removes longitudinal polarizations. The physical transverse [polarization tensor](../../../string-theory.md#polarization-tensor) decomposes into a symmetric trace-free [graviton](../../../quantum-theory.md#graviton), an antisymmetric [Kalb–Ramond field](../../../string-theory.md#kalb-ramond-field), and a scalar [dilaton](../../../string-theory.md#dilaton). In four spacetime dimensions these have respectively two, one, and one physical polarizations; the two-form can be dualized to a scalar.

With two fermion insertions there are two possibilities. One fermion in each chirality gives

$$
C_{ij}:\psi^i\bar\psi^j E_p:,qquad (\ell_L,\ell_R)=(1/2,1/2),\qquad \boxed{M^2=-2/\alpha'.}
$$

These are **$44^2=1936$ scalar tachyons** before any projection. There is no spacetime derivative or spacetime polarization to impose a vector transversality condition.

Two different fermions in the same chirality form an antisymmetric [fermion bilinear](../../../relativistic-quantum-field.md#fermion-bilinear), a weight-one current $J^{ij}=: \psi^i\psi^j:$; equal-species undifferentiated bilinears vanish. [Closed-string level matching](../../../string-theory.md#closed-string-level-matching) then requires a weight-one bosonic derivative in the opposite chirality. The resulting [string vertex operators](../../../string-theory.md#string-vertex-operator) are

$$
A^{ij}_\mu:\psi^i\psi^j\bar\partial X^\mu E_p:,qquad \widetilde A^{ij}_\mu:\partial X^\mu\bar\psi^i\bar\psi^j E_p:,qquad i<j.
$$

They have **$M^2=0$ and are gauge vectors**, with $p\cdot A^{ij}=0$ and $A^{ij}_\mu\sim A^{ij}_\mu+p_\mu\lambda^{ij}$, and likewise for $\widetilde A$. Each chirality supplies $\binom{44}{2}=946$ gauge vectors. The [fermion bilinears](../../../relativistic-quantum-field.md#fermion-bilinear) generate the two $\mathfrak{so}(44)$ current algebras associated with the [Special orthogonal Lie algebra](../../../semisimple-lie-algebra.md#special-orthogonal-lie-algebra), giving the unprojected [gauge group](../../../relativistic-quantum-field.md#gauge-group) $SO(44)_L\times SO(44)_R$. The tempting vertex $:\psi^i\psi^j E_p:$ alone fails [closed-string level matching](../../../string-theory.md#closed-string-level-matching) because its weights are $(1,0)$ before the common momentum contribution. Additional derivatives raise the levels above the nonpositive-mass range; a product of a left and a right bilinear has four fermion insertions and is outside this requested sector. This completes the [zero- and two-fermion vertices of an internally fermionized bosonic string](../../../string-theory.md#zero-and-two-fermion-vertices-of-an-internally-fermionized-bosonic-string); a specified global projection can remove some of the listed states.

## 3

↑ **Parent:** [Paper 44](paper-44.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

Locally in the space of [worldsheet metrics](../../../string-theory.md#worldsheet-metric), divide out the volume of [worldsheet diffeomorphisms](../../../string-theory.md#worldsheet-diffeomorphism) and [Weyl transformations](../../../string-theory.md#weyl-transformation). With stabilizer zero modes omitted, the inverse [Faddeev-Popov determinant](../../../relativistic-quantum-field.md#faddeev-popov-determinant) at a metric $g$ is

$$
\boxed{\Delta_{\rm FP}^{-1}[g]=\int D\omega\,Dv\ \delta\!\left[2\omega g_{ab}+\nabla_a v_b+\nabla_b v_a\right].}
$$

This is the linearized orbit integral: the delta functional is the product of the metric-component delta functions, and its Jacobian is the inverse determinant of the gauge-orbit map. The omitted zero modes and any metric moduli must be handled separately; this local formula is not an integration over the physical moduli themselves.

The [trace elimination in string Faddeev-Popov gauge fixing](../../../string-theory.md#trace-elimination-in-string-faddeev-popov-gauge-fixing) is essential. In two dimensions, split the variation as

$$
\delta g_{ab}=(2\omega+\nabla\cdot v)g_{ab}+(P_1v)_{ab},\qquad (P_1v)_{ab}=\nabla_av_b+\nabla_bv_a-g_{ab}\nabla\cdot v.
$$

The second term is trace-free. Integration over $\omega$ removes the trace delta function, leaving $\int Dv\,\delta[P_1v]=(\det{}'P_1)^{-1}$, with the measure understood through the metric inner products. Equivalently, a Fourier representation of the metric delta functional introduces a commuting symmetric tensor $\beta^{ab}$. Integration over $\omega$ enforces $g_{ab}\beta^{ab}=0$, and the remaining exponent is proportional to $\int\sqrt g\,\beta^{ab}(P_1v)_{ab}$. This gives the same inverse [Faddeev-Popov determinant](../../../relativistic-quantum-field.md#faddeev-popov-determinant) and explains why its tensor variable must be trace-free.

For the [Polyakov path integral](../../../string-theory.md#polyakov-path-integral), insert the gauge-fixing identity

$$
1=\Delta_{\rm FP}[g]\int D\omega\,Dv\ \delta[g^{\omega,v}-\widehat g(m)],
$$

where $\widehat g(m)$ is a representative depending on the [worldsheet moduli](../../../string-theory.md#worldsheet-moduli) $m$. Gauge invariance of the action, measure, and [Faddeev-Popov determinant](../../../relativistic-quantum-field.md#faddeev-popov-determinant) lets us change variables along the gauge orbit. Its volume cancels the original gauge-group denominator, leaving an integral over $X$, the moduli, and the determinant evaluated at $\widehat g$. This is how the determinant enters the numerator of the gauge-fixed integral, despite the inverse determinant occurring in the orbit integral above.

A [fermionic Gaussian integral](../../../quantum-field-theory.md#grassmann-gaussian-integral) exponentiates $\det{}'P_1$ using an anticommuting vector $c^a$ and an anticommuting symmetric trace-free tensor $b^{ab}$:

$$
\det{}'P_1\ \propto\ \int Db\,Dc\ \exp\!\left[-C\int d^2\sigma\sqrt g\,b^{ab}(P_1c)_{ab}\right].
$$

The constant $C$ can be absorbed into $b$. In local complex [conformal gauge](../../../string-theory.md#conformal-gauge), trace-freeness sets $b_{z\bar z}=0$. The only surviving components of the [worldsheet diffeomorphism ghost operator](../../../string-theory.md#worldsheet-diffeomorphism-ghost-operator) are proportional to $\bar\partial c^z$ and $\partial c^{\bar z}$. Rescaling the antighost therefore gives exactly the chiral [worldsheet ghost action](../../../string-theory.md#worldsheet-ghost-action)

$$
\boxed{S_{\rm gh}=\int d^2z\left(b_{zz}\bar\partial c^z+b_{\bar z\bar z}\partial c^{\bar z}\right).}
$$

The chiral [bc ghost system](../../../string-theory.md#bc-system) has weights $h_b=2$, $h_c=-1$, with $b(z)c(w)\sim1/(z-w)$. Its [worldsheet stress tensor](../../../string-theory.md#worldsheet-stress-energy-tensor) is $T_{\rm gh}=-2:b\partial c:-:(\partial b)c:$. Fermionic double [Wick contractions](../../../perturbative-quantum-field-theory.md#wick-contraction) in $T_{\rm gh}T_{\rm gh}$ give the fourth-order coefficient $-13$, hence [central charge](../../../string-theory.md#central-charge) $c_{\rm gh}=-26$. More generally this calculation gives $c=1-3(2h_b-1)^2$. Each embedding scalar contributes one, so the total chiral [central charge](../../../string-theory.md#central-charge) is $D-26$. The gauge-fixed quantum theory must have no [worldsheet Weyl anomaly](../../../string-theory.md#worldsheet-weyl-anomaly); consequently **the [critical dimension of the bosonic string](../../../string-theory.md#critical-dimension-of-string-theory) is $D=26$**. Zero-mode insertions for [Conformal Killing vector fields](../../../general-relativity.md#conformal-killing-vector-field) and moduli do not change this local anomaly calculation.

For the [Veneziano amplitude](../../../string-theory.md#veneziano-amplitude), first examine an ordered beta-function term. A pole occurs when $-\alpha's-1=-n$, with $n=0,1,2,\ldots$, so the exchanged masses follow the [open bosonic string mass spectrum](../../../string-theory.md#open-bosonic-string-mass-spectrum)

$$
\boxed{M_n^2=\frac{n-1}{\alpha'},\qquad n=0,1,2,\ldots.}
$$

There is a tachyon at level zero, a massless vector at level one, then an infinite tower with equally spaced squared masses. In oscillator quantization these levels are $N=n$; the poles alone do not determine all oscillator degeneracies or all states that might fail to couple to the chosen external particles.

The [Veneziano amplitude pole residue](../../../string-theory.md#veneziano-amplitude-pole-residue) gives considerably more information than a pole position. Near $s_n=(n-1)/\alpha'$, use $\Gamma(-n+\epsilon)\sim(-1)^n/(n!\epsilon)$ and $\epsilon=-\alpha'(s-s_n)$. The finite [gamma function](../../../complex-analysis.md#gamma-function) ratio is a product of $n$ linear factors. Thus, for generic $t$,

$$
\operatorname*{Res}_{s=s_n}B(-\alpha's-1,-\alpha't-1)=-\frac1{\alpha'n!}\prod_{j=1}^{n}(\alpha't+j+1).
$$

The empty product at $n=0$ is one. This degree-$n$ angular polynomial decomposes into spin [partial waves](../../../quantum-mechanics.md#partial-wave); it reveals the spins that couple, up to maximal spin $n$ in the ordered channel, and the corresponding products of three-point couplings. For example, the level-one linear residue encodes vector exchange. A single external-state amplitude need not separate all states with the same mass and spin.

There is a qualification specific to the sum printed in the question. For four identical on-shell tachyons, $s+t+u=-4/\alpha'$. At $\alpha's=n-1$, put $P_n(t)=\prod_{j=1}^n(\alpha't+j+1)$. Then $\alpha'u=-n-3-\alpha't$, and reversing the product gives $P_n(u)=(-1)^nP_n(t)$. The $t,u$ beta-function term is regular at a generic $s$-channel pole. The residue of the full symmetric amplitude is therefore proportional to

$$
-\frac{1+(-1)^n}{\alpha'n!}\,P_n(t).
$$

This is [odd-level pole cancellation in the symmetric Veneziano amplitude](../../../string-theory.md#odd-level-pole-cancellation-in-the-symmetric-veneziano-amplitude). **The fully symmetrized identical-tachyon amplitude has only even-level poles at generic angle**, including the tachyon but not the massless vector. This is an external-state selection rule, not removal of odd-level states from the string theory. Ordered amplitudes, or suitable amplitudes with color factors and different external states, retain those exchanges. Thus interpreting every candidate [gamma function](../../../complex-analysis.md#gamma-function) pole as a pole of the printed sum would give a false inference about that amplitude.

At high energy with $x=-t/s\in(0,1)$ fixed, the [gamma function](../../../complex-analysis.md#gamma-function) reflection formula followed by the [Stirling formula](../../../real-analysis.md#stirling-formula) gives the [fixed-angle softness of an open-string amplitude](../../../string-theory.md#fixed-angle-softness-of-an-open-string-amplitude):

$$
\log|A|=-\alpha's\left[-x\log x-(1-x)\log(1-x)\right]+O(\log s),
$$

up to oscillatory factors and possible additional cancellations. The bracket is positive at a genuinely nonforward fixed angle. This is the envelope away from resonance poles, or the corresponding analytically continued asymptotic regime; it is not a uniform bound through real-axis poles. **String scattering is exponentially soft at fixed angle**, unlike the typical power-law behavior of point-particle interactions. The finite string length distributes a hard collision over an extended object. This is evidence of improved ultraviolet behavior, not by itself a proof that every loop amplitude is finite. The fixed-angle limit also differs from the fixed-$t$ [Regge limit](../../../string-theory.md#regge-limit).

## 4

↑ **Parent:** [Paper 44](paper-44.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

Choose a Euclidean [string worldsheet](../../../string-theory.md#worldsheet) and the usual normalization of the [Polyakov action](../../../string-theory.md#polyakov-action). For a closed oriented worldsheet $\Sigma$, the [string nonlinear sigma model](../../../string-theory.md#string-nonlinear-sigma-model) is

$$
\boxed{\begin{aligned}
S={}&\frac1{4\pi\alpha'}\int_\Sigma d^2\sigma\sqrt g\,g^{ab}G_{\mu\nu}(X)\partial_aX^\mu\partial_bX^\nu\\
&+\frac{i}{4\pi\alpha'}\int_\Sigma d^2\sigma\,\varepsilon^{ab}B_{\mu\nu}(X)\partial_aX^\mu\partial_bX^\nu
+\frac1{4\pi}\int_\Sigma d^2\sigma\sqrt g\,\Phi(X)R^{(2)}.
\end{aligned}}
$$

Here $\varepsilon^{12}=1$ is the alternating density, not the tensor with components $1/\sqrt g$. The imaginary coefficient in the [Kalb–Ramond field](../../../string-theory.md#kalb-ramond-field) term is the Euclidean continuation; in Lorentzian signature this term is real. $G$ is the spacetime metric and $\Phi$ the [dilaton](../../../string-theory.md#dilaton).

All three terms have [worldsheet diffeomorphism](../../../string-theory.md#worldsheet-diffeomorphism) invariance, and are covariant under [spacetime](../../../special-relativity.md#spacetime) coordinate transformations when $X$, $G$, $B$ and $\Phi$ are transformed together. Under a [Weyl transformation](../../../string-theory.md#weyl-transformation) $g_{ab}\mapsto e^{2\omega}g_{ab}$, $\sqrt g\,g^{ab}$ is invariant in two dimensions, so the metric coupling has classical [Weyl invariance](../../../string-theory.md#weyl-transformation). The antisymmetric coupling is independent of the [worldsheet metric](../../../string-theory.md#worldsheet-metric), so it too has classical [Weyl invariance](../../../string-theory.md#weyl-transformation).

The curvature coupling requires care. An infinitesimal [Weyl transformation](../../../string-theory.md#weyl-transformation) gives $\delta_\omega(\sqrt gR^{(2)})=-2\sqrt g\,\Delta_g\omega$. Integration by parts on the closed worldsheet therefore gives the [Weyl variation of a nonconstant dilaton coupling](../../../string-theory.md#weyl-variation-of-a-nonconstant-dilaton-coupling):

$$
\delta_\omega S_\Phi=-\frac1{2\pi}\int_\Sigma\sqrt g\,\Phi(X)\Delta_g\omega=-\frac1{2\pi}\int_\Sigma\sqrt g\,\omega\Delta_g\Phi(X).
$$

**A constant dilaton coupling is topological and Weyl invariant; a general varying dilaton coupling is not separately classically Weyl invariant.** Its classical variation participates in canceling the quantum [worldsheet Weyl anomaly](../../../string-theory.md#worldsheet-weyl-anomaly), producing the improved background equations below.

To relate these background couplings to the flat-space [bosonic string mass spectrum](../../../string-theory.md#bosonic-string-mass-spectrum), expand $G_{\mu\nu}=\eta_{\mu\nu}+h_{\mu\nu}(X)$ and express $h$ and $B$ as superpositions of plane waves. The perturbation of the action is a sum of [integrated string vertex operators](../../../string-theory.md#integrated-string-vertex-operator) of the form

$$
\int d^2z\,\epsilon_{\mu\nu}:\partial X^\mu\bar\partial X^\nu e^{ip\cdot X}:.
$$

This is the vertex of $\alpha_{-1}^\mu\widetilde\alpha_{-1}^\nu|p\rangle$ in the [massless first closed-string level](../../../string-theory.md#massless-first-closed-string-level). Its [conformal weights](../../../string-theory.md#conformal-weight) are $(1+\alpha'p^2/4,1+\alpha'p^2/4)$, so marginality gives $p^2=0$. The [primary operator](../../../string-theory.md#primary-field) conditions give transversality, and the [string-state gauge redundancy](../../../string-theory.md#string-state-gauge-redundancy) removes longitudinal components. The symmetric trace-free [polarization tensor](../../../string-theory.md#polarization-tensor) is the [graviton](../../../quantum-theory.md#graviton) and perturbs $G$; its antisymmetric part is the [Kalb–Ramond field](../../../string-theory.md#kalb-ramond-field) and perturbs $B$. The scalar physical polarization is the [dilaton](../../../string-theory.md#dilaton). At the level of background fields its vertex involves the metric trace and the curvature improvement, so an arbitrary off-shell metric trace should not simply be identified with the physical dilaton without this distinction.

The spacetime [gauge invariance](../../../relativistic-quantum-field.md#gauge-invariance) of the antisymmetric coupling is

$$
\boxed{B\longmapsto B+d\Lambda,\qquad \delta B_{\mu\nu}=\partial_\mu\Lambda_\nu-\partial_\nu\Lambda_\mu,\qquad H=dB.}
$$

Indeed its action is $S_B=i(2\pi\alpha')^{-1}\int_\Sigma X^*B$. Its variation is

$$
\delta S_B=\frac{i}{2\pi\alpha'}\int_\Sigma d(X^*\Lambda)=\frac{i}{2\pi\alpha'}\int_{\partial\Sigma}X^*\Lambda=0
$$

for a closed worldsheet, by [Stokes theorem](../../../calculus.md#stokes-theorem). In components this is the total derivative $\partial_a(\varepsilon^{ab}\Lambda_\nu(X)\partial_bX^\nu)$: the term containing $\partial_a\partial_bX^\nu$ vanishes by antisymmetry. Thus only the [Kalb-Ramond field strength](../../../string-theory.md#kalb-ramond-field-strength) $H$ can enter the local spacetime equations. With boundaries, a compensating boundary gauge-field transformation is needed.

Separate the [dilaton](../../../string-theory.md#dilaton) into a constant $\Phi_0$ and a varying part. The [Gauss-Bonnet theorem](../../../differential-geometry.md#gauss-bonnet-theorem) gives

$$
\frac1{4\pi}\int_\Sigma\sqrt g\,R^{(2)}=\chi(\Sigma)=2-2g
$$

for a connected closed orientable genus-$g$ worldsheet. Its Euclidean path-integral weight contains

$$
\boxed{e^{-S_{\Phi_0}}=e^{-(2-2g)\Phi_0}=g_s^{2g-2},\qquad g_s=e^{\Phi_0}.}
$$

Consequently the sum over worldsheet topologies is the [string genus expansion](../../../string-theory.md#string-genus-expansion) $\sum_{g\ge0}g_s^{2g-2}\mathcal A_g$, with each coefficient integrating over that genus's [worldsheet moduli](../../../string-theory.md#worldsheet-moduli). Each extra handle costs $g_s^2$, which is the loop-counting factor of [string perturbation theory](../../../string-theory.md#string-perturbation-theory). With the usual normalization of $n$ external closed-string vertices, the connected amplitude carries $g_s^{2g-2+n}$. This [dilaton Euler-characteristic weighting](../../../string-theory.md#dilaton-euler-characteristic-weighting) is distinct from the expansion in $\alpha'$ of a fixed-worldsheet [string nonlinear sigma model](../../../string-theory.md#string-nonlinear-sigma-model).

Finally quantize that two-dimensional theory. The background fields are its couplings. The [background field expansion of a string sigma model](../../../string-theory.md#background-field-expansion-of-a-string-sigma-model), $X=x+\xi$ in target-space [normal coordinates](../../../general-relativity.md#normal-coordinates), contains curvature vertices quadratic in the fluctuation $\xi$. Contracting their two fluctuation indices produces the [Ricci tensor](../../../general-relativity.md#ricci-tensor) multiplying $\partial x^\mu\bar\partial x^\nu$. Logarithmic short-distance contractions renormalize $G$, $B$, and $\Phi$, giving functional [sigma-model beta functions](../../../string-theory.md#sigma-model-beta-function). Gauge independence requires vanishing of the [worldsheet Weyl anomaly](../../../string-theory.md#worldsheet-weyl-anomaly), including the classical improvement from the varying [dilaton](../../../string-theory.md#dilaton), not merely an arbitrary choice of renormalization scale.

For clarity, in conventional leading-order normalization the improved coefficients are

$$
\begin{aligned}
\overline\beta^G_{\mu\nu}&=\alpha'\left(R_{\mu\nu}-\frac14H_{\mu\rho\sigma}H_\nu{}^{\rho\sigma}+2\nabla_\mu\nabla_\nu\Phi\right)+O(\alpha'^2),\\
\overline\beta^B_{\mu\nu}&=\alpha'\left(-\frac12\nabla^\rho H_{\rho\mu\nu}+\nabla^\rho\Phi\,H_{\rho\mu\nu}\right)+O(\alpha'^2),\\
\overline\beta^\Phi&=\frac{D-26}{6}+\alpha'\left((\nabla\Phi)^2-\frac12\nabla^2\Phi-\frac1{24}H^2\right)+O(\alpha'^2).
\end{aligned}
$$

Here $H^2=H_{\mu\nu\rho}H^{\mu\nu\rho}$. The constant term in the [dilaton](../../../string-theory.md#dilaton) coefficient is the matter-plus-ghost [central charge](../../../string-theory.md#central-charge) deficit. At $D=26$, setting these coefficients to zero gives the leading spacetime field equations

$$
\boxed{\begin{aligned}
R_{\mu\nu}-\frac14H_{\mu\rho\sigma}H_\nu{}^{\rho\sigma}+2\nabla_\mu\nabla_\nu\Phi&=0,\\
\nabla^\rho(e^{-2\Phi}H_{\rho\mu\nu})&=0,\\
R+4\nabla^2\Phi-4(\nabla\Phi)^2-\frac1{12}H^2&=0.
\end{aligned}}
$$

For the last equation, take the trace of the first, $R-H^2/4+2\nabla^2\Phi=0$, and combine it with $\overline\beta^\Phi=0$; this verifies the coefficients and signs. These are equivalently the equations from the leading [string-frame massless effective action](../../../string-theory.md#string-frame-massless-effective-action)

$$
S_{\rm eff}\propto\int d^{26}x\sqrt{-G}\,e^{-2\Phi}\left(R+4(\nabla\Phi)^2-\frac1{12}H^2\right).
$$

Higher worldsheet orders give higher-derivative $\alpha'$ corrections, whereas additional handles give string-loop corrections controlled by $g_s$. Thus quantum consistency of a two-dimensional [string nonlinear sigma model](../../../string-theory.md#string-nonlinear-sigma-model) determines the dynamics of its spacetime background fields. These leading coefficient conventions agree with [the primary string-theory lectures' background-field calculation](https://arxiv.org/html/0908.0333v3).

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2010](../../2010.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
