<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Use $\bar\psi=\psi^\dagger\gamma^0$, the [Minkowski metric](../../../../../minkowski-metric.md) $(+---)$ and $\gamma^5=i\gamma^0\gamma^1\gamma^2\gamma^3$. Distinguish the numerical [charge-conjugation matrix](../../../../../charge-conjugation-matrix.md) $C$ from the unitary operator $\widehat C$ acting on fields. The [adjoint Dirac equation](../../../../../adjoint-dirac-equation.md) is $i(\partial_\mu\bar\psi)\gamma^\mu+m\bar\psi=0$. Transpose it and multiply by $C$; the identity $C\gamma^{\mu T}=-\gamma^\mu C$ gives

$$
iC\gamma^{\mu T}\partial_\mu\bar\psi^T+mC\bar\psi^T=0
\quad\Longrightarrow\quad
\boxed{(i\gamma^\mu\partial_\mu-m)\psi^c=0,\qquad\psi^c=C\bar\psi^T.}
$$

Thus the charge-conjugate field satisfies the same free [Dirac equation](../../../../../dirac-equation.md).

To compute its [Dirac adjoint](../../../../../dirac-adjoint.md), use $C^\dagger=C^{-1}$ and Hermitian $\gamma^0$ with $(\gamma^0)^2=1$. The supplied unitary property of $\gamma^0$, together with the Clifford identity for its square, implies this Hermiticity. Since $\gamma^{0T}C^{-1}=-C^{-1}\gamma^0$,

$$
\overline{\psi^c}=\psi^T(\gamma^0)^*C^{-1}\gamma^0
=\psi^T\gamma^{0T}C^{-1}\gamma^0=-\psi^TC^{-1}.
$$

Therefore [charge conjugation of the Dirac adjoint](../../../../../charge-conjugation-of-the-dirac-adjoint.md) gives

$$
\boxed{\widehat C\bar\psi(x)\widehat C^{-1}=-\eta_C^*\psi(x)^TC^{-1}.}
$$

The intrinsic phase obeys $|\eta_C|=1$. Antisymmetry of $C$ also gives $(\psi^c)^c=-C(C^{-1})^T\psi=\psi$.

[Charge conjugation](../../../../../charge-conjugation.md) exchanges electron and positron modes while preserving momentum and the spin label in a compatible spin basis. Write the [mode expansion of a Dirac field](../../../../../mode-expansion-of-a-dirac-field.md) as

$$
\psi(x)=\sum_s\int d\Pi_p\,[a(p,s)u(p,s)e^{-ip\cdot x}+b^\dagger(p,s)v(p,s)e^{ip\cdot x}].
$$

Its charge conjugate is

$$
\psi^c(x)=\sum_s\int d\Pi_p\,[b(p,s)C\bar v(p,s)^Te^{-ip\cdot x}+a^\dagger(p,s)C\bar u(p,s)^Te^{ip\cdot x}].
$$

Choose the [charge-conjugate particle and antiparticle spinors](../../../../../charge-conjugate-particle-and-antiparticle-spinors.md) so that

$$
\boxed{v(p,s)=C\bar u(p,s)^T,\qquad u(p,s)=C\bar v(p,s)^T.}
$$

This is legitimate: transposing $\bar u(\not p-m)=0$ shows $(\not p+m)C\bar u^T=0$, and the involution above supplies the inverse relation. Comparing the two independent frequency coefficients in $\widehat C\psi\widehat C^{-1}=\eta_C\psi^c$ then gives

$$
\boxed{\widehat Ca\widehat C^{-1}=\eta_Cb,\qquad
\widehat Cb\widehat C^{-1}=\eta_C^*a,\qquad
\widehat Ca^\dagger\widehat C^{-1}=\eta_C^*b^\dagger,\qquad
\widehat Cb^\dagger\widehat C^{-1}=\eta_Ca^\dagger.}
$$

Different conventional spinor phases can move the phases between these relations, but the exchange of particles and antiparticles is invariant.

For local [fermion bilinears](../../../../../fermion-bilinear.md), understand the products as [normal-ordered](../../../../../normal-ordering.md) or equivalently use a consistent renormalized composite-operator prescription. The transformed product is initially $-\psi^TC^{-1}\Gamma C\bar\psi^T$. Reordering the fermions gives a second minus sign, hence

$$
\widehat C:\bar\psi\Gamma\psi:\widehat C^{-1}
=:\bar\psi(C^{-1}\Gamma C)^T\psi:.
$$

For $\Gamma=\gamma^\mu$, the transposed matrix is $-\gamma^\mu$, so the [vector current](../../../../../vector-current.md) is C-odd:

