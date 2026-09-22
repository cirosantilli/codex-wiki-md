<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Use the metric $g^{\mu\nu}=\operatorname{diag}(1,-1,-1,-1)$ and $\{\gamma^\mu,\gamma^\nu\}=2g^{\mu\nu}$. Transposing a product reverses its order but does not conjugate the factor $i$. Thus the [charge-conjugation matrix](../../../../../charge-conjugation-matrix.md) identity gives

$$
C\gamma_5^TC^{-1}=i(-\gamma^3)(-\gamma^2)(-\gamma^1)(-\gamma^0)=i\gamma^0\gamma^1\gamma^2\gamma^3=\boxed{\gamma_5},
$$

where reversing the four distinct [gamma matrices](../../../../../gamma-matrices.md) requires six exchanges. Similarly,

$$
C[\gamma^\mu,\gamma^\nu]^TC^{-1}=\gamma^\nu\gamma^\mu-\gamma^\mu\gamma^\nu=\boxed{-[\gamma^\mu,\gamma^\nu]}.
$$

To fix the transpose sign, work in the [Weyl representation of the gamma matrices](../../../../../weyl-representation-of-the-gamma-matrices.md):

$$
\gamma^0=\begin{pmatrix}0&I\\I&0\end{pmatrix},\qquad \gamma^j=\begin{pmatrix}0&\tau_j\\-\tau_j&0\end{pmatrix},\qquad C_0=i\gamma^2\gamma^0=\begin{pmatrix}\varepsilon&0\\0&-\varepsilon\end{pmatrix},\quad\varepsilon=i\tau_2.
$$

The Pauli identity checks $C_0\gamma^{\mu T}C_0^{-1}=-\gamma^\mu$ directly, and $\varepsilon^T=-\varepsilon$ gives $C_0^T=-C_0$, with $C_0^\dagger C_0=I$. Any other intertwiner differs from $C_0$ by a scalar: its ratio with $C_0$ commutes with all [gamma matrices](../../../../../gamma-matrices.md), whose products span the full four-by-four matrix algebra. A matrix commuting with all matrix units is scalar. Under a spinor basis change $S$, the intertwiner becomes $SC_0S^T$, whose transpose is still its negative. Therefore in every such four-component representation

$$
\boxed{C^T=-C.}
$$

This proves the [antisymmetry of the four-dimensional charge-conjugation matrix](../../../../../antisymmetry-of-the-four-dimensional-charge-conjugation-matrix.md), rather than leaving the sign undetermined by the general transpose argument.

Hermitian conjugating the charged [Dirac equation](../../../../../dirac-equation.md), using real $A_\mu,e,m$ and $\gamma^0\gamma^{\mu\dagger}\gamma^0=\gamma^\mu$, gives the [adjoint Dirac equation](../../../../../adjoint-dirac-equation.md)

$$
-i(\partial_\mu\bar\psi)\gamma^\mu+eA_\mu\bar\psi\gamma^\mu-m\bar\psi=0.
$$

Transpose it and multiply by $C$. Since $C\gamma^{\mu T}=-\gamma^\mu C$, the field $\psi^c=C\bar\psi^T$ obtained by [charge conjugation](../../../../../charge-conjugation.md) obeys

$$
\boxed{[i\gamma^\mu(\partial_\mu+ieA_\mu)-m]\psi^c=0.}
$$

Thus algebraic [charge conjugation](../../../../../charge-conjugation.md) reverses the electromagnetic coupling.

If $\gamma_5\psi=\eta\psi$, $\eta=\pm1$, Hermiticity of $\gamma_5$ and its anticommutation with $\gamma^0$ imply

$$
\bar\psi\gamma_5=\psi^\dagger\gamma^0\gamma_5=-\psi^\dagger\gamma_5\gamma^0=-\eta\bar\psi.
$$

Using the first transpose identity,

$$
\gamma_5\psi^c=C\gamma_5^T\bar\psi^T=C(\bar\psi\gamma_5)^T=-\eta\psi^c.
$$

