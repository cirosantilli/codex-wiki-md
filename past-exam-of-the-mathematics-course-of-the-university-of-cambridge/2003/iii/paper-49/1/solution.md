<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Assume $\lambda>0$ and $v>0$. The minima of the [scalar potential](../../../../../scalar-potential.md) have $|\phi|=v$. Choose the [vacuum expectation value](../../../../../vacuum-expectation-value.md) $\phi_0=ve_3$. Its [stabilizer subgroup](../../../../../stabilizer-subgroup.md) consists exactly of matrices $\operatorname{diag}(R_2,1)$ with $R_2\in O(2)$, so

$$
\boxed{O(3)\longrightarrow O(2).}
$$

The continuous [spontaneous symmetry breaking](../../../../../spontaneous-symmetry-breaking.md) is $SO(3)\to SO(2)$ and has two broken generators. For the full orthogonal group, the cross-product notation requires the [gauge connection](../../../../../connection-vector-bundle.md) to transform in the adjoint, as an axial vector: $R[A]_\times R^{-1}=[(\det R)RA]_\times$. The [scalar field](../../../../../scalar-field.md) transforms as the ordinary vector $R\phi$. This [axial transformation of orthogonal gauge connections](../../../../../axial-transformation-of-orthogonal-gauge-connections.md) makes the stated [covariant derivative](../../../../../covariant-derivative.md) transform correctly even for $\det R=-1$; assigning an ordinary-vector transformation to the connection would fail.

Near this nonzero vacuum, [unitary gauge](../../../../../unitary-gauge.md) removes the two angular [Goldstone bosons](../../../../../goldstone-boson.md) and gives $\phi=(0,0,v+h)$. Put

$$
W_\mu^\pm=\frac{A_\mu^1\mp iA_\mu^2}{\sqrt2},\qquad A_\mu=A_\mu^3,\qquad f_{\mu\nu}=\partial_\mu A_\nu-\partial_\nu A_\mu.
$$

These are the physical charged [gauge bosons](../../../../../gauge-boson.md), neutral massless [gauge boson](../../../../../gauge-boson.md), and radial [scalar field](../../../../../scalar-field.md). Directly substituting into the original [gauge field strengths](../../../../../gauge-field-strength.md) gives

$$
\mathcal F_{\mu\nu}^\pm=(\partial_\mu\mp ieA_\mu)W_\nu^\pm-(\partial_\nu\mp ieA_\nu)W_\mu^\pm,\qquad \mathcal F_{\mu\nu}^3=f_{\mu\nu}-ie(W_\mu^+W_\nu^--W_\nu^+W_\mu^-).
$$

The [scalar field](../../../../../scalar-field.md) [kinetic term](../../../../../kinetic-term.md) has no radial-vector cross term, because $\partial_\mu\phi$ and $\mathbf A_\mu\times\phi$ lie in perpendicular internal directions. The complete physical gauge-scalar [Lagrangian](../../../../../lagrangian.md) becomes

$$
\mathcal L=-\frac14\mathcal F^{3\mu\nu}\mathcal F^3_{\mu\nu}-\frac12\mathcal F^{+\mu\nu}\mathcal F^-_{\mu\nu}+\frac12(\partial h)^2+e^2(v+h)^2W_\mu^+W^{-\mu}-\frac12\lambda v^2h^2-\frac12\lambda vh^3-\frac18\lambda h^4.
$$

For each real vector the [mass term](../../../../../mass-term.md) is $m^2A_\mu A^\mu/2$, while for the complex pair it is $m_W^2W_\mu^+W^{-\mu}$. Hence the [adjoint triplet Higgs spectrum](../../../../../adjoint-triplet-higgs-spectrum.md) is

$$
\boxed{m_{W^+}=m_{W^-}=ev,\qquad m_A=0.}
$$

