<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Adopt the phase convention $CP|K^0\rangle=-|\bar K^0\rangle$ and $CP|\bar K^0\rangle=-|K^0\rangle$. Changing both phases changes the convention for the mixing parameter, not physical predictions. The flavor contents are $K^0=d\bar s$ and $\bar K^0=s\bar d$. A pair of [charged weak currents](../../../../../charged-current.md) changes [strangeness](../../../../../strangeness.md) by two units through the following box contractions, with $u_i,u_j=u,c,t$ summed over.

<a id="1/image-charged-current-box-contractions-for-neutral-kaon-mixing-solid-arrows-carry-quark-number-and-wavy-lines-denote-w-bosons"></a>
![](../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-53-kaon-boxes.png)

**[Figure 1](#1/image-charged-current-box-contractions-for-neutral-kaon-mixing-solid-arrows-carry-quark-number-and-wavy-lines-denote-w-bosons). Charged-current box contractions for neutral-kaon mixing; solid arrows carry quark number and wavy lines denote W bosons**.

The drawing uses [unitary gauge](../../../../../unitary-gauge.md): the [W boson](../../../../../w-boson.md) [gauge-boson propagator](../../../../../gauge-boson-propagator.md) contains its longitudinal part. In a gauge of a [renormalizable quantum field theory](../../../../../renormalizable-quantum-field-theory.md), charged [Goldstone boson](../../../../../goldstone-boson.md) boxes must also be included to obtain the same gauge-independent result. The external lines represent the valence [quarks](../../../../../quark.md); the [meson](../../../../../meson.md) [matrix element](../../../../../matrix-element.md) also contains [strong interaction](../../../../../strong-interaction.md) binding effects.

Put $\lambda_i=V_{is}^*V_{id}$, $x_i=m_i^2/m_W^2$ and $P_L=(1-\gamma^5)/2$. The [charged weak box contribution to kaon mixing](../../../../../charged-weak-box-contribution-to-kaon-mixing.md) has the effective [four-fermion interaction](../../../../../four-fermion-interaction.md) structure

$$
H_{\Delta S=2}=C(\bar s\gamma_\mu P_Ld)(\bar s\gamma^\mu P_Ld)+\text{h.c.},\qquad
C\sim\frac{G_F^2m_W^2}{16\pi^2}\sum_{i,j}\lambda_i\lambda_j S(x_i,x_j).
$$

Here $G_F$ is the [Fermi constant](../../../../../fermi-constant.md), $V$ is the [CKM matrix](../../../../../cabibbo-kobayashi-maskawa-matrix.md), and $S$ is a dimensionless loop function from a [Feynman integral](../../../../../feynman-integral.md); the estimate suppresses convention-dependent numerical factors. Four [weak interaction](../../../../../weak-interaction.md) [Feynman vertices](../../../../../interaction-vertex.md) and a one-loop [Feynman integral](../../../../../feynman-integral.md) give the coupling and [loop order](../../../../../loop-order.md) suppression. [Unitarity](../../../../../unitary-operator.md) of the [CKM matrix](../../../../../cabibbo-kobayashi-maskawa-matrix.md) gives $\sum_i\lambda_i=0$, so the [GIM mechanism](../../../../../gim-mechanism.md) cancels the [mass](../../../../../mass.md)-independent part. With a negligible [up quark](../../../../../up-quark.md) [mass](../../../../../mass.md), the leading [charm quark](../../../../../charm-quark.md) term has $S(x_c,x_c)\sim x_c$. Define $f_K$ by $\langle0|\bar s\gamma_\mu\gamma^5d|K^0(p)\rangle=if_Kp_\mu$. Estimating the hadronic [matrix element](../../../../../matrix-element.md) by $f_K^2m_K B_K$, with the dimensionless [kaon bag parameter](../../../../../kaon-bag-parameter.md) $B_K$ of order unity, gives

$$
\boxed{|H'_{21}|_{\rm charm}\sim
\frac{G_F^2m_c^2}{16\pi^2}|V_{cs}^*V_{cd}|^2 f_K^2m_K B_K}.
$$

The hadronic normalization includes division by $2m_K$ when relativistically normalized states are converted to the [effective Hamiltonian for neutral-meson mixing](../../../../../effective-hamiltonian-for-neutral-meson-mixing.md). Since $|V_{cs}^*V_{cd}|\simeq\sin\theta_C\cos\theta_C$, the [Cabibbo suppression](../../../../../cabibbo-suppression.md) is explicit. Illustrative scales $G_F\sim10^{-5}\,\mathrm{GeV}^{-2}$, $m_c\sim1\,\mathrm{GeV}$, $f_K\sim0.1\,\mathrm{GeV}$ and $m_K\sim0.5\,\mathrm{GeV}$ give an order $10^{-16}$ to $10^{-15}\,\mathrm{GeV}$ estimate. The full sum includes [charm quark](../../../../../charm-quark.md)-[top quark](../../../../../top-quark.md) and [top quark](../../../../../top-quark.md)-[top quark](../../../../../top-quark.md) terms, important for [CP violation](../../../../../cp-violation.md); long-distance [strong interaction](../../../../../strong-interaction.md) contributions prevent this dimensional estimate from being a precision prediction. A [meson](../../../../../meson.md) [matrix element](../../../../../matrix-element.md) necessarily needs hadronic input in addition to electroweak parameters.

For the decaying [kaon](../../../../../kaon.md) system write $H'=M-i\Gamma/2$, where $M$ and $\Gamma$ are [Hermitian matrices](../../../../../hermitian-operator.md). The entries denoted $M_{ij}$ in the question are entries of this [effective Hamiltonian for neutral-meson mixing](../../../../../effective-hamiltonian-for-neutral-meson-mixing.md); they need not themselves form a [Hermitian matrix](../../../../../hermitian-operator.md). [CPT](../../../../../cpt-symmetry.md) invariance equates the diagonal [masses](../../../../../mass.md) and diagonal [decay widths](../../../../../decay-width.md), giving

$$
\boxed{H'_{11}=H'_{22}}.
$$

One can see why there is no [complex conjugation](../../../../../complex-conjugation.md) on the right as follows. In the flavor subspace let $J=\begin{pmatrix}0&1\\1&0\end{pmatrix}$ and represent the [antiunitary](../../../../../antiunitary-operator.md) [CPT](../../../../../cpt-symmetry.md) operation by $J$ followed by [complex conjugation](../../../../../complex-conjugation.md). [CPT](../../../../../cpt-symmetry.md) changes a projected forward propagator into its adjoint. Indeed, if $P$ projects onto the flavor subspace and $H_{\rm full}$ is the Hermitian microscopic generator, its invariance and the [antiunitary](../../../../../antiunitary-operator.md) reversal of $i$ give $\Theta P e^{-iH_{\rm full}t}P\Theta^{-1}=P e^{+iH_{\rm full}t}P=(P e^{-iH_{\rm full}t}P)^\dagger$. In the time-independent two-state approximation, the effective generator this means $J{H'}^*J={H'}^\dagger$, whose diagonal entries give $(H'_{22})^*=(H'_{11})^*$; the off-diagonal entries impose no further condition. Equivalently, apply [CPT](../../../../../cpt-symmetry.md) separately to the dispersive and absorptive [Hermitian matrices](../../../../../hermitian-operator.md). Treating the decaying [effective Hamiltonian for neutral-meson mixing](../../../../../effective-hamiltonian-for-neutral-meson-mixing.md) as a [Hermitian matrix](../../../../../hermitian-operator.md) would incorrectly discard the absorptive part.

In the chosen flavor phase convention [CP](../../../../../cp-symmetry.md) is represented by $-J$. Its invariance requires $JH'J=H'$. Thus it gives diagonal equality and additionally

$$
\boxed{H'_{12}=H'_{21}}.
$$

The normalized [CP eigenstates](../../../../../cp-eigenstate.md) are

$$
\boxed{|K_1^0\rangle=\frac{|K^0\rangle-|\bar K^0\rangle}{\sqrt2},\qquad
|K_2^0\rangle=\frac{|K^0\rangle+|\bar K^0\rangle}{\sqrt2}}.
$$

Applying [CP](../../../../../cp-symmetry.md) directly gives [eigenvalues](../../../../../eigenvalue.md) $+1$ and $-1$ respectively.

Now use [CPT](../../../../../cpt-symmetry.md) to put $H'=\begin{pmatrix}a&b\\c&a\end{pmatrix}$ and take correlated [square roots](../../../../../square-root.md) $\alpha=\sqrt b$, $\beta=\sqrt c$. Its [characteristic polynomial](../../../../../characteristic-polynomial.md) equation is $(a-\mu)^2-bc=0$, and direct multiplication shows

$$
H'\binom{\alpha}{-\beta}=(a-\alpha\beta)\binom{\alpha}{-\beta},\qquad
H'\binom{\alpha}{\beta}=(a+\alpha\beta)\binom{\alpha}{\beta}.
$$

Expressing these two [eigenvectors](../../../../../eigenvector.md) in the [CP eigenstate](../../../../../cp-eigenstate.md) basis gives, respectively, coefficients proportional to $(\alpha+\beta,\alpha-\beta)$ and $(\alpha-\beta,\alpha+\beta)$. Therefore the [kaon CP mixing parameter](../../../../../kaon-cp-mixing-parameter.md) is

$$
\epsilon=\frac{\alpha-\beta}{\alpha+\beta}
=\frac{\sqrt{M_{12}}-\sqrt{M_{21}}}{\sqrt{M_{12}}+\sqrt{M_{21}}},\qquad
\frac qp=\frac\beta\alpha=\frac{1-\epsilon}{1+\epsilon},
$$

and, because the [CP eigenstate](../../../../../cp-eigenstate.md) basis is [orthonormal](../../../../../orthonormal-set.md), the normalized states at production are

$$
\boxed{|K_S^0\rangle=\frac{|K_1^0\rangle+\epsilon|K_2^0\rangle}{\sqrt{1+|\epsilon|^2}},\qquad
|K_L^0\rangle=\frac{|K_2^0\rangle+\epsilon|K_1^0\rangle}{\sqrt{1+|\epsilon|^2}}}.
$$

The [kaon mixing square-root branch convention](../../../../../kaon-mixing-square-root-branch-convention.md) correlates the roots continuously with the limit of conserved [CP](../../../../../cp-symmetry.md) $b=c$, where $\alpha=\beta$ and $\epsilon=0$. Reversing one root interchanges the two [eigenstates](../../../../../eigenstate.md). The labels short and long are fixed by their [decay widths](../../../../../decay-width.md): their complex [eigenvalues](../../../../../eigenvalue.md) are $\mu_{S,L}=m_{S,L}-i\Gamma_{S,L}/2$, and subsequent evolution supplies $e^{-i\mu_{S,L}t}$. The displayed formula assumes nonzero mixing and $\alpha+\beta\ne0$, as in the physical [kaon](../../../../../kaon.md) system; degenerate or defective matrices require a separate limiting treatment.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 53](../../paper-53-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
