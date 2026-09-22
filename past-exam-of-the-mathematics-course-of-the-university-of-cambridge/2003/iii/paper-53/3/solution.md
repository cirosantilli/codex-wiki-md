<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Here a supersymmetry-preserving combination means a real combination of Hermitian [Majorana spinor](../../../../../majorana-spinor.md) [supercharges](../../../../../supersymmetry-generator.md), in a positive-norm [unitary representation](../../../../../unitary-representation.md) of the ordinary [Super-Poincaré algebra](../../../../../super-poincare-algebra.md). This reality qualification is essential. Let $|\psi\rangle$ be normalized and in the charge domains, and define the real [symmetric matrix](../../../../../symmetric-matrix.md)

$$
M_{ab}=\frac12\langle\psi|\{Q_a,Q_b\}|\psi\rangle.
$$

For real $u$, the Hermitian operator $q_u=u^aQ_a$ satisfies

$$
\|q_u\psi\|^2=\langle\psi|q_u^2|\psi\rangle=u^TMu.
$$

Therefore $M$ is a [positive semidefinite matrix](../../../../../positive-semidefinite-matrix.md), and

$$
q_u\psi=0\quad\Longleftrightarrow\quad u\in\ker M.
$$

The reverse implication uses positivity: diagonalize $M$, so a zero quadratic form has zero component in every positive-eigenvalue direction. This converts the problem into [nullity of real N=1 supercharges](../../../../../nullity-of-real-n-1-supercharges.md), not just a condition on the determinant of an operator-valued expression.

In the equivalent [Weyl spinor](../../../../../weyl-spinor.md) form, $\{q_\alpha,q_\beta^\dagger\}=2\sigma^m_{\alpha\dot\beta}P_m$. After a fixed invertible change of real charge basis, $M$ is the realification of the Hermitian two-by-two matrix

$$
B=E I+\mathbf p\cdot\boldsymbol\sigma,\qquad
E=\langle P^0\rangle,\quad\mathbf p=\langle\mathbf P\rangle,
$$

up to the harmless spatial-sign convention. A complex [Hermitian matrix](../../../../../hermitian-operator.md) has the same [eigenvalues](../../../../../eigenvalue.md) in its realification, each repeated twice. The [Pauli matrix multiplication law](../../../../../pauli-matrix-multiplication-law.md) gives $(\mathbf p\cdot\boldsymbol\sigma)^2=|\mathbf p|^2I$, so these [eigenvalues](../../../../../eigenvalue.md) are $E+|\mathbf p|$ and $E-|\mathbf p|$, each twice. Positivity forces $E\geq|\mathbf p|$. If one nonzero real $u$ annihilates the state, $M$ has a kernel: either $E=|\mathbf p|>0$, with exactly two zero [eigenvalues](../../../../../eigenvalue.md), or $E=|\mathbf p|=0$, with four. Thus

$$
\boxed{\dim_{\mathbb R}\{u:(u\cdot Q)|\psi\rangle=0\}=2\ \text{or}\ 4.}
$$

For a momentum eigenstate these are the null-momentum and zero-momentum cases; the expectation-matrix proof also covers states not assumed to have definite momentum. There are no massive states preserving a real charge in this unextended algebra.

If “linear combination” instead allows arbitrary complex coefficients, the unrestricted claim is false. In a massive [fermionic Fock space](../../../../../fermionic-fock-space.md) with two lowering operators $a_1,a_2$ and a spin-half [Clifford vacuum](../../../../../clifford-vacuum.md) spectator, take

$$
|\psi\rangle=\frac{|00\rangle\otimes|\uparrow\rangle+
|01\rangle\otimes|\downarrow\rangle}{\sqrt2}.
$$

Then $a_1\psi=0$. The three vectors $a_2\psi$, $a_2^\dagger\psi$ and $a_1^\dagger\psi$ are linearly independent, by their occupation numbers and spectator [spin](../../../../../spin.md) labels. The complex annihilator is therefore only one-dimensional. Such a lowering operator is not a Hermitian generator of preserved real [supersymmetry](../../../../../supersymmetry-split.md). The boxed conclusion applies to the physical real-charge interpretation; it also assumes no [domain-wall charge in N=1 supersymmetry](../../../../../domain-wall-charge-in-n-1-supersymmetry.md).

## ↑ Ancestors (11)

1. [3](../3.md)
2. [Section A](../section-a.md)
3. [Paper 53](../../paper-53-split.md)
4. [Iii](../../split.md)
5. [2003](../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
