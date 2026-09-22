<h1 id="8/solution">Solution</h1>

↑ **Parent:** [8](../8.md)

The [loop group](../../../../../loop-group.md) here is $LU(1)=C^\infty(S^1,U(1))$, with pointwise multiplication. Although it is abelian, its nontrivial positive-energy quantum representations are projective: implementers can commute only up to a phase. A [positive energy representation of the loop group of U(1)](../../../../../positive-energy-representation-of-the-loop-group-of-u-1.md) has rotations $R_t$ whose [self-adjoint](../../../../../self-adjoint-operator.md) generator is bounded below and which implement $g(z)\mapsto g(e^{it}z)$ in the [projective unitary group](../../../../../projective-unitary-group.md). The fermionic construction gives both that phase and an explicit bosonic description.

Choose the one-particle [Hilbert space](../../../../../hilbert-space-split.md) $H=L^2(S^1)$ with modes $e_r(z)=z^r$, $r\in\mathbb Z$, and projection $P$ onto $r\geq0$. Use the [polarized fermionic Fock space](../../../../../polarized-fermionic-fock-space.md)

$$
\mathcal F_P=\Lambda(PH)\,\widehat\otimes\,\Lambda(\overline{(I-P)H}),
$$

where the [exterior powers](../../../../../exterior-power.md) are Hilbert-completed and the [tensor product](../../../../../tensor-product.md) is graded. Its vacuum fills all modes $r<0$ and leaves $r\geq0$ empty; excitations are particles in the empty modes and holes in the filled modes. The [fermionic annihilation operators](../../../../../fermionic-annihilation-operator.md) $c_r$ and [fermionic creation operators](../../../../../fermionic-creation-operator.md) $c_r^*$ satisfy the [canonical anticommutation relations](../../../../../canonical-anticommutation-relations.md)

$$
\{c_r,c_s^*\}=\delta_{rs}I,\qquad\{c_r,c_s\}=\{c_r^*,c_s^*\}=0,
\qquad c_r\Omega=0\ (r\geq0),\quad c_r^*\Omega=0\ (r<0).
$$

Finite particle-hole configurations form an [orthonormal basis](../../../../../orthonormal-basis.md). As in the finite-dimensional [exterior algebra](../../../../../exterior-algebra.md) construction, their [creation and annihilation operators](../../../../../creation-and-annihilation-operators.md) act irreducibly: an operator in the [commutant](../../../../../centralizer.md) sends the vacuum to a scalar vacuum, since the joint [kernel](../../../../../kernel-of-a-linear-map.md) of its vacuum annihilators is one-dimensional, and then acts by that scalar on the dense configuration basis.

