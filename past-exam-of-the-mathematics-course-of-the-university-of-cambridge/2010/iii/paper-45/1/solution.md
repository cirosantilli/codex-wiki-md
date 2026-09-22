<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Take $T_i=\tau_i/2$ and the [hypercharge](../../../../../hypercharge.md) generator $Y=I_2/2$ on the scalar. The two commuting factors of the [electroweak interaction](../../../../../electroweak-interaction.md) have independent invariant gauge kinetic terms and therefore independent coupling constants. Non-Abelian [gauge invariance](../../../../../gauge-invariance.md) requires the same $g$ for all three $SU(2)$ generators, while the $U(1)$ factor has its own $g'$; no symmetry of this product group requires $g=g'$.

A nonzero [Higgs doublet](../../../../../higgs-field.md) can be rotated by $SU(2)$ to

$$
\phi_0=\frac v{\sqrt2}\begin{pmatrix}0\\1\end{pmatrix},\qquad v>0.
$$

The [fundamental representation](../../../../../fundamental-representation.md) acts transitively on normalized complex doublets, so this fixes an internal direction without changing the vacuum norm. A general infinitesimal generator annihilates this vacuum only if

$$
(\alpha_iT_i+\beta Y)\phi_0=\frac v{2\sqrt2}\begin{pmatrix}\alpha_1-i\alpha_2\\-\alpha_3+\beta\end{pmatrix}=0.
$$

For real parameters this means $\alpha_1=\alpha_2=0$ and $\beta=\alpha_3$. Thus the connected [stabilizer subgroup](../../../../../stabilizer-subgroup.md) is one-dimensional:

$$
\boxed{SU(2)_T\times U(1)_Y\longrightarrow U(1)_Q,\qquad Q=T_3+Y=\begin{pmatrix}1&0\\0&0\end{pmatrix},\qquad Q\phi_0=0.}
$$

This proves the claimed [electroweak symmetry breaking](../../../../../electroweak-symmetry-breaking.md) and identifies the unbroken [electric charge](../../../../../electric-charge.md) generator.

The [gauge covariant derivative](../../../../../gauge-covariant-derivative.md) is

