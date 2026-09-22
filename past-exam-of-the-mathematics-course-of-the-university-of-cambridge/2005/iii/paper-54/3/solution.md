<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The [Polyakov action](../../../../../polyakov-action.md) has independent [worldsheet metric](../../../../../worldsheet-metric.md) $\gamma_{ab}$ and embedding fields $X^\mu$. Varying the metric before imposing a gauge gives

$$
T_{ab}=\frac1{\alpha'}\left(\partial_aX\cdot\partial_bX-\frac12\gamma_{ab}\gamma^{cd}\partial_cX\cdot\partial_dX\right)=0.
$$

[Worldsheet diffeomorphisms](../../../../../worldsheet-diffeomorphism.md) and [Weyl transformations](../../../../../weyl-transformation.md) allow [conformal gauge](../../../../../conformal-gauge.md) $\gamma_{ab}=e^{2\omega}\eta_{ab}$ locally. The Weyl factor then cancels out of the classical action, leaving

$$
S_X=\frac1{4\pi\alpha'}\int d\tau\,d\sigma\,(\dot X^2-X'^2),\qquad (\partial_\tau^2-\partial_\sigma^2)X^\mu=0.
$$

These are free two-dimensional [scalar fields](../../../../../scalar-field.md), but the surviving metric equations require

$$
\boxed{(\dot X+X')^2=(\dot X-X')^2=0.}
$$

Equivalently, $\dot X^2+X'^2=0$ and $\dot X\cdot X'=0$. [Gauge fixing](../../../../../gauge-fixing.md) does not license dropping these [Virasoro constraints](../../../../../virasoro-constraint.md).

For an ordinary [open string](../../../../../open-string.md), the boundary conditions relate the two chiral sectors. With $\alpha_0^\mu=\sqrt{2\alpha'}k^\mu$, their independent Fourier generators are

$$
L_m=\frac12\sum_{r\in\mathbb Z}\alpha_{m-r}\cdot\alpha_r.
$$

The classical oscillator [Poisson brackets](../../../../../poisson-bracket.md) $\{\alpha_m^\mu,\alpha_n^\nu\}=-im\eta^{\mu\nu}\delta_{m+n,0}$ give the [classical Virasoro constraint algebra](../../../../../classical-virasoro-constraint-algebra.md)

$$
\{L_m,L_n\}=-i(m-n)L_{m+n}.
$$

Thus they are [first-class constraints](../../../../../first-class-constraint.md). In the [quantum theory](../../../../../quantum-theory-split.md) one applies [normal ordering](../../../../../normal-ordering.md) to the product and uses $[\alpha_m^\mu,\alpha_n^\nu]=m\eta^{\mu\nu}\delta_{m+n,0}$. The oscillator [commutator](../../../../../commutator.md) gives

$$
[L_m,\alpha_n^\mu]=-n\alpha_{m+n}^\mu,\qquad [L_m,L_n]=(m-n)L_{m+n}+\frac D{12}(m^3-m)\delta_{m+n,0}.
$$

For example, for $m>0$ the extra vacuum term is $(D/2)\sum_{r=1}^{m-1}r(m-r)=D(m^3-m)/12$. This exhibits the [Virasoro central extension](../../../../../virasoro-central-extension.md) rather than concealing it in a classical constraint equation. The matter [central charge](../../../../../central-charge.md) is $D$; the [worldsheet ghost fields](../../../../../worldsheet-ghost-field.md) have charge $-26$. Quantum consistency sets $D=26$ and the [string intercept](../../../../../normal-ordering-constant-of-a-string.md) to one.

In [old covariant string quantization](../../../../../old-covariant-string-quantization.md) the [physical-state Virasoro conditions for an open string](../../../../../physical-state-virasoro-conditions-for-an-open-string.md) are

$$
L_m|\Psi\rangle=0\quad(m>0),\qquad (L_0-1)|\Psi\rangle=0,\qquad L_0=\alpha'k^2+N.
$$

[Physical string states](../../../../../physical-string-state.md) are then identified modulo physical [null string states](../../../../../null-string-state.md). One does not impose both positive and negative generators as annihilation conditions: their central extension would obstruct that prescription. The resulting [null-state quotient of a string](../../../../../null-state-quotient-of-a-string.md) agrees with the transverse light-cone spectrum at nonzero [momentum](../../../../../momentum.md).

At $N=0$, the [oscillator vacuum](../../../../../oscillator-vacuum.md) $|k\rangle$ is a single [spacetime](../../../../../spacetime.md) [scalar field](../../../../../scalar-field.md) with $\alpha'M^2=-1$: the bosonic [tachyon](../../../../../tachyon.md). At $N=1$, write $|\Psi\rangle=\epsilon_\mu\alpha_{-1}^\mu|k\rangle$. The zero-mode equation gives $k^2=0$, and $L_1$ gives $k\cdot\epsilon=0$. The null descendant $L_{-1}|k\rangle=\sqrt{2\alpha'}k\cdot\alpha_{-1}|k\rangle$ identifies $\epsilon\sim\epsilon+\lambda k$. **This leaves 24 physical polarizations of a massless gauge vector.**

At $N=2$, use the [level-two open-string polarization decomposition](../../../../../level-two-open-string-polarization-decomposition.md)

$$
|\Psi\rangle=\left(\frac12h_{\mu\nu}\alpha_{-1}^\mu\alpha_{-1}^\nu+b_\mu\alpha_{-2}^\mu\right)|k\rangle,\qquad h_{\mu\nu}=h_{\nu\mu}.
$$

The mass is $M^2=1/\alpha'$. The oscillator [commutators](../../../../../commutator.md) give all the nontrivial positive-mode conditions:

$$
\sqrt{2\alpha'}\,k^\mu h_{\mu\nu}+2b_\nu=0,\qquad \frac12h^\mu{}_{\mu}+2\sqrt{2\alpha'}\,k\cdot b=0.
$$

Higher positive modes annihilate this level. To see the quotient explicitly, the 25 transverse-parameter null states $L_{-1}(\xi\cdot\alpha_{-1}|k\rangle)$, with $k\cdot\xi=0$, shift

$$
\Delta h_{\mu\nu}=\sqrt{2\alpha'}(k_\mu\xi_\nu+k_\nu\xi_\mu),\qquad \Delta b_\mu=\xi_\mu.
$$

The additional [level-two scalar Virasoro null state](../../../../../level-two-scalar-virasoro-null-state.md) $(L_{-2}+\tfrac32L_{-1}^2)|k\rangle$ shifts

$$
\Delta h_{\mu\nu}=\eta_{\mu\nu}+6\alpha'k_\mu k_\nu,\qquad \Delta b_\mu=\frac52\sqrt{2\alpha'}\,k_\mu.
$$

Substitution into the two physical equations verifies the null-state conditions; the second residual is $(D-26)/2$. Because $k$ is timelike, these null shifts span all components of $b$, so choose a representative with $b=0$. The physical conditions then say $k^\mu h_{\mu\nu}=0$ and $h^\mu{}_{\mu}=0$. In the [rest frame](../../../../../rest-frame.md) this is a [traceless second-rank tensor](../../../../../traceless-second-rank-tensor.md) in 25 spatial dimensions, with $25\cdot26/2-1=324$ polarizations. The light-cone basis independently gives $24$ states $\alpha_{-2}^i|k\rangle$ and $24\cdot25/2=300$ symmetric states $\alpha_{-1}^i\alpha_{-1}^j|k\rangle$. Hence

$$
\boxed{\alpha'M^2=-1,0,1:\qquad1\ \text{scalar},\quad24\ \text{vector polarizations},\quad324\ \text{massive spin-two polarizations}.}
$$

For the fermionic extension, an explicit convention prevents ambiguity in the signs. Keep [worldsheet](../../../../../worldsheet.md) signature $(-,+)$ and use

$$
\rho^0=\begin{pmatrix}0&-i\\i&0\end{pmatrix},\qquad \rho^1=\begin{pmatrix}0&i\\i&0\end{pmatrix},\qquad \{\rho^a,\rho^b\}=-2\eta^{ab}.
$$

Take $\psi=(\psi_1,\psi_2)^T$ and the constant parameter $\epsilon=(\epsilon_1,\epsilon_2)^T$ to be real Grassmann-odd Majorana components, with $\bar\psi=\psi^T\rho^0$. Put $\partial_\pm=\partial_\tau\pm\partial_\sigma$. Apart from the common factor $1/(4\pi\alpha')$, the combined Lagrangian is

$$
\mathcal L=\partial_+X\cdot\partial_-X+i\psi_1\cdot\partial_+\psi_1+i\psi_2\cdot\partial_-\psi_2.
$$

The rigid transformations can be written

$$
\delta X=\bar\epsilon\psi,\qquad \delta\psi=-i\rho^a\partial_aX\,\epsilon,
$$

or, in components,

$$
\delta X=i(\epsilon_2\psi_1-\epsilon_1\psi_2),\qquad \delta\psi_1=-\epsilon_2\partial_-X,\qquad \delta\psi_2=\epsilon_1\partial_+X.
$$

For the $\epsilon_2$ part, the bosonic variation is $i\epsilon_2(\partial_+\psi_1\cdot\partial_-X+\partial_+X\cdot\partial_-\psi_1)$, while the fermionic variation is $-i\epsilon_2\partial_-X\cdot\partial_+\psi_1+i\epsilon_2\psi_1\cdot\partial_+\partial_-X$. Anticommuting the constant parameter past the [fermion](../../../../../fermion.md) is essential in the second term. The first terms cancel. The other chiral component works in the same way, giving the [chiral proof of rigid worldsheet supersymmetry](../../../../../chiral-proof-of-rigid-worldsheet-supersymmetry.md)

$$
\boxed{\delta\mathcal L=i\epsilon_2\partial_-(\psi_1\cdot\partial_+X)-i\epsilon_1\partial_+(\psi_2\cdot\partial_-X).}
$$

Thus the action is invariant off shell up to a [boundary term](../../../../../boundary-term.md). The transformation is a genuine [supersymmetry](../../../../../supersymmetry-split.md): on $X$ its [commutator](../../../../../commutator.md) for parameters $\epsilon,\zeta$ is the translation

$$
[\delta_\epsilon,\delta_\zeta]X=2i(\epsilon_2\zeta_2\partial_-+\epsilon_1\zeta_1\partial_+)X.
$$

On $\psi$ the same translation follows using $\partial_+\psi_1=0$ and $\partial_-\psi_2=0$; the remaining cross terms are proportional to these [Dirac equations](../../../../../dirac-equation.md). This is [on-shell closure of rigid worldsheet supersymmetry](../../../../../on-shell-closure-of-rigid-worldsheet-supersymmetry.md). On a [surface with boundary](../../../../../surface-with-boundary.md), compatible endpoint conditions must make the boundary flux vanish. On a compact [worldsheet](../../../../../worldsheet.md), a constant parameter must preserve the [spin structure](../../../../../spin-structure.md); the local identity alone does not make a constant transformation compatible with every antiperiodic sector.

The [fermions](../../../../../fermion.md) contribute to the [worldsheet stress-energy tensor](../../../../../worldsheet-stress-energy-tensor.md) and produce a fermionic [superconformal current](../../../../../superconformal-current.md). In holomorphic normalization with $\psi^\mu(z)\psi^\nu(w)\sim\eta^{\mu\nu}/(z-w)$,

$$
T=-\frac1{\alpha'}:\partial X\cdot\partial X:-\frac12:\psi\cdot\partial\psi:,qquad G=i\sqrt{\frac2{\alpha'}}:\psi\cdot\partial X:.
$$

The free-field contractions give $G(z)G(w)\sim(2c/3)/(z-w)^3+2T(w)/(z-w)$ and [conformal weight](../../../../../conformal-weight.md) $3/2$ for $G$, where $c=D+D/2=3D/2$. Consequently the modes obey the [N=1 super-Virasoro algebra](../../../../../n-1-super-virasoro-algebra.md)

$$
\begin{aligned}
[L_m,L_n]&=(m-n)L_{m+n}+\frac c{12}(m^3-m)\delta_{m+n,0},\\
[L_m,G_r]&=\left(\frac m2-r\right)G_{m+r},\\
\{G_r,G_s\}&=2L_{r+s}+\frac c3\left(r^2-\frac14\right)\delta_{r+s,0}.
\end{aligned}
$$

Dropping the central terms gives the classical graded [constraint algebra](../../../../../constraint-algebra.md). [Integer](../../../../../integer.md) $r$ gives the [Ramond sector](../../../../../ramond-sector.md); half-integer $r$ gives the [Neveu–Schwarz sector](../../../../../neveu-schwarz-sector.md). In the displayed conformal-plane convention $G_0^2=L_0-c/24$ in the [Ramond sector](../../../../../ramond-sector.md). Shifting to the Ramond vacuum-normal-ordered [zero mode](../../../../../zero-mode.md) gives the usual [Ramond supercurrent zero-mode square](../../../../../ramond-supercurrent-zero-mode-square.md) $G_0^2=L_0^{(R)}$.

Rigid symmetry of matter already supplies these currents, but promoting their vanishing to new gauge constraints requires coupling to [worldsheet](../../../../../worldsheet.md) [supergravity](../../../../../supergravity.md) and varying its [worldsheet gravitino](../../../../../worldsheet-gravitino.md). In [superconformal gauge](../../../../../superconformal-gauge.md) one retains $T=G=0$. The fermionic current constraints and their physical-state conditions extend the bosonic Virasoro conditions. The ghost charges are $-26+11=-15$, so cancellation with $3D/2$ gives the [critical dimension of the RNS superstring](../../../../../critical-dimension-of-the-rns-superstring.md) $D=10$; the NS and Ramond intercepts are respectively $1/2$ and zero. This distinguishes the global [supersymmetry](../../../../../supersymmetry-split.md) established above from its locally gauged string completion.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 54](../../paper-54-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