[Segal's quantization criterion for fermions](../../../../../segal-quantization-criterion-for-fermions.md) says that a unitary one-particle operator $u$ has a unitary implementer $\Gamma(u)$ on this Fock space, satisfying $\Gamma(u)c^*(f)\Gamma(u)^*=c^*(uf)$, exactly when

$$
\boxed{[P,u]\text{ is Hilbert-Schmidt}.}
$$

Equivalently $P-uPu^*$ is [Hilbert-Schmidt](../../../../../hilbert-schmidt-operator.md). Implementers are unique up to phase, hence form a [projective unitary representation](../../../../../projective-unitary-representation.md) of the [restricted unitary group](../../../../../restricted-unitary-group.md). This is the fermionic, polarized criterion; it is not a condition that the entire operator $u-I$ be [Hilbert-Schmidt](../../../../../hilbert-schmidt-operator.md). The criterion and the corresponding continuity topology are stated in [Theorem III.2.1.1 of the fermionic construction of loop-group representations](https://arxiv.org/pdf/math/0409044). For the compact principal-angle part of a pair of polarizations, the threshold has a concrete interpretation. Its two-dimensional blocks are rotations through angles $\theta_j$; finitely many unmatched modes can be handled separately. Each angle $\theta_j$ rotates the vacuum into $\cos\theta_j$ times its original component plus $\sin\theta_j$ times a particle-hole pair. After discarding finitely many exceptional blocks, the successive [tensor products](../../../../../tensor-product.md) are Cauchy precisely when $\prod_j\cos\theta_j$ converges to a nonzero value, equivalently $\sum_j\sin^2\theta_j<\infty$. In this block model the sum is exactly half the squared [Hilbert-Schmidt](../../../../../hilbert-schmidt-operator.md) [norm](../../../../../norm.md) of the projection difference; finitely many unmatched modes account for a change of charge. Infinitely many unmatched modes already violate the criterion. This explains why infinitely many arbitrarily small mixings can fail to be implementable.

For $g(z)=\sum_n g_nz^n\in LU(1)$, multiplication $M_g$ is a unitary one-particle operator. Its [matrix](../../../../../matrix.md) entry from $e_s$ to $e_r$ is $g_{r-s}$. Therefore

$$
\|[P,M_g]\|_{\mathrm{HS}}^2
=\sum_{r,s}|\mathbf1_{r\geq0}-\mathbf1_{s\geq0}|^2|g_{r-s}|^2
=\sum_{n\in\mathbb Z}|n||g_n|^2.
$$

For a fixed difference $n$, exactly $|n|$ pairs cross the polarization boundary. Smoothness makes the sum finite, so [Segal's quantization criterion for fermions](../../../../../segal-quantization-criterion-for-fermions.md) constructs a continuous [projective unitary representation](../../../../../projective-unitary-representation.md) of every smooth loop. Smooth convergence gives operator-norm convergence of $M_g$ and [Hilbert-Schmidt](../../../../../hilbert-schmidt-operator.md) convergence of its [commutator](../../../../../commutator.md), which is sufficient for the strong projective continuity of the implementers.

[Normal ordering](../../../../../normal-ordering.md) fixes the charge and rotation energy. On the dense finite-configuration domain put

$$
E_{rs}=:c_r^*c_s:=c_r^*c_s-\delta_{rs}\mathbf1_{r<0}I,
\qquad Q=\sum_rE_{rr},\qquad L_0=\sum_r rE_{rr}.
$$

The sums are finite on each configuration. A particle at $r\geq0$ adds charge one and energy $r$; a hole at $r<0$ adds charge minus one and energy $-r$. Consequently $L_0$ is a nonnegative [self-adjoint](../../../../../self-adjoint-operator.md) diagonal operator with integer [spectrum](../../../../../spectrum-functional-analysis.md) and finite-dimensional [eigenspaces](../../../../../eigenspace.md). The unitaries $R_t=e^{itL_0}$ are strongly continuous, have period $2\pi$, and implement $e_r\mapsto e^{itr}e_r$. Conjugating multiplication by this one-particle rotation gives $M_{g(e^{it}\,\cdot)}$, so their Fock implementers rotate the loop representation projectively. This is an actual positive-energy [circle](../../../../../circle.md) action.

The scalar anomaly is visible in the [Heisenberg current algebra of a fermion on the circle](../../../../../heisenberg-current-algebra-of-a-fermion-on-the-circle.md). Define on finite-energy [vectors](../../../../../vector.md)

$$
J_n=\sum_{r\in\mathbb Z}E_{r,r+n},\qquad J_n^*=J_{-n},\qquad J_0=Q.
$$

For fixed $n$ the sum has only finitely many nonzero actions on any configuration. Direct use of the [canonical anticommutation relations](../../../../../canonical-anticommutation-relations.md) gives

$$
[E_{rs},E_{tu}]=\delta_{st}E_{ru}-\delta_{ur}E_{ts}
+\delta_{st}\delta_{ur}(\mathbf1_{r<0}-\mathbf1_{s<0})I.
$$

On summing, the two noncentral sums cancel. If $m=-n$ the central sum is $\sum_r(\mathbf1_{r<0}-\mathbf1_{r+n<0})=n$: for $n>0$ the terms are precisely $r=-n,\ldots,-1$. Thus

$$
\boxed{[J_n,J_m]=n\delta_{n+m,0}I,\qquad[L_0,J_n]=-nJ_n.}
$$

In particular $J_n\Omega=0$ for $n>0$. The coefficient one in the central term is the level of this basic representation.

Let $h(\theta)=\sum_n h_ne^{in\theta}$ be smooth and real. The normal-ordered infinitesimal implementer of multiplication by $h$ is

$$
A(h)=\sum_n h_nJ_{-n}.
$$

The sign of the current index matters: multiplication by $z^n$ raises the one-particle mode by $n$, so it corresponds to $J_{-n}$. It follows either directly from the bilinear [commutator](../../../../../commutator.md) or from the [fermionic currents on the circle](../../../../../fermionic-current-on-the-circle.md) that $[A(h),c_r^*]=\sum_n h_nc_{r+n}^*$. For trigonometric $h$ these are oscillator fields on the finite-energy domain; their [self-adjoint](../../../../../self-adjoint-operator.md) closures exponentiate to the implementers of $e^{ih}$. For general smooth $h$, their extensions are obtained by the oscillator-field construction below: $\sum_{n>0}n|h_n|^2<\infty$ guarantees the square-summable field coefficients, and Fourier truncation converges in the corresponding [Weyl relations](../../../../../weyl-relations.md) implementers. Thus no unjustified infinite operator product is required.

Set

$$
\omega(h,k)=\frac1{2\pi}\int_0^{2\pi}h'(\theta)k(\theta)\,d\theta
=i\sum_n nh_nk_{-n}.
$$

It is real and antisymmetric for real $h,k$. The [Heisenberg current algebra of a fermion on the circle](../../../../../heisenberg-current-algebra-of-a-fermion-on-the-circle.md) relations give $[A(h),A(k)]=i\omega(h,k)I$. The [Weyl relations](../../../../../weyl-relations.md), or the finite-mode Baker-Campbell-Hausdorff computation followed by the square-summable limit, yield

$$
e^{iA(h)}e^{iA(k)}=e^{-i\omega(h,k)/2}e^{iA(h+k)}.
$$

This is an explicit [two-cocycle](../../../../../two-cocycle.md) on the identity component of the [loop group](../../../../../loop-group.md). A different phase choice changes it by a [group coboundary](../../../../../group-coboundary.md), but its antisymmetric [commutator](../../../../../commutator.md) remains $e^{-i\omega(h,k)}$, and hence cannot be removed.

The winding components also matter. Every smooth loop is $z^we^{ih}$ with $w\in\mathbb Z$, real periodic $h$, and mean $h_0$ determined modulo $2\pi$. Let $S$ implement multiplication by $z$. It moves the filled boundary one place upwards, so it raises charge by one; phases of charge [ground states](../../../../../ground-state.md) can be chosen so that $S\Omega_q=\Omega_{q+1}$. Conjugating the [fermionic currents on the circle](../../../../../fermionic-current-on-the-circle.md) gives

$$
SQS^*=Q-I,\qquad SJ_nS^*=J_n\quad(n\ne0).
$$

Choose $U(w,h)=S^we^{iA(h)}$. Since $e^{iA(h)}S^v=S^ve^{i(A(h)+vh_0I)}$, one obtains the full [loop group two-cocycle for U(1)](../../../../../loop-group-two-cocycle-for-u-1.md)

$$
\boxed{U(w,h)U(v,k)=c((w,h),(v,k))U(w+v,h+k),\quad
c((w,h),(v,k))=\exp\bigl(ivh_0-i\omega(h,k)/2\bigr).}
$$

The exponent is bilinear in the additive winding-logarithm coordinates, so expansion immediately gives $c(a,b)c(a+b,d)=c(b,d)c(a,b+d)$. Replacing $h$ by $h+2\pi\ell$ changes $A(h)$ by $2\pi\ell Q$, whose exponential is identity since charges are integers; the scalar cocycle also stays unchanged since $v\in\mathbb Z$. Thus the expression is well-defined on loops, not just on chosen logarithms. It records both the [derivative](../../../../../derivative.md) anomaly and the [commutator](../../../../../commutator.md) of winding with constant loops.

For the [fermion-boson correspondence on the circle](../../../../../fermion-boson-correspondence-on-the-circle.md), decompose $\mathcal F_P=\bigoplus_{q\in\mathbb Z}\mathcal F_q$ into charge [eigenspaces](../../../../../eigenspace.md). The charge-$q$ [ground state](../../../../../ground-state.md) $\Omega_q$ fills all integer modes $r<q$. Its energy is

$$
L_0\Omega_q=\frac{q(q-1)}2\Omega_q.
$$

For $q>0$, sum the energies of the added modes $0,\ldots,q-1$; for $q<0$, sum the hole energies of the removed modes $q,\ldots,-1$. Every other charge-$q$ configuration is obtained by moving finitely many occupied levels upwards, so this is the lowest energy. Since $J_n$ preserves charge and lowers energy by $n>0$, $J_n\Omega_q=0$ for $n>0$.

Define [bosonic annihilation operators](../../../../../bosonic-annihilation-operator.md) $b_n=J_n/\sqrt n$ and $b_n^*=J_{-n}/\sqrt n$, $n>0$. They obey $[b_n,b_m^*]=\delta_{nm}I$. Their occupation [vectors](../../../../../vector.md)

$$
\prod_{n>0}\frac{(J_{-n})^{m_n}}{\sqrt{n^{m_n}m_n!}}\Omega_q,
\qquad m_n\in\mathbb N_0\text{ with finite support},
$$

are [orthonormal](../../../../../orthonormal-set.md) by commuting positive [fermionic currents on the circle](../../../../../fermionic-current-on-the-circle.md) through negative [fermionic currents on the circle](../../../../../fermionic-current-on-the-circle.md). Their energies are $q(q-1)/2+\sum_{n>0}nm_n$. It remains to prove that they span, rather than assume the boson correspondence. Count configurations by formal charge $u$ and energy $t$. Empty modes $r\geq0$ can contain one extra particle, while filled modes $-r$, $r\geq1$, can contain one hole. Therefore the fermionic character is

$$
\prod_{r\geq0}(1+ut^r)\prod_{r\geq1}(1+u^{-1}t^r).
$$

The charge form of the [Jacobi triple product](../../../../../jacobi-triple-product.md) proved in Question 4 identifies this with

$$
\sum_{q\in\mathbb Z}\frac{u^qt^{q(q-1)/2}}{\prod_{n\geq1}(1-t^n)}.
$$

The reciprocal product counts bosonic occupations, or [partitions of an integer](../../../../../partition-of-an-integer.md). For fixed charge and energy, the finite-dimensional fermion space has exactly as many basis configurations as the independent [fermionic current on the circle](../../../../../fermionic-current-on-the-circle.md) monomials already constructed. Hence those monomials exhaust every such space, proving their dense completeness. This establishes a unitary identification of every charge sector with a [bosonic Fock space](../../../../../bosonic-fock-space.md), and on that identification

$$
\boxed{L_0=\frac{Q(Q-I)}2+\sum_{n>0}n b_n^*b_n.}
$$

The usual half-integer fermion convention instead gives ground energy $q^2/2$ and requires the corresponding adjustment of rotations. Here integer modes were deliberately chosen to obtain a genuine [circle](../../../../../circle.md) action with integral nonnegative energies. The two [ground states](../../../../../ground-state.md) of energy zero, at charges zero and one, are therefore consistent, not a negative-energy defect.

This is also a constructive bosonic realization of the loop representation: the mean of $h$ acts by $h_0Q$, nonzero modes of $h$ act as the square-summable oscillator field $\sum_{n>0}\sqrt n(h_n b_n^*+\overline{h_n}b_n)$, and winding shifts the charge sectors. Taking $k$ tensor copies adds the [fermionic current on the circle](../../../../../fermionic-current-on-the-circle.md) central terms and gives level $k\in\mathbb N$. Positivity constrains their sign, since in a vacuum sector $\|J_{-n}\Omega\|^2=kn$ for $n>0$. The level-one construction, its explicit loop cocycle, and its complete bosonic occupation basis show how an abelian classical [loop group](../../../../../loop-group.md) acquires noncommuting quantum currents while retaining positive rotation energy.

## ↑ Ancestors (10)

1. [8](../8.md)
2. [Paper 10](../../paper-10-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
