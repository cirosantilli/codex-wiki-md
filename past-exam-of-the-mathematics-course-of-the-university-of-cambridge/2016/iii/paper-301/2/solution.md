<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

For this question use the [mostly-plus Dirac convention](../../../../../mostly-plus-dirac-convention.md): the [Minkowski metric](../../../../../minkowski-metric.md) is $\eta_{ab}=\operatorname{diag}(-1,1,1,1)$ and

$$
\boxed{\{\gamma^a,\gamma^b\}=-2\eta^{ab}I_4},\qquad
\boxed{(i\gamma^a\partial_a+m)\Psi=0}.
$$

This convention matches the printed plane-wave phase and final identity. It is related to the usual mostly-minus [Dirac equation](../../../../../dirac-equation.md) by reversing the metric and taking the negatives of the usual [gamma matrices](../../../../../gamma-matrices.md). In particular, the resulting [Dirac action](../../../../../dirac-action.md) and its [Dirac adjoint](../../../../../dirac-adjoint.md) describe the same physical massive field. The [Dirac gamma matrices](../../../../../gamma-matrices.md) are four complex $4\times4$ matrices representing the spacetime [Clifford algebra](../../../../../clifford-algebra.md) with quadratic form $-\eta$. The irreducible complex representation has dimension four. A convenient explicit choice is the negative of the standard [Dirac representation of the gamma matrices](../../../../../dirac-representation-of-the-gamma-matrices.md):

$$
\gamma^0=-\begin{pmatrix}I_2&0\\0&-I_2\end{pmatrix},\qquad
\gamma^i=-\begin{pmatrix}0&\sigma^i\\-\sigma^i&0\end{pmatrix},\qquad i=1,2,3,
$$

where $\sigma^i$ are the [Pauli matrices](../../../../../pauli-matrices.md). Their multiplication law verifies the displayed [anticommutator](../../../../../anticommutator.md).

In this representation the [gamma matrix adjoint and transpose identities](../../../../../gamma-matrix-adjoint-and-transpose-identities.md) are

$$
(\gamma^0)^\dagger=\gamma^0,\qquad(\gamma^i)^\dagger=-\gamma^i,\qquad
\boxed{(\gamma^a)^\dagger=\gamma^0\gamma^a\gamma^0},
$$

and

$$
(\gamma^0)^T=\gamma^0,\quad(\gamma^1)^T=-\gamma^1,\quad
(\gamma^2)^T=\gamma^2,\quad(\gamma^3)^T=-\gamma^3.
$$

The invariant way to express the latter pattern uses the [charge-conjugation matrix](../../../../../charge-conjugation-matrix.md):

$$
C=i\gamma^2\gamma^0,\qquad C^T=-C,\qquad C^\dagger=C^{-1},\qquad
\boxed{C^{-1}\gamma^aC=-(\gamma^a)^T}.
$$

Individual transpose signs depend on the basis. More generally, a [similarity transformation](../../../../../similarity-transformation.md) $\gamma'^a=M\gamma^aM^{-1}$ changes the [Hermitizing matrix](../../../../../hermitizing-matrix.md) to $H'=M^{-\dagger}\gamma^0M^{-1}$ and the [charge-conjugation matrix](../../../../../charge-conjugation-matrix.md) to $C'=MCM^T$. Then $\gamma'^{a\dagger}=H'\gamma'^aH'^{-1}$ and $C'^{-1}\gamma'^aC'=-\gamma'^{aT}$. Thus the simple formula with $\gamma'^0$ itself presumes a compatible Hermitian basis, rather than an arbitrary nonunitary [similarity transformation](../../../../../similarity-transformation.md).

Applying $(i\gamma^a\partial_a-m)$ to the [Dirac equation](../../../../../dirac-equation.md) gives $(\Box-m^2)\Psi=0$. Its [mass shell](../../../../../mass-shell.md) is $p^2=-m^2$, so the frequencies are $p^0=\pm\sqrt{\mathbf p^2+m^2}$. The [Dirac spinor](../../../../../dirac-spinor.md) transforms in the four-component [Spinor representation of the Lorentz group](../../../../../spinor-representation-of-the-lorentz-group.md). Under spatial rotations, the two upper and the two lower components each transform as a two-component spin-$1/2$ representation: the [spin angular momentum](../../../../../spin.md) matrices are $\operatorname{diag}(\sigma^i,\sigma^i)/2$. At rest the positive-energy equation selects the upper two components, giving two independent [spin](../../../../../spin.md) polarizations, and the negative-frequency equation selects the lower two.

