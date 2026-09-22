<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Take $\partial_\pm=(\partial_\tau\pm\partial_\sigma)/2$ on the strip $0\leq\sigma\leq\pi$. Varying the Grassmann-odd [worldsheet Majorana fermions](../../../../../worldsheet-majorana-fermion.md) gives $\partial_-\psi_1=0$, $\partial_+\psi_2=0$ and, up to the orientation of the strip boundary, the surface term

$$
\delta I_{\rm bdry}=\frac{i}{2\pi}\int d\tau\,
\left(\psi_2\cdot\delta\psi_2-\psi_1\cdot\delta\psi_1\right)\Big|_0^\pi.
$$

At each endpoint it vanishes if $\psi_1=\eta\psi_2$ with $\eta=\pm1$, with the same relation on variations. A common sign can be absorbed by redefining one chiral field, so set $\eta_0=+1$. Since $\psi_1=f(\tau+\sigma)$ and $\psi_2=f(\tau-\sigma)$, the second endpoint imposes $f(u+2\pi)=\eta_\pi f(u)$. Equal endpoint signs give the periodic [Ramond sector](../../../../../ramond-sector.md), and opposite endpoint signs give the antiperiodic [Neveu–Schwarz sector](../../../../../neveu-schwarz-sector.md):

$$
\boxed{\psi_1(0)=\psi_2(0),\quad
\psi_1(\pi)=+\psi_2(\pi)\ (R),\quad
\psi_1(\pi)=-\psi_2(\pi)\ (NS).}
$$

These gluing choices preserve the Neumann-endpoint [worldsheet supersymmetry](../../../../../worldsheet-supersymmetry.md) conditions and give integer or half-integer [worldsheet Majorana fermion](../../../../../worldsheet-majorana-fermion.md) modes, respectively.

First fix a normalization issue in the original PDF. With its stated canonical [string oscillator](../../../../../string-oscillator.md) algebra, the standard [superconformal current](../../../../../superconformal-current.md) mode is

$$
G_r=\sum_{m\in\mathbb Z}:\alpha_m\cdot\psi_{r-m}:,
$$

without the printed factor $1/2$. To check the [Ramond supercurrent zero-mode square](../../../../../ramond-supercurrent-zero-mode-square.md) directly, pair positive and negative integer modes:

$$
G_0=\alpha_0\cdot\psi_0+\sum_{m>0}Q_m,
\qquad Q_m=\alpha_{-m}\cdot\psi_m+\alpha_m\cdot\psi_{-m}.
$$

The zero-mode Clifford relations give $(\alpha_0\cdot\psi_0)^2=\alpha_0^2/2$. Different $Q_m$ anticommute, and so do $Q_m$ with the zero-mode term. The two same-sign terms in $Q_m^2$ vanish by antisymmetry of the [fermions](../../../../../fermion.md) and symmetry of the bosonic product. The cross terms give

$$
Q_m^2=\alpha_{-m}\cdot\alpha_m+m\psi_{-m}\cdot\psi_m.
$$

The second term comes from commuting $\alpha_m$ through $\alpha_{-m}$, so the frequency factor $m$ is essential. Therefore

$$
G_0^2=\frac12\alpha_0^2+
\sum_{m>0}\left(\alpha_{-m}\cdot\alpha_m+m\psi_{-m}\cdot\psi_m\right)
=L_0^R,
\qquad\boxed{\{G_0,G_0\}=2L_0^R.}
$$

Here $L_0^R$ uses vacuum-annihilating Ramond [normal ordering](../../../../../normal-ordering.md); its [string intercept](../../../../../normal-ordering-constant-of-a-string.md) is zero. A plane-to-cylinder central shift must be included consistently if a different zero-mode convention is used.

**For the mode $F_r=G_r/2$ actually printed, the algebra instead gives $\{F_0,F_0\}=L_0^R/2$.** Already the oscillator-free term gives $\{F_0,F_0\}=\alpha_0^2/4$, whereas $2L_0^R=\alpha_0^2$. Thus the requested identity is not valid with both that prefactor and the supplied [string oscillator](../../../../../string-oscillator.md) algebra. Removing the prefactor gives the identity just derived. Renaming $L_0^R/4$ as $L_0$ would fix this isolated equality but would spoil the usual Virasoro normalization and the subsequent mass formula. We use the standard normalized modes $G_r$ in the remaining physical constraints; their vanishing is unaffected by a common nonzero rescaling.

The [RNS string](../../../../../spinning-string.md) physical-state conditions in the two sectors are

$$
\begin{array}{ll}
NS:&(L_0-\tfrac12)|\Phi\rangle=0,\quad
L_{n>0}|\Phi\rangle=0,\quad G_{r>0}|\Phi\rangle=0,
\quad r\in\mathbb Z+\tfrac12,\\
R:&L_0^R|\Phi\rangle=0,\quad
L_{n>0}|\Phi\rangle=0,\quad G_{n>0}|\Phi\rangle=0,
\quad G_0|\Phi\rangle=0.
\end{array}
$$

