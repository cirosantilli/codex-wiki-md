<h1 id="7/solution">Solution</h1>

↑ **Parent:** [7](../7.md)

[Geometric quantization](../../../../../geometric-quantization.md) starts from a classical [symplectic manifold](../../../../../symplectic-manifold.md) $(P,\omega)$ and seeks a [Hilbert space](../../../../../hilbert-space-split.md) and quantum observables that reflect its geometry. It has two distinct stages: [prequantization](../../../../../prequantization.md), which represents the full [Poisson algebra](../../../../../poisson-algebra.md) on sections of a [line bundle](../../../../../line-bundle.md), and a choice of [polarization in geometric quantization](../../../../../polarization-in-geometric-quantization.md), which reduces the excessive phase-space dependence of those sections.

Use the conventions $\iota_{X_f}\omega=df$ and $\{f,g\}=\omega(X_f,X_g)$. A [prequantum line bundle](../../../../../prequantum-line-bundle.md) is a Hermitian [line bundle](../../../../../line-bundle.md) $L\to P$ with unitary connection of curvature

$$
F_\nabla=\frac{i}{\hbar}\omega.
$$

Existence requires

$$
\boxed{\frac1{2\pi\hbar}\int_\Sigma\omega\in\mathbb Z}
$$

for every closed integral two-cycle $\Sigma$, equivalently integrality of the symplectic [cohomology class](../../../../../cohomology-class.md). Necessity follows from the integral curvature periods of a unitary [line bundle](../../../../../line-bundle.md); conversely an integral class defines such a bundle, and one adjusts its connection to give the specified curvature. This is a restriction on the classical system, not a choice of local coordinates. For an exact cotangent [symplectic form](../../../../../symplectic-form.md) $\omega=-d\theta$, with $\theta=p_jdq_j$, the bundle can be trivial and a connection is $\nabla=d-i\theta/\hbar$. On a sphere with [symplectic area](../../../../../symplectic-area.md) $4\pi s$, the condition becomes $2s/\hbar\in\mathbb Z$. The sign of the curvature convention changes if one changes the Hamiltonian-vector-field convention or uses the dual bundle; the integrality condition is unaffected.

The [Kostant-Souriau prequantum operator](../../../../../kostant-souriau-prequantum-operator.md) for a real observable is

$$
\widehat f=-i\hbar\nabla_{X_f}+f.
$$

Its derivative part describes the classical [Hamiltonian flow](../../../../../hamiltonian-flow.md) and the multiplication term corrects the bracket. Indeed,

$$
[X_f,X_g]=-X_{\{f,g\}},\qquad
[\nabla_{X_f},\nabla_{X_g}]
=-\nabla_{X_{\{f,g\}}}+\frac{i}{\hbar}\{f,g\}.
$$

Since $X_f(g)=-\{f,g\}$, expanding the operator [commutator](../../../../../commutator.md) gives

$$
\boxed{[\widehat f,\widehat g]=i\hbar\,\widehat{\{f,g\}},\qquad \widehat1=I.}
$$

With the Hermitian bundle metric and [Liouville measure](../../../../../symplectic-volume-form.md), these operators are formally symmetric for real $f$ because [Hamiltonian flows](../../../../../hamiltonian-flow.md) preserve [symplectic volume](../../../../../symplectic-volume.md). On noncompact spaces, domains and self-adjointness still require attention; the algebraic identity initially holds on an appropriate common smooth domain.

[Prequantization](../../../../../prequantization.md) alone is too large. Sections depend on $2n$ phase-space variables, and the [canonical commutation relations](../../../../../canonical-commutation-relation.md) are represented reducibly. A polarization is an involutive maximal isotropic distribution $\mathcal F\subset T_{\mathbb C}P$ of complex rank $n$. Polarized sections satisfy

$$
\nabla_Ys=0\qquad(Y\in\mathcal F).
$$

The curvature vanishes on pairs of polarization vectors because $\omega|_{\mathcal F}=0$, and involutivity makes the equations locally compatible. A real polarization is tangent to a [Lagrangian foliation](../../../../../lagrangian-foliation.md). A complex polarization in a [Kähler manifold](../../../../../kahler-manifold.md) chooses one complex tangent type. With the curvature sign used here, choose the holomorphic tangent distribution, giving antiholomorphic wavefunctions. The conjugate line-bundle and sign convention gives the more usual holomorphic description.