In the quantum theory a mode expansion is

$$
\Psi(x)=\sum_{s=1}^2\int\frac{d^3p}{(2\pi)^3\sqrt{2E_{\mathbf p}}}
\left[b_s(\mathbf p)u_s(p)e^{ip\cdot x}+d_s^\dagger(\mathbf p)v_s(p)e^{-ip\cdot x}\right],\qquad p^0=E_{\mathbf p}>0.
$$

With the [mostly-plus Dirac convention](../../../../../mostly-plus-dirac-convention.md), $e^{ip\cdot x}=e^{-iEt+i\mathbf p\cdot\mathbf x}$ is positive frequency. The negative-frequency coefficient obeys $(\not p+m)v_s(p)=0$. The [fermionic annihilation operators](../../../../../fermionic-annihilation-operator.md) $b_s$ and $d_s$ satisfy the [canonical anticommutation relations](../../../../../canonical-anticommutation-relations.md), with their respective [fermionic creation operators](../../../../../fermionic-creation-operator.md). The $b_s^\dagger$ excitations are particles; the $d_s^\dagger$ excitations are [antiparticles](../../../../../antiparticle.md) with the same positive [energy](../../../../../energy.md), [mass](../../../../../mass.md) and spin-$1/2$ but opposite charge. After [normal ordering](../../../../../normal-ordering.md), the [Hamiltonian operator](../../../../../hamiltonian-quantum-mechanics.md) contains positive multiples of $b_s^\dagger b_s+d_s^\dagger d_s$. Reinterpreting the negative-frequency part as antiparticle creation supplies a spectrum bounded below rather than a physical tower of negative-energy particles.

For the printed $e^{ip\cdot x}$ wave, $\partial_a\Psi=ip_a\Psi$. Substitution gives

$$
(-\gamma^ap_a+m)u_s(p)=0,\qquad
\boxed{(\not p-m)u_s(p)=0},\qquad\not p=\gamma^ap_a.
$$

The spin label $s$ indexes the two states of a spin-$1/2$ particle, rather than varying the particle's total spin. For real on-shell $p$, [Hermitian conjugation](../../../../../hermitian-conjugation.md) and $\gamma^{a\dagger}=\gamma^0\gamma^a\gamma^0$ give

$$
u_s^\dagger(p)(\not p^\dagger-m)=0
\quad\Longrightarrow\quad
\boxed{\bar u_s(p)(\not p-m)=0},\qquad\bar u_s=u_s^\dagger\gamma^0.
$$

These are right and left null-vector equations for the same on-shell matrix.

To obtain the [Gordon identity](../../../../../gordon-identity.md), take both external [Dirac spinors](../../../../../dirac-spinor.md) to have the same real [mass](../../../../../mass.md) $m$. Their two equations imply

$$
\bar u_{s'}(p')\bigl[\gamma^a\not p+\not p'\gamma^a-2m\gamma^a\bigr]u_s(p)=0.
$$

Define $\gamma^{ab}=[\gamma^a,\gamma^b]/2$. The [Clifford algebra](../../../../../clifford-algebra.md) relation yields

$$
\gamma^a\gamma^b=-\eta^{ab}+\gamma^{ab},\qquad
\gamma^b\gamma^a=-\eta^{ab}-\gamma^{ab}.
$$

Therefore

$$
\gamma^a\not p+\not p'\gamma^a
=-(p^a+p'^a)-\gamma^{ab}(p'_b-p_b).
$$

Multiplying the previous null-vector equation by $-1$ proves the required formula exactly:

$$
\boxed{\bar u_{s'}(p')\gamma^{ab}(p'_b-p_b)u_s(p)
+\bar u_{s'}(p')(2m\gamma^a+p^a+p'^a)u_s(p)=0}.
$$

For $m\ne0$ it can be solved for the vector-current matrix element, separating a momentum term from the antisymmetric [Dirac spinor](../../../../../dirac-spinor.md) term. The identity before division also holds at $m=0$. **The signs depend jointly on the metric, Clifford relation, Dirac mass term and plane-wave phase.** In the mostly-minus convention of Questions 1 and 3, the printed phase instead gives $(\not p+m)u=0$; the corresponding identity uses $(p_b-p'_b)$ in the antisymmetric term. Mixing that convention with the formula proved here would produce an apparent sign error.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 301](../../paper-301-split.md)
3. [Iii](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