The last condition is the fermionic zero-mode constraint; its square implies the Ramond [mass-shell condition](../../../../../string-mass-shell-condition.md). Physical [null string states](../../../../../null-string-state.md) are quotiented. Matter [central charge](../../../../../central-charge.md) is $3d/2$, while the reparameterization [worldsheet ghost fields](../../../../../worldsheet-ghost-field.md) and [superconformal ghosts](../../../../../superconformal-ghost.md) contribute $-26+11=-15$. Thus $d=10$ is the [critical dimension of the RNS superstring](../../../../../critical-dimension-of-the-rns-superstring.md), with $a_{NS}=1/2$ and $a_R=0$.

To solve the constraints, choose $X^\pm=(X^0\pm X^9)/\sqrt2$, so $\eta_{+-}=-1$, and work on a patch with $\alpha_0^+=\sqrt{2\alpha'}p^+\ne0$. In [light-cone gauge in string theory](../../../../../light-cone-gauge-in-string-theory.md) fix all nonzero $\alpha_n^+$ and all $\psi_r^+$ to zero. For the [Ramond sector](../../../../../ramond-sector.md), the printed restriction to nonzero [fermion](../../../../../fermion.md) modes is not by itself complete: one must also reduce the longitudinal fermionic zero modes using the zero-mode supersymmetry constraint. The usual reduced light-cone description sets the remaining $\psi_0^+$ to zero as well and retains the transverse [Clifford algebra](../../../../../clifford-algebra.md). Covariantly this reduction is the [Dirac equation](../../../../../dirac-equation.md) on the ground-state [particle polarization](../../../../../particle-polarization.md); it is not an extra unconstrained canonical [string oscillator](../../../../../string-oscillator.md).

With this reduction the [string oscillator](../../../../../string-oscillator.md) generators have the form

$$
\begin{aligned}
L_n&=-\alpha_0^+\alpha_n^-+L_n^\perp,\\
L_n^\perp&=\frac12\sum_{m\in\mathbb Z}:\alpha_{n-m}^i\alpha_m^i:
+\frac12\sum_r\left(r-\frac n2\right):\psi_{n-r}^i\psi_r^i:,\\
G_r&=-\alpha_0^+\psi_r^-+G_r^\perp,
\qquad G_r^\perp=\sum_m\alpha_m^i\psi_{r-m}^i.
\end{aligned}
$$

Repeated $i$ runs over the eight transverse directions. The coefficient in $L_n^\perp$ comes from the [fermion](../../../../../fermion.md) [worldsheet stress tensor](../../../../../worldsheet-stress-energy-tensor.md) $-\psi\partial\psi/2$; for $n=0$, positive and negative $r$ combine to give the occupation energy $r\psi_{-r}\psi_r$. Thus the [light-cone super-Virasoro constraints](../../../../../light-cone-super-virasoro-constraints.md) are explicitly solved by

$$
\boxed{\alpha_n^-=\frac1{\alpha_0^+}\left[
\frac12\sum_m:\alpha_{n-m}^i\alpha_m^i:
+\frac12\sum_r\left(r-\frac n2\right):\psi_{n-r}^i\psi_r^i:
-a\delta_{n0}\right],\qquad
\psi_r^-=\frac1{\alpha_0^+}\sum_m\alpha_m^i\psi_{r-m}^i.}
$$

Here $a$ is $1/2$ in the [NS sector](../../../../../neveu-schwarz-sector.md) and zero in the [R sector](../../../../../ramond-sector.md). The zero-mode equation says $2p^+p^-=p_i^2+(N-a)/\alpha'$. All longitudinal excitations are consequently determined by transverse bilinears. The critical dimension and [string intercepts](../../../../../normal-ordering-constant-of-a-string.md) are necessary for the resulting quantum theory to preserve the target [Lorentz algebra](../../../../../lorentz-algebra.md).

The frequency-weighted [Neveu–Schwarz level operator](../../../../../neveu-schwarz-level-operator.md) is

$$
N_{NS}=\sum_{n=1}^\infty\alpha_{-n}^i\alpha_n^i
+\sum_{r=1/2,3/2,\ldots}r\psi_{-r}^i\psi_r^i.
$$

**The PDF's displayed number operator omits the [fermion](../../../../../fermion.md) frequency weights and the $r=1/2$ term.** With the stated anticommutators that cannot be a level operator: it would assign no level to the first fermionic excitation. The bosonic term already includes its frequency through $[\alpha_n,\alpha_{-n}]=n$, whereas the fermionic term must include its frequency explicitly.

One independent way to obtain the [string intercept](../../../../../normal-ordering-constant-of-a-string.md) is the transverse zero-point energy. Each periodic [boson](../../../../../boson.md) contributes $\tfrac12\sum_{n\ge1}n=-1/24$. Each antiperiodic real [fermion](../../../../../fermion.md) contributes $-\tfrac12\sum_{r\ge1/2}r=-1/48$, with the minus sign due to fermionic [normal ordering](../../../../../normal-ordering.md). For example a common exponential cutoff gives

$$
\sum_{n\ge1}n e^{-\varepsilon n}=\frac1{\varepsilon^2}-\frac1{12}+O(\varepsilon^2),
\qquad
\sum_{r\ge1/2}r e^{-\varepsilon r}=\frac1{\varepsilon^2}+\frac1{24}+O(\varepsilon^2).
$$

Subtracting the local divergent terms leaves $8(-1/24-1/48)=-1/2$, so **the NS [string intercept](../../../../../normal-ordering-constant-of-a-string.md) is $a=1/2$**. In the [Ramond sector](../../../../../ramond-sector.md) the integer [fermions](../../../../../fermion.md) instead contribute $+1/24$ per component and cancel the bosonic contribution, giving $a_R=0$.

The unprojected [NS sector](../../../../../neveu-schwarz-sector.md) [oscillator vacuum](../../../../../oscillator-vacuum.md) has $N=0$ and

$$
\boxed{M_{NS,0}^2=-\frac1{2\alpha'}=-1\quad(\alpha'=1/2).}
$$

It is a spacetime scalar [tachyon](../../../../../tachyon.md). The first excitation $\psi_{-1/2}^i|0;p\rangle$ has $N=1/2$ and is massless, with eight vector [particle polarizations](../../../../../particle-polarization.md). Covariantly its [particle polarization](../../../../../particle-polarization.md) obeys $p\cdot\epsilon=0$ modulo the longitudinal null [particle polarization](../../../../../particle-polarization.md), leaving the same eight degrees of freedom.

The [R sector](../../../../../ramond-sector.md) [oscillator vacuum](../../../../../oscillator-vacuum.md) is also massless, but it is degenerate because $\{\psi_0^\mu,\psi_0^\nu\}=\eta^{\mu\nu}$. The operators $\Gamma^\mu=\sqrt2\psi_0^\mu$ give the target [Clifford algebra](../../../../../clifford-algebra.md), and $G_0|u;p\rangle=0$ becomes $p_\mu\Gamma^\mu u=0$. At nonzero null momentum this [Dirac equation](../../../../../dirac-equation.md) leaves sixteen unprojected on-shell spinor states. Equivalently the eight transverse zero modes give the sixteen-dimensional spin representation $8_s\oplus8_c$ of $SO(8)$. Thus the Ramond ground state describes spacetime [fermions](../../../../../fermion.md), not a single scalar [oscillator vacuum](../../../../../oscillator-vacuum.md).

To define the [GSO projection](../../../../../gso-projection.md) explicitly, let $f_{NS}$ count excited NS [fermions](../../../../../fermion.md) and give its vacuum even parity. Then

$$
P_{NS}=\frac12\left(1-(-1)^{f_{NS}}\right).
$$

It retains odd [fermion](../../../../../fermion.md) number, removes the [tachyon](../../../../../tachyon.md), and retains the eight massless vector [particle polarizations](../../../../../particle-polarization.md). In the [Ramond sector](../../../../../ramond-sector.md) let $\Gamma_*$ be transverse [chirality](../../../../../chirality-physics.md) and $f_R$ count nonzero-mode [fermions](../../../../../fermion.md). Choose one consistent [chirality](../../../../../chirality-physics.md) sign $s=\pm1$ and use

$$
P_R=\frac12\left(1+s\Gamma_* (-1)^{f_R}\right).
$$

Each operator squares to itself. At the ground level $P_R$ retains one eight-dimensional spinor [chirality](../../../../../chirality-physics.md), so the retained spectrum has eight massless bosonic and eight massless fermionic states. The parity convention can instead assign the NS vacuum odd parity and write a plus projector; the retained states are identical.

Equality continues at every mass level. Let $q$ count $\alpha'M^2$, suppressing common momentum and endpoint-label factors, and set $D(q)=\prod_{n\ge1}(1-q^n)^8$. The projected [string oscillator](../../../../../string-oscillator.md) [generating functions](../../../../../generating-function.md) are

$$
Z_{NS}(q)=\frac{q^{-1/2}}{2D(q)}
\left[\prod_{r\ge1/2}(1+q^r)^8-\prod_{r\ge1/2}(1-q^r)^8\right],
\qquad
Z_R(q)=\frac8{D(q)}\prod_{n\ge1}(1+q^n)^8.
$$

The Ramond factor eight follows because either [chirality](../../../../../chirality-physics.md) projector selects eight ground states for every nonzero-oscillator parity. The [Jacobi abstruse identity](../../../../../jacobi-abstruse-identity.md) makes the bracket equal to $16q^{1/2}\prod_{n\ge1}(1+q^n)^8$, so

$$
\boxed{Z_{NS}(q)=Z_R(q).}
$$

This proves level-by-level equality of bosonic and fermionic multiplicities. The appropriate [spacetime supercharge from an RNS spin field](../../../../../spacetime-supercharge-from-an-rns-spin-field.md) relates the two sectors; the projection ensures that it acts within the retained state space. These sector and [chirality](../../../../../chirality-physics.md) conventions agree with [the primary superstring lecture notes](https://arxiv.org/pdf/hep-th/9709062). Equal total counts alone are not the definition of the projection; they follow from the stated parity selection and the [string oscillator](../../../../../string-oscillator.md) identity.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 54](../../paper-54-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