Hence **$\boxed{\bar\psi\gamma_5=-\eta\bar\psi,\quad\gamma_5\psi^c=-\eta\psi^c}$**: [algebraic charge conjugation reverses chirality](../../../../../algebraic-charge-conjugation-reverses-chirality.md). This concerns conjugating the already projected spinor, not the distinct operation of keeping a chiral projector outside an operator conjugation.

For the [Grassmann variation of a chiral Majorana mass term](../../../../../grassmann-variation-of-a-chiral-majorana-mass-term.md), variations of odd fields must be moved past odd fields with a minus sign. If $A^T=-A$, componentwise reordering gives

$$
\delta(\psi^TA\psi)=\delta\psi^TA\psi+\psi^TA\delta\psi=2\delta\psi^TA\psi.
$$

Both $C$ and $C^{-1}$ are antisymmetric. Treating $\psi,\bar\psi$ independently, integrating the kinetic variation by parts, and placing varied Grassmann fields on the left gives

$$
\delta\mathcal L=\delta\bar\psi(i\gamma^\mu\partial_\mu\psi-m^*C\bar\psi^T)+\delta\psi^T(i\gamma^{\mu T}\partial_\mu\bar\psi^T+mC^{-1}\psi)+\partial_\mu(\cdots).
$$

The factors two from variation cancel the mass-term factors $1/2$. The first coefficient gives one equation; multiplying the second by $C$ gives the other:

$$
\boxed{i\gamma^\mu\partial_\mu\psi-m^*\psi^c=0,\qquad i\gamma^\mu\partial_\mu\psi^c-m\psi=0.}
$$

The variations can be restricted to their chiral subspaces: the two terms in each equation have the same opposite output [chirality](../../../../../chirality-physics.md), so no inactive component equation has been imposed.

Applying $i\not\partial$ to the first equation and substituting the second, using $(i\not\partial)^2=-\Box$, gives

$$
(\Box+|m|^2)\psi=0,\qquad\boxed{M=|m|.}
$$

A phase rotation removes the phase of $m$, and combining the chiral field with its conjugate then gives a [Majorana fermion](../../../../../majorana-spinor.md) of this mass, not two independent chiral species.

Let $\chi=\phi'^\dagger\Psi$ and $\bar\chi=\bar\Psi\phi'$. Question 1 shows they are gauge singlets, so both terms in $\mathcal L_G=G\chi^TC^{-1}\chi-G^*\bar\chi C\bar\chi^T$ preserve [electroweak gauge invariance](../../../../../electroweak-gauge-invariance.md). The original PDF has $C^{-1}$ in the first term; the TeX aid incorrectly replaces it by $G^{-1}$. At the [Higgs field](../../../../../higgs-field.md) vacuum,

$$
\phi'_0=\frac v{\sqrt2}\begin{pmatrix}1\\0\end{pmatrix},\qquad \chi\longrightarrow\frac v{\sqrt2}\nu_L,
$$

so

$$
\mathcal L_{G,0}=\frac12\left[Gv^2\nu_L^TC^{-1}\nu_L-G^*v^2\bar\nu_LC\bar\nu_L^T\right].
$$

Comparing with the just-derived chiral mass equations yields the [Majorana neutrino mass from the Weinberg operator](../../../../../majorana-neutrino-mass-from-the-weinberg-operator.md):

$$
\boxed{m_{\rm parameter}=Gv^2,\qquad m_\nu=|G|v^2.}
$$

For nonzero $G$ this generates a mass without introducing a [right-handed neutrino](../../../../../right-handed-neutrino.md). Under [lepton number](../../../../../lepton-number.md) rotation $\Psi\mapsto e^{i\alpha}\Psi$, the first operator acquires $e^{2i\alpha}$ and its conjugate acquires $e^{-2i\alpha}$. Thus **the interaction violates lepton number by $\boxed{\Delta L=2}$**. Each composite contains one scalar of mass dimension one and one fermion of dimension $3/2$, so the interaction is dimension five and $G$ has dimension $-1$. This is the [Weinberg operator](../../../../../weinberg-operator.md), an effective extension of the minimal renormalizable [Standard Model](../../../../../standard-model-split.md), consistent with the absence of bare quadratic masses in Question 1.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 45](../../paper-45-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
