<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

The [canonical anticommutation relations](../../../../../canonical-anticommutation-relations.md) realize the internal states as a [fermionic Fock space](../../../../../fermionic-fock-space.md) $\Lambda^\bullet\mathbb C^3$. Choosing a [Clifford vacuum](../../../../../clifford-vacuum.md) $|0\rangle$ annihilated by all $\psi_a$, the states are functions multiplying $|0\rangle$, $\psi_a^\dagger|0\rangle$, $\psi_a^\dagger\psi_b^\dagger|0\rangle$ with $a<b$, or $\psi_1^\dagger\psi_2^\dagger\psi_3^\dagger|0\rangle$. Thus the four [fermion-number sectors in supersymmetric quantum mechanics](../../../../../fermion-number-sectors-in-supersymmetric-quantum-mechanics.md) are

$$
\boxed{\mathcal H_n=L^2(\mathbb R^3)\otimes\Lambda^n\mathbb C^3,\quad n=0,1,2,3,}
$$

with internal dimensions $1,3,3,1$. The [fermion number operator](../../../../../fermion-number-operator.md) $N=\sum_a\psi_a^\dagger\psi_a$ has value $n$ on $\mathcal H_n$. The sectors $n=0,2$ have even [fermion parity](../../../../../fermion-parity.md), and $n=1,3$ have odd [fermion parity](../../../../../fermion-parity.md).

Write $q=\sum_a\psi_a^\dagger A_a$, so that the [supercharge](../../../../../supersymmetry-generator.md) is $Q=q+q^\dagger$. The [commutator](../../../../../commutator.md) $[A_a,A_b]$ is zero because the two [mixed partial derivatives](../../../../../mixed-partial-derivative.md) of $\chi$ agree. The [canonical anticommutation relations](../../../../../canonical-anticommutation-relations.md) then imply $q^2=(q^\dagger)^2=0$ and

$$
H=qq^\dagger+q^\dagger q,\qquad [H,N]=[H,q]=[H,q^\dagger]=[H,Q]=0.
$$

The [Hamiltonian operator](../../../../../hamiltonian-quantum-mechanics.md) preserves each sector, while $q$ raises and $q^\dagger$ lowers its degree by one. For a state in its operator domain, $\langle v,Hv\rangle=\|qv\|^2+\|q^\dagger v\|^2\geq0$, so the [spectrum](../../../../../spectrum-functional-analysis.md) is nonnegative. If $Hv=Ev$ with $E>0$, then $Qv/\sqrt E$ is a state of the same energy and opposite [fermion parity](../../../../../fermion-parity.md), and $Q(Qv/\sqrt E)=\sqrt E v$. This is an [odd involution pairing bosonic and fermionic states](../../../../../odd-involution-pairing-bosonic-and-fermionic-states.md) and proves equal even and odd multiplicities at every positive [eigenvalue](../../../../../eigenvalue.md).

There is also a more precise adjacent-sector pairing. On the positive-energy [eigenspace](../../../../../eigenspace.md),

$$
v=E^{-1}qq^\dagger v+E^{-1}q^\dagger qv.
$$

The two summands are [orthogonal](../../../../../orthogonal-vectors.md) since $q^2=(q^\dagger)^2=0$. A state $u$ in the image of $q^\dagger$ obeys $q^\dagger u=0$, $q^\dagger qu=Eu$, so $q/\sqrt E$ maps it to a normalized partner in the next sector, with inverse $q^\dagger/\sqrt E$. Thus positive-energy doublets lie in $\mathcal H_0\oplus\mathcal H_1$, $\mathcal H_1\oplus\mathcal H_2$, or $\mathcal H_2\oplus\mathcal H_3$. In particular, every positive-energy state of $\mathcal H_0$ has a partner in $\mathcal H_1$, and every one of $\mathcal H_3$ has a partner in $\mathcal H_2$; the remaining middle-sector states pair with each other. There is no requirement that all four individual sector spectra coincide. Zero-energy states satisfy $qv=q^\dagger v=Qv=0$ and can be unpaired. No confinement assumption was given: a continuous [spectrum](../../../../../spectrum-functional-analysis.md) is possible, with the same even/odd pairing on its positive spectral subspaces.

For real $\chi$, the [adjoint operator](../../../../../adjoint-operator.md) is $A_a^\dagger=-\partial_a-\partial_a\chi$. In $\mathcal H_0$, every $\psi_a^\dagger\psi_b$ vanishes; in the one-dimensional internal space of $\mathcal H_3$, it equals $\delta_{ab}$. The two scalar [Hamiltonian operators](../../../../../hamiltonian-quantum-mechanics.md) are consequently

$$
\boxed{H_0=\sum_a A_a^\dagger A_a=-\Delta+|\nabla\chi|^2+\Delta\chi,\qquad H_3=\sum_a A_aA_a^\dagger=-\Delta+|\nabla\chi|^2-\Delta\chi.}
$$

These are the extreme sectors of the [gradient superpotential Hamiltonian in supersymmetric quantum mechanics](../../../../../gradient-superpotential-hamiltonian-in-supersymmetric-quantum-mechanics.md).

For radial $\chi$ and a normalized state $v_0=f(r)|0\rangle$ with $E>0$, $q^\dagger v_0=0$ and $A_af=(x_a/r)(f'-\chi'f)$. The [radial superpartner in three-dimensional supersymmetric quantum mechanics](../../../../../radial-superpartner-in-three-dimensional-supersymmetric-quantum-mechanics.md) therefore has the simple form

$$
\boxed{v_1=\frac{f'(r)-\chi'(r)f(r)}{\sqrt E}\,\psi_r^\dagger|0\rangle,\qquad \psi_r^\dagger=\sum_a\frac{x_a}{r}\psi_a^\dagger.}
$$

It belongs to $\mathcal H_1$; $Hv_1=Ev_1$ follows from $[H,Q]=0$, and its [wavefunction normalization](../../../../../wavefunction-normalization.md) follows from $\|Qv_0\|^2=\langle v_0,Hv_0\rangle=E$. Also $Qv_1=\sqrt E v_0$. At the origin the formula is interpreted by regular extension; its degree-one components carry the radial [unit vector](../../../../../unit-vector.md) rather than being three independent radial scalars.

For a [zero mode in the fermion-vacuum sector](../../../../../zero-mode-in-the-fermion-vacuum-sector.md), the factorization of $H_0$ gives $0=\sum_a\|A_af\|^2$. Hence $\partial_a f=(\partial_a\chi)f$, or $\partial_a(e^{-\chi}f)=0$. The requested [wavefunction](../../../../../wave-function.md) is

$$
\boxed{f(r)=Ce^{\chi(r)},\qquad |C|^{-2}=4\pi\int_0^\infty r^2e^{2\chi(r)}\,dr.}
$$

A nonzero [normalizable wavefunction](../../../../../normalizable-wavefunction.md) exists only if this integral is finite. The positive sign in the exponential is fixed by the given convention $A_a=\partial_a-\partial_a\chi$.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 42](../../paper-42-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