For $T^*Q$, the vertical real polarization is spanned locally by $\partial_{p_j}$. Since the canonical [one-form](../../../../../one-form.md) has no vertical component, its polarized sections are functions of $q$ alone. In the above trivialization,

$$
\widehat f=-i\hbar X_f+f-\theta(X_f),\qquad
\boxed{\widehat q_j=q_j,\qquad \widehat p_j=-i\hbar\partial_{q_j}.}
$$

One does not simply integrate these states over every momentum to retain the prequantum [norm](../../../../../norm.md): they are constant along noncompact polarization leaves and that integral would diverge. The polarized inner product instead uses the configuration-space measure or an intrinsic [half-density](../../../../../half-density.md) description. This recovers the Schrödinger realization.

Only observables whose [Hamiltonian flows](../../../../../hamiltonian-flow.md) preserve $\mathcal F$ act directly on the polarized space. For example, the free-particle flow generated by $p^2/2$ sends vertical tangent vectors into directions with a configuration-space component, so its raw prequantum operator does not preserve the vertical polarization. To obtain the usual kinetic operator one needs an additional procedure, such as transporting the polarization and pairing back, rather than pretending every classical observable restricts automatically. The [Blattner-Kostant-Sternberg pairing](../../../../../blattner-kostant-sternberg-pairing.md) and related projection methods address this problem. The impossibility of quantizing all classical observables with every desired algebraic property is another reason to specify the admissible observable algebra.

A [metaplectic correction](../../../../../metaplectic-correction.md) tensors $L$ with a square root of the polarization's canonical [determinant](../../../../../determinant.md) bundle when such a square root exists. These half-forms make the pairing more intrinsic and supply corrections to operator transport. They account for familiar Maslov and zero-point shifts; their existence is an extra topological condition. For a flat phase plane, take $z=q+ip$ and replace $\theta=p\,dq$ by the gauge-equivalent $\theta_s=(p\,dq-q\,dp)/2$. Then

$$
\nabla=d+\frac{\bar z\,dz-z\,d\bar z}{4\hbar},\qquad
\nabla_{\partial_z}s=0
\quad\Longrightarrow\quad
s=e^{-|z|^2/(4\hbar)}f(\bar z).
$$

The antiholomorphic function therefore has Gaussian [norm](../../../../../norm.md), the complex-conjugate [Bargmann-Fock space](../../../../../bargmann-fock-space.md). This explicit calculation fixes which polarization matches our curvature sign. Choosing the opposite tangent type with the same sign would give growing Gaussian sections, not the desired [Hilbert space](../../../../../hilbert-space-split.md). On compact positive [Kähler](../../../../../kahler-manifold.md) examples, the corresponding holomorphic description (or its conjugate in these conventions) gives finite-dimensional state spaces.

Finding a suitable polarization is therefore a substantial part of the construction. A globally smooth real [Lagrangian foliation](../../../../../lagrangian-foliation.md) may fail to exist; for example a regular real polarization on $S^2$ would require a line field that its tangent topology forbids. Singular foliations and noncompact leaves complicate both states and inner products. Although the restricted prequantum connection is locally flat on a Lagrangian leaf, a global nonzero parallel section requires trivial [holonomy](../../../../../holonomy.md). In an integrable system this selects the [Bohr-Sommerfeld quantization](../../../../../bohr-sommerfeld-quantization.md) leaves; including the [half-form correction](../../../../../metaplectic-correction.md) gives the familiar action condition

$$
\oint\theta=2\pi\hbar\left(n+\frac{\mu_{\mathrm{Maslov}}}{4}\right)
$$

in the usual Maslov-index convention. Complex polarizations require compatible global complex geometry and positivity. Different choices can lead to quite different realizations, and a natural unitary comparison is not automatic. Thus **integral curvature provides [prequantization](../../../../../prequantization.md); polarization and its global compatibility determine the actual quantum state space**.

## ↑ Ancestors (10)

1. [7](../7.md)
2. [Paper 64](../../paper-64-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
