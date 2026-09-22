<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use a mostly-plus [Minkowski metric](../../../../../minkowski-metric.md) and [string tension](../../../../../string-tension.md) $T=(2\pi\alpha')^{-1}$. The [Polyakov action](../../../../../polyakov-action.md) is

$$
S_P=-\frac1{4\pi\alpha'}\int_\Sigma d^2\sigma\,\sqrt{-h}\,h^{ab}\partial_aX^\mu\partial_bX^\nu\eta_{\mu\nu}.
$$

Varying the auxiliary metric sets its [worldsheet stress-energy tensor](../../../../../worldsheet-stress-energy-tensor.md) to zero and makes $h$ conformal to the induced metric. Substitution gives the equivalent [Nambu–Goto action](../../../../../nambu-goto-action.md) $-T\int\sqrt{-\det(\partial_aX\cdot\partial_bX)}$. The [string coupling](../../../../../string-coupling.md) is separate from $T$. A constant [dilaton](../../../../../dilaton.md) contributes $S_\Phi=\Phi_0\chi(\Sigma)$ to the Euclidean [action](../../../../../action.md), by the [Gauss-Bonnet theorem](../../../../../gauss-bonnet-theorem.md), including its boundary term when necessary. With $g_s=e^{\Phi_0}$, a connected [worldsheet](../../../../../worldsheet.md) has weight $g_s^{-\chi}$. For an oriented closed surface of [genus](../../../../../genus-of-a-surface.md) $g$, this is **$g_s^{2g-2}$**; with $b$ boundaries it is $g_s^{2g+b-2}$. Normalizing each external [closed string](../../../../../closed-string.md) vertex with a factor $g_s$ gives $g_s^{2g+M-2}$ for $M$ external [closed strings](../../../../../closed-string.md). This is the [string genus expansion](../../../../../string-genus-expansion.md).

The local [gauge symmetries](../../../../../gauge-invariance.md) are [worldsheet diffeomorphisms](../../../../../worldsheet-diffeomorphism.md), under which $X$ is a [scalar field](../../../../../scalar-field.md), and [Weyl transformations](../../../../../weyl-transformation.md) $h_{ab}\mapsto e^{2\omega(\sigma)}h_{ab}$. Two coordinate functions and one Weyl function locally fix the three components of the two-dimensional metric, giving [conformal gauge](../../../../../conformal-gauge.md) $h_{ab}=e^{2\omega}\eta_{ab}$ and then $\omega=0$. Globally one instead chooses a fiducial metric and integrates over the [worldsheet moduli](../../../../../worldsheet-moduli.md); conformal Killing transformations can remain. Target-space Poincaré transformations are global symmetries, not additional local gauge freedoms.

For an infinitesimal coordinate change $v$, the trace-free metric variation is

$$
(P_1v)_{ab}=\nabla_av_b+\nabla_bv_a-h_{ab}\nabla_cv^c.
$$

After the Weyl trace is removed, gauge fixing produces the [Faddeev-Popov determinant](../../../../../faddeev-popov-determinant.md) of this operator. An anticommuting [vector](../../../../../vector.md) $c^a$ and symmetric traceless [tensor](../../../../../tensor.md) $b_{ab}$ represent that determinant through a [Grassmann Gaussian integral](../../../../../grassmann-gaussian-integral.md). The resulting [worldsheet ghost action](../../../../../worldsheet-ghost-action.md) is, up to field-normalization conventions,

$$
S_{bc}=\frac1{2\pi}\int d^2\sigma\sqrt{|\widehat h|}\,b^{ab}(P_1c)_{ab}.
$$

In complex coordinates this is a sum of chiral $b\bar\partial c$ and antichiral $\widetilde b\partial\widetilde c$ terms. The [worldsheet ghost fields](../../../../../worldsheet-ghost-field.md) have [conformal weights](../../../../../conformal-weight.md) two and minus one. Their [central charge](../../../../../central-charge.md) is $-26$, while the $d$ free embedding [bosons](../../../../../boson.md) contribute $d$. In the critical dimension the total anomaly cancels, consistently with the stated nilpotence of the [BRST charge](../../../../../brst-charge.md).

Physical states are [BRST cohomology](../../../../../brst-cohomology.md) classes at the appropriate [ghost number](../../../../../ghost-number.md): **$\ker Q/\operatorname{im}Q$**, with $Q|\phi\rangle=0$ and $|\phi\rangle\sim|\phi\rangle+Q|\chi\rangle$. Nilpotence ensures that an exact state is closed and that the equivalence is well-defined. For the usual [open string](../../../../../open-string.md) representatives the physical [ghost number](../../../../../ghost-number.md) is one. [BRST-exact](../../../../../brst-exact-operator.md) excitations describe gauge or null directions rather than additional physical particles.

To calculate the [ghost oscillator Virasoro generators](../../../../../ghost-oscillator-virasoro-generators.md), use the elementary fermionic identities

$$
[AB,C]=A\{B,C\}-\{A,C\}B
$$

when $A,B,C$ are odd. In the first commutator only $\{c_{-k},b_n\}=\delta_{k,n}$ survives, giving

$$
[L_m^{(b,c)},b_n]=\sum_k(m-k)b_{m+k}\delta_{k,n}=\boxed{(m-n)b_{m+n}}.
$$

In the second only $\{b_{m+k},c_n\}=\delta_{m+k+n,0}$ survives, giving

$$
[L_m^{(b,c)},c_n]=-\sum_k(m-k)\delta_{m+k+n,0}c_{-k}=\boxed{-(2m+n)c_{m+n}}.
$$

Normal-ordering constants commute with the [string oscillators](../../../../../string-oscillator.md) and do not change these results.

For the last request choose the [ghost oscillator vacuum](../../../../../ghost-oscillator-vacuum.md) $|\downarrow\rangle$ with $b_{m>0}|\downarrow\rangle=c_{m>0}|\downarrow\rangle=b_0|\downarrow\rangle=0$. The given conditions restrict a general state to $|\phi\rangle=|\Psi\rangle\otimes|\downarrow\rangle$ with no nonzero ghost excitations. Indeed, the positive modes annihilate both members of each creation–annihilation pair, and $b_0$ selects one member of the ghost zero-mode doublet. Use the [ghost Virasoro zero-mode convention](../../../../../ghost-virasoro-zero-mode-convention.md) compatible with the displayed explicit $-c_0$ term. Reordering the charge gives

$$
Q=\sum_m c_{-m}L_m^\alpha-\frac12\sum_{m,n}(m-n):c_{-m}c_{-n}b_{m+n}:-c_0.
$$

The normal-ordered cubic term annihilates $|\downarrow\rangle$. If both $c$ modes are creators, $m,n\geq0$, the $b_{m+n}$ mode is an annihilator, including $b_0$. If either $c$ is an annihilator, [normal ordering](../../../../../normal-ordering.md) puts an annihilator on the right. Consequently

$$
Q|\phi\rangle=c_0(L_0^\alpha-1)|\phi\rangle+\sum_{m>0}c_{-m}L_m^\alpha|\phi\rangle.
$$

These ghost states are independent. Acting with $b_0$ isolates $(L_0^\alpha-1)|\Psi\rangle$, while $b_m$, $m>0$, isolates $L_m^\alpha|\Psi\rangle$. Thus closure is equivalent to

$$
\boxed{(L_0^\alpha-1)|\Psi\rangle=0,\qquad L_m^\alpha|\Psi\rangle=0\quad(m>0).}
$$

Conversely these conditions make every term in $Q|\phi\rangle$ vanish. They are exactly the [physical-state Virasoro conditions for an open string](../../../../../physical-state-virasoro-conditions-for-an-open-string.md); the cohomology quotient additionally identifies physically equivalent representatives.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 50](../../paper-50-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
