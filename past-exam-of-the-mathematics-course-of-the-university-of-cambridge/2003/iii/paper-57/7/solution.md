<h1 id="7/solution">Solution</h1>

↑ **Parent:** [7](../7.md)

[Geometric quantization](../../../../../geometric-quantization.md) constructs quantum state spaces from the geometry of a classical [symplectic manifold](../../../../../symplectic-manifold.md) $(P,\omega)$. Its first task is to represent classical [observables](../../../../../observable.md) and their [Poisson bracket](../../../../../poisson-bracket.md) by operators; its second is to reduce the excessive phase-space dependence of the resulting states. These are different steps, called [prequantization](../../../../../prequantization.md) and choice of a [polarization in geometric quantization](../../../../../polarization-in-geometric-quantization.md).

Use $\iota_{X_f}\omega=df$ and $\{f,g\}=\omega(X_f,X_g)$, so $[X_f,X_g]=-X_{\{f,g\}}$. A [prequantum line bundle](../../../../../prequantum-line-bundle.md) is a Hermitian complex [line bundle](../../../../../line-bundle.md) $L\to P$ with unitary [connection on a vector bundle](../../../../../connection-vector-bundle.md) of curvature

$$
F_\nabla=\frac{i}{\hbar}\omega.
$$

Its existence requires the integrality of all symplectic periods:

$$
\boxed{\frac1{2\pi\hbar}\int_\Sigma\omega\in\mathbb Z\quad\text{for every integral closed two-cycle }\Sigma.}
$$

One way to see the obstruction is to choose local primitives $\omega=-d\theta_i$ on contractible charts. The local connections are $d-i\theta_i/\hbar$. On overlaps the differences of $\theta_i$ are exact and determine unitary transition phases. On triple overlaps their exponentials obey the cocycle condition exactly when the periods have the stated integral values. Conversely that integral class is realized by a line bundle; adjusting a connection by a global one-form makes its curvature equal to the prescribed representative. Connections with this curvature can still differ by a flat connection, so integrality need not specify unique quantum data.

On smooth sections define the [Kostant-Souriau prequantum operator](../../../../../kostant-souriau-prequantum-operator.md)

$$
\widehat f=-i\hbar\nabla_{X_f}+f.
$$

Its defining algebraic property follows directly from the curvature commutator:

$$
[\nabla_{X_f},\nabla_{X_g}]=-\nabla_{X_{\{f,g\}}}+\frac{i}{\hbar}\{f,g\}.
$$

The multiplication terms contribute $-i\hbar(X_fg-X_gf)=2i\hbar\{f,g\}$, so

$$
\boxed{[\widehat f,\widehat g]=i\hbar\widehat{\{f,g\}},\qquad\widehat1=I.}
$$

The preliminary inner product integrates the Hermitian pairing against the [symplectic volume](../../../../../symplectic-volume.md) $\omega^n/n!$, where $\dim P=2n$. Hamiltonian flows preserve this measure, so real observables give formally symmetric operators on suitable compactly supported sections. Actual self-adjoint realizations and their domains require analysis, especially on a noncompact phase space.

The prequantum representation is generally reducible and depends on all $2n$ variables, whereas a configuration-space wave function should depend on $n$. A [polarization in geometric quantization](../../../../../polarization-in-geometric-quantization.md) is an involutive complex rank-$n$ distribution $\mathcal F\subset T_\mathbb CP$ that is isotropic for $\omega$. A real polarization is tangent to a [Lagrangian foliation](../../../../../lagrangian-foliation.md); a compatible complex polarization is supplied by a [Kähler manifold](../../../../../kahler-manifold.md). Polarized sections satisfy

$$
\nabla_Xs=0\quad(X\in\mathcal F).
$$

This condition is locally consistent because the connection curvature vanishes on pairs of polarization vectors, and involutivity closes the differential constraints. Globally, leaf holonomy can obstruct nonzero polarized sections. To construct the quantum [Hilbert space](../../../../../hilbert-space-split.md), one must also choose the appropriate quotient measure or density data and complete the polarized sections; it need not be a literal closed subspace of the original phase-space $L^2$ space.

For $P=T^*\mathbb R^n$, set $\theta=\sum_jp_jdq^j$, so $\omega=-d\theta$ and the line bundle is trivial with $\nabla=d-i\theta/\hbar$. The vertical polarization is spanned by $\partial_{p_j}$. Its equations say $\partial_{p_j}\psi=0$, hence $\psi=\psi(q)$. Before this restriction,

$$
\widehat f=-i\hbar X_f+f-\theta(X_f),\quad
\widehat q^j=i\hbar\partial_{p_j}+q^j,\quad
\widehat p_j=-i\hbar\partial_{q^j}.
$$

After restricting and using the configuration-space measure, the [Schrödinger representation](../../../../../schrodinger-representation-of-the-heisenberg-group.md) is

$$
\boxed{\mathcal H=L^2(\mathbb R^n,dq),\qquad
\widehat q^j\psi=q^j\psi,\quad \widehat p_j\psi=-i\hbar\partial_{q^j}\psi.}
$$

Their commutator is $i\hbar\delta^j{}_k$ on a common smooth test-function domain. Functions of $q$ act by multiplication. Observables affine in momenta have flows preserving this polarization and can act directly, with density terms when required for symmetry. An arbitrary observable does not: already $p^2/(2m)$ has a flow taking a vertical fiber to a slanted one. Thus merely restricting its prequantum operator does not produce the free Schrödinger Hamiltonian.

The [Blattner-Kostant-Sternberg pairing](../../../../../blattner-kostant-sternberg-pairing.md) compares different polarizations. One can transport a state by a Hamiltonian flow to its transported polarization, pair back with the chosen state space and differentiate to obtain additional operators when the pairing is well defined. The [metaplectic correction](../../../../../metaplectic-correction.md) tensors polarized sections with a suitable square root of the polarization's canonical bundle. Half-forms improve the invariant state pairing and contribute to operator transport; their global existence is additional data.

A closed real-polarization leaf illustrates the topological restriction. Since $\omega$ vanishes along a [Lagrangian leaf](../../../../../lagrangian-leaf.md), the restricted prequantum connection is flat. A nonzero parallel section exists around a closed loop only if its holonomy is trivial. In cotangent coordinates this is

$$
\exp\left(\frac i\hbar\oint p\,dq\right)=1,
\qquad \oint p\,dq=2\pi\hbar N.
$$

This is the [Bohr-Sommerfeld quantization condition](../../../../../bohr-sommerfeld-quantization.md) before the half-form correction. With the standard Maslov correction it becomes $\oint p\,dq=2\pi\hbar(N+\nu/4)$, where $\nu$ is the [Maslov index](../../../../../maslov-index.md). For an oscillator ellipse, the enclosed phase-space area is $2\pi E/\omega_0$ and the index is two; the corrected rule gives $E_N=\hbar\omega_0(N+1/2)$ for $N\geq0$, exhibiting the zero-point shift. Singular real polarizations can require distributional sections rather than ordinary smooth polarized sections.

The construction thus separates local operator algebra from global integrality, polarization and holonomy. It recovers familiar quantum representations while exposing their geometric choices. A polarization also limits which observables preserve the state space, and exact Poisson-to-commutator correspondence cannot in general be extended to every classical polynomial in an irreducible canonical quantization. Changes of polarization, operator domains, half-form existence and singular reductions are substantive issues, so geometric quantization is a framework with specified additional data rather than a unique automatic procedure for every classical system.

## ↑ Ancestors (10)

1. [7](../7.md)
2. [Paper 57](../../paper-57-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