The radial scalar also has $m_h^2=\lambda v^2$ in the question's potential normalization. The two lost scalar modes supply the longitudinal polarizations of the massive vectors through the [Higgs mechanism](../../../../../higgs-mechanism.md).

For the [lepton](../../../../../lepton.md) [kinetic terms](../../../../../kinetic-term.md) let $P_L=(1-\gamma^5)/2$, $P_R=(1+\gamma^5)/2$, and denote the left neutral triplet entry by $n_L=c_\alpha\nu_L+s_\alpha N_L$. The missing singlet is the perpendicular combination

$$
\boxed{L^S=P_L(-\nu_e\sin\alpha+N\cos\alpha).}
$$

Its overall sign is immaterial. The real [orthogonal matrix](../../../../../orthogonal-matrix.md) $\left(\begin{smallmatrix}c_\alpha&s_\alpha\\-s_\alpha&c_\alpha\end{smallmatrix}\right)$ is orthogonal, so the sum of the kinetic terms of $n_L$ and $L^S$ is $\bar\nu_Li\not\partial\nu_L+\bar N_Li\not\partial N_L$ with no mixed terms. Combining with the right triplet gives ordinary [Dirac field](../../../../../dirac-field.md) [kinetic terms](../../../../../kinetic-term.md) for $E^+,N,e$, and only a left-handed [kinetic term](../../../../../kinetic-term.md) for the massless [neutrino](../../../../../neutrino.md). This is [orthogonal completion of mixed neutral lepton kinetic terms](../../../../../orthogonal-completion-of-mixed-neutral-lepton-kinetic-terms.md). The heavy charged field is $E^+$, as printed in the PDF, not the TeX's $N^+$.

To compute the charge commutator, the [canonical anticommutation relations](../../../../../canonical-anticommutation-relations.md) imply

$$
[\psi_i^\dagger(\mathbf x)\psi_j(\mathbf x),\psi_k^\dagger(\mathbf y)\psi_l(\mathbf y)]=\delta^3(\mathbf x-\mathbf y)(\delta_{jk}\psi_i^\dagger\psi_l-\delta_{il}\psi_k^\dagger\psi_j).
$$

The quartic terms cancel on reordering the fermions. Thus well-defined normal-ordered integrated bilinears obey [fermionic bilinear charge algebra](../../../../../fermionic-bilinear-charge-algebra.md), $[Q_C,Q_D]=Q_{[C,D]}$. Left/right mixed [commutators](../../../../../commutator.md) vanish since $P_LP_R=0$.

In either triplet, write

$$
K=\begin{pmatrix}0&1&0\\0&0&1\\0&0&0\end{pmatrix},\qquad [K,K^\dagger]=\operatorname{diag}(1,0,-1).
$$

The displayed current has a factor two relative to the projected bilinears, since $1\mp\gamma^5=2P_{L,R}$. Consequently its charges are $T^+=2(Q_K^L+Q_K^R)$ and $T^-=(T^+)^\dagger$. The neutral combinations have canonical anticommutators because $c_\alpha^2+s_\alpha^2=1$. Applying the matrix commutator gives

$$
[T^+,T^-]=4\int d^3x:(E^{+\dagger}E^+-e^\dagger e):=\boxed{\frac4eQ_\ell},
$$

where $Q_\ell=e\int:(E^{+\dagger}E^+-e^\dagger e):$ is the electromagnetic charge in the lepton sector. The neutrino, heavy neutral lepton and singlet contribute zero. This establishes [triplet charged-current closure on electromagnetic charge](../../../../../triplet-charged-current-closure-on-electromagnetic-charge.md), with the requested proportionality independent of normalization choices for the weak [Noether charges](../../../../../noether-charge.md). The PDF correctly writes $J^-=(J^+)^\dagger$; the TeX repeats $J^+$ incorrectly. Equal-time algebra does not require conservation of the separate fermionic weak currents after symmetry breaking. For full gauge-theory charges, the corresponding charged-boson contributions must also be included.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 49](../../paper-49-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