$$
\boxed{D_\mu\phi=(\partial_\mu-igA_\mu^iT_i-ig'B_\mu Y)\phi.}
$$

Writing the connection as $\mathcal A_\mu=gA_\mu^iT_i+g'B_\mu Y$, its local transformation is $\mathcal A'_\mu=U\mathcal A_\mu U^{-1}-i(\partial_\mu U)U^{-1}$. Direct substitution gives $D'_\mu(U\phi)=UD_\mu\phi$. Unitarity then proves

$$
(D'^\mu\phi')^\dagger D'_\mu\phi'=(D^\mu\phi)^\dagger U^\dagger U D_\mu\phi=(D^\mu\phi)^\dagger D_\mu\phi,
$$

so the scalar kinetic term is [gauge-invariant](../../../../../gauge-invariance.md).

At the constant vacuum the [gauge covariant derivative](../../../../../gauge-covariant-derivative.md) becomes

$$
D_\mu\phi_0=-\frac{iv}{2\sqrt2}\begin{pmatrix}g(A_\mu^1-iA_\mu^2)\\-gA_\mu^3+g'B_\mu\end{pmatrix}.
$$

Consequently

$$
\mathcal L_{\rm mass}=\frac{v^2}{8}\left[g^2(A_\mu^1A^{1\mu}+A_\mu^2A^{2\mu})+(gA_\mu^3-g'B_\mu)(gA^{3\mu}-g'B^\mu)\right]=\frac12\mathcal V_\mu^TM^2\mathcal V^\mu,
$$

where $\mathcal V=(A^1,A^2,A^3,B)^T$ and

$$
\boxed{M^2=\frac{v^2}{4}\begin{pmatrix}g^2&0&0&0\\0&g^2&0&0\\0&0&g^2&-gg'\\0&0&-gg'&g'^2\end{pmatrix}.}
$$

The factor $1/2$ is the canonical real-vector mass-term normalization; the displayed [electroweak doublet gauge-boson mass matrix](../../../../../electroweak-doublet-gauge-boson-mass-matrix.md) contains squared masses when the gauge kinetic terms are canonical.

The [electric charge](../../../../../electric-charge.md) generator acts on gauge fields through the [Adjoint representation](../../../../../adjoint-representation-of-a-lie-algebra.md), not through the scalar's two-by-two matrix. With $U=e^{i\alpha Q}$, the brackets $[T_3,T_1]=iT_2$ and $[T_3,T_2]=-iT_1$ give $\delta A^1=\alpha A^2$, $\delta A^2=-\alpha A^1$, and neutral $A^3,B$. Hence the [electromagnetic charge matrix of electroweak gauge fields](../../../../../electromagnetic-charge-matrix-of-electroweak-gauge-fields.md) in the requested basis is

$$
\boxed{Q_{\rm gauge}=\begin{pmatrix}0&-i&0&0\\i&0&0&0\\0&0&0&0\\0&0&0&0\end{pmatrix},\qquad\delta\mathcal V=i\alpha Q_{\rm gauge}\mathcal V.}
$$

Choose positive gauge couplings by the gauge-field sign convention. Set $s_W=g'/\sqrt{g^2+g'^2}$ and $c_W=g/\sqrt{g^2+g'^2}$. The [Weinberg angle](../../../../../weinberg-angle.md) rotation diagonalizes the neutral block, while $W^\pm=(A^1\mp iA^2)/\sqrt2$ obey $\delta W^\pm=\pm i\alpha W^\pm$. The physical [electroweak gauge bosons](../../../../../electroweak-gauge-boson.md) are

$$
\boxed{\begin{array}{c|c|c|c}
\text{boson}&\text{field}&\text{mass}&Q\\\hline
W^+&(A^1-iA^2)/\sqrt2&gv/2&+1\\
W^-&(A^1+iA^2)/\sqrt2&gv/2&-1\\
Z&c_WA^3-s_WB&v\sqrt{g^2+g'^2}/2&0\\
\gamma&s_WA^3+c_WB&0&0
\end{array}.}
$$

The charges are in units of $e=gs_W=g'c_W$. Thus the [tree-level electroweak gauge-boson masses](../../../../../tree-level-electroweak-gauge-boson-masses.md) satisfy $m_W=m_Zc_W$, and the unbroken [photon](../../../../../photon.md) is massless.

The electron and neutrino form the left-chiral lepton doublet, while the right-chiral electron is a weak singlet. In four-component notation use [chiral projectors](../../../../../chiral-projector.md) $P_{L,R}=(1\mp\gamma_5)/2$ and package

$$
\boxed{\Psi=\begin{pmatrix}\nu_L\\e_L\end{pmatrix}: (\mathbf2)_{-1/2},\qquad \psi=e_R:(\mathbf1)_{-1}.}
$$

Here each entry can be obtained by projecting a [Dirac field](../../../../../dirac-field.md); only the indicated [chirality](../../../../../chirality-physics.md) propagates. The [hypercharges](../../../../../hypercharge.md) follow from $Q=T_3+Y$: $(0,-1)=(1/2,-1/2)+Y_\Psi$ gives $Y_\Psi=-1/2$, and $T_3=0,Q=-1$ gives $Y_\psi=-1$. The minimal theory has no [right-handed neutrino](../../../../../right-handed-neutrino.md).

The gauge-invariant lepton kinetic Lagrangian is

$$
\boxed{\mathcal L_{\ell}=\bar\Psi i\gamma^\mu(\partial_\mu-igA_\mu^i\tau_i/2+ig'B_\mu/2)\Psi+\bar\psi i\gamma^\mu(\partial_\mu+ig'B_\mu)\psi.}
$$

If unprojected Dirac spinors are used as notation instead, insert $P_L$ in the first kinetic term and $P_R$ in the second. The inactive components are not additional physical degrees of freedom. Each term is invariant because the [gauge covariant derivative](../../../../../gauge-covariant-derivative.md) transforms in the same [gauge group representation](../../../../../gauge-group-representation.md) as its field.

No bare [Dirac mass term](../../../../../dirac-mass-term.md) is possible: $\bar\Psi\Psi$ and $\bar\psi\psi$ vanish by opposite adjoint projectors, while a cross term $\bar\Psi\psi$ has an uncontracted weak-doublet index and hypercharge $-1/2$. A neutrino [Dirac mass](../../../../../dirac-mass-term.md) would additionally require the absent right-handed field. A [Majorana mass term](../../../../../majorana-mass-term.md) pairs a chiral field with itself; $\Psi^TC^{-1}\Psi$ has hypercharge $-1$ and $\psi^TC^{-1}\psi$ has $-2$, so neither is invariant. These statements concern quadratic masses before [electroweak symmetry breaking](../../../../../electroweak-symmetry-breaking.md), not masses involving scalar insertions.

For the [Higgs conjugate doublet](../../../../../higgs-conjugate-doublet.md), put $\varepsilon=i\tau_2$. The given identity $\varepsilon\tau_i^*=-\tau_i\varepsilon$ exponentiates to $\varepsilon U^*=U\varepsilon$ for $U\in SU(2)$. Therefore

$$
\phi'=\varepsilon\phi^*\longmapsto e^{-i\beta/2}U\phi',\qquad\boxed{\phi':(\mathbf2)_{-1/2}.}
$$

In particular its weak isospin remains $T=1/2$ while its [hypercharge](../../../../../hypercharge.md) reverses. Since $\Psi\mapsto e^{-i\beta/2}U\Psi$, both $\phi'^\dagger\Psi$ and $\bar\Psi\phi'$ transform in the [trivial representation](../../../../../trivial-representation.md) of the full [gauge group](../../../../../gauge-group.md). They remain a Lorentz spinor and its adjoint; gauge singlet does not mean Lorentz scalar.

Finally the [Yukawa interaction](../../../../../yukawa-interaction.md)

$$
\mathcal L_Y=-y_e\bar\Psi\phi\psi-y_e^*\bar\psi\phi^\dagger\Psi
$$

is gauge invariant: the first term has total hypercharge $+1/2+1/2-1=0$, and its doublet indices are contracted. At the [Higgs field](../../../../../higgs-field.md) vacuum it becomes $-(y_ev/\sqrt2)\bar e_Le_R+\mathrm{h.c.}$. Rephase $e_R$ to make the coefficient real and positive and assemble $e=e_L+e_R$. Then

$$
\boxed{\mathcal L_{Y,0}=-m_e\bar ee,\qquad m_e=\frac{|y_e|v}{\sqrt2}.}
$$

This explicitly generates the [gauge-invariant electron Yukawa mass](../../../../../gauge-invariant-electron-yukawa-mass.md), without a bare mass in the unbroken theory.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 45](../../paper-45-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