$$
\boxed{\widehat Cj^\mu(x)\widehat C^{-1}=-j^\mu(x).}
$$

The [quantum electrodynamics](../../../../../quantum-electrodynamics.md) interaction $-ej_\mu A^\mu$ is C-invariant when the [photon](../../../../../photon.md) field is also odd, $\widehat CA^\mu\widehat C^{-1}=-A^\mu$. Its field strength is then odd and its quadratic kinetic term even.

For the [chirality matrix](../../../../../chirality-matrix.md), there is no complex conjugation of the numerical $i$ by this unitary field operation. Thus

$$
\begin{aligned}
C^{-1}\gamma^5C
&=i(-\gamma^{0T})(-\gamma^{1T})(-\gamma^{2T})(-\gamma^{3T})\\
&=i\gamma^{0T}\gamma^{1T}\gamma^{2T}\gamma^{3T}
=i\gamma^{3T}\gamma^{2T}\gamma^{1T}\gamma^{0T}=\gamma^{5T}.
\end{aligned}
$$

The reversal takes six swaps of mutually anticommuting [gamma matrices](../../../../../gamma-matrices.md), giving a positive sign. Therefore

$$
(C^{-1}\gamma^\mu\gamma^5C)^T=-\gamma^5\gamma^\mu=\gamma^\mu\gamma^5,
\qquad\boxed{\widehat Cj_5^\mu\widehat C^{-1}=+j_5^\mu.}
$$

The [axial current](../../../../../axial-current.md) is C-even. Hence a photon-like interaction containing both currents transforms as

$$
\widehat C:(j_\mu-j_{5\mu})A^\mu\longmapsto(j_\mu+j_{5\mu})A^\mu.
$$

It is **not C-invariant when the axial part is present**; C symmetry of ordinary electromagnetic vector coupling does not extend to this chiral combination.

For [parity symmetry in quantum field theory](../../../../../parity-symmetry-in-quantum-field-theory.md), taking the adjoint of the field transformation gives $\bar\psi(x)\mapsto\eta_P^*\bar\psi(x_P)\gamma^0$. The phases cancel in bilinears, and $\gamma^0\gamma^\mu\gamma^0=P^\mu{}_{\nu}\gamma^\nu$, with $P=\operatorname{diag}(1,-1,-1,-1)$. Since $\gamma^5$ anticommutes with $\gamma^0$,

$$
\boxed{j^\mu(x)\mapsto P^\mu{}_{\nu}j^\nu(x_P),\qquad
j_5^\mu(x)\mapsto-P^\mu{}_{\nu}j_5^\nu(x_P).}
$$

In components, the vector's time component is even and spatial components are odd; the axial time component is odd and its spatial components are even.

Combining the C and P transformations, both currents acquire the same overall minus sign:

$$
j^\mu(x)\xrightarrow{CP}-P^\mu{}_{\nu}j^\nu(x_P),\qquad
j_5^\mu(x)\xrightarrow{CP}-P^\mu{}_{\nu}j_5^\nu(x_P).
$$

Let the real vector transform as $V^\mu(x)\xrightarrow{CP}\xi P^\mu{}_{\nu}V^\nu(x_P)$, with $\xi=\pm1$. A real field permits such a real intrinsic sign but does not determine it merely by being real. The Lorentz contraction then gives the [CP invariance of a neutral chiral vector interaction](../../../../../cp-invariance-of-a-neutral-chiral-vector-interaction.md) criterion:

$$
\boxed{(j_\mu-j_{5\mu})V^\mu(x)\xrightarrow{CP}-\xi[(j_\mu-j_{5\mu})V^\mu](x_P).}
$$

It is invariant for $\xi=-1$. With ordinary vector parity and the C-odd neutral-gauge-field assignment, this is precisely the usual transformation, $V^0\mapsto-V^0(x_P)$ and $\mathbf V\mapsto+\mathbf V(x_P)$.

The diagonal [Z boson](../../../../../z-boson.md) couplings have the form $Z_\mu\bar f\gamma^\mu(g_V^f-g_A^f\gamma^5)f$ with real coefficients. The same calculation applies to any real vector and axial coefficients. Thus **the tree-level flavour-diagonal neutral-current Z interaction preserves CP although it violates C and P separately when both current structures occur**. This statement is about the neutral-current interaction, not a claim that the entire [Standard Model](../../../../../standard-model-split.md) preserves CP: complex charged-current [CKM matrix](../../../../../cabibbo-kobayashi-maskawa-matrix.md) phases provide [CP violation](../../../../../cp-violation.md).

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 52](../../paper-52-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
