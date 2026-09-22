<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Choose the [extended supersymmetry](../../../../../extended-supersymmetry.md) normalization

$$
\{Q^A_\alpha,\bar Q_{\dot\beta B}\}=2\sigma^\mu_{\alpha\dot\beta}P_\mu\delta^A{}_B,\qquad
\{Q^A_\alpha,Q^B_\beta\}=\epsilon_{\alpha\beta}Z^{AB},\qquad \epsilon_{12}=1.
$$

The [central charge in supersymmetry](../../../../../central-charge-in-supersymmetry.md) is antisymmetric in $A,B$, because the full [anticommutator](../../../../../anticommutator.md) is symmetric and $\epsilon_{\alpha\beta}$ is antisymmetric. In a massive [one-particle state](../../../../../one-particle-state.md) rest frame, $P_\mu=(M,0,0,0)$, and the first [anticommutator](../../../../../anticommutator.md) becomes $2M\delta_{\alpha\beta}\delta^A{}_B$.

A [unitary skew-diagonalization of an antisymmetric matrix](../../../../../unitary-skew-diagonalization-of-an-antisymmetric-matrix.md) puts $Z$ into blocks $\begin{pmatrix}0&z_r\\-z_r&0\end{pmatrix}$, with a remaining zero direction if $\mathcal N$ is odd. For one block write $z=|z|e^{i\varphi}$, and label its two supersymmetries $1,2$. The combinations

$$
A_\pm=\frac{Q^1_1\pm e^{i\varphi}(Q^2_2)^\dagger}{\sqrt2},\qquad
B_\pm=\frac{Q^1_2\mp e^{i\varphi}(Q^2_1)^\dagger}{\sqrt2}
$$

have

$$
\{A_\pm,A_\pm^\dagger\}=\{B_\pm,B_\pm^\dagger\}=2M\pm|z|.
$$

For example the mixed contribution to the first expression is $\pm(e^{-i\varphi}z+e^{i\varphi}\bar z)/2=\pm|z|$. This is the phase-aligned version of taking a [supercharge](../../../../../supersymmetry-generator.md) minus a unitary combination of its adjoints, as suggested by the hint.

For every operator $X$ and normalized state $|v\rangle$,

$$
\langle v|\{X,X^\dagger\}|v\rangle=\|Xv\|^2+\|X^\dagger v\|^2\ge0.
$$

Applying this to $A_-,B_-$ in every block proves **the BPS bound**

$$
\boxed{M\ge\frac12\max_r|z_r|.}
$$

If the algebra is instead written with $2Z$ on its right side, the same result is $M\ge\max_r|Z_r|$; the factor is purely a central-charge convention.

A [BPS state](../../../../../bps-state.md) saturates at least one of these inequalities. The corresponding zero-norm combinations of [supercharges](../../../../../supersymmetry-generator.md) and their adjoints annihilate the representation, so part of [supersymmetry](../../../../../supersymmetry-split.md) is preserved. Its [massive supermultiplet](../../../../../massive-supermultiplet.md) is shortened: each saturated block removes two complex fermionic oscillators, giving $(2j+1)2^{2\mathcal N-2k}$ states from a spin-$j$ [Clifford vacuum](../../../../../clifford-vacuum.md) when $k$ blocks saturate, before any necessary [CPT completion of a supermultiplet](../../../../../cpt-completion-of-a-supermultiplet.md). It preserves $4k$ of the $4\mathcal N$ real [supercharges](../../../../../supersymmetry-generator.md). Its mass is tied to the [central charges in supersymmetry](../../../../../central-charge-in-supersymmetry.md) and remains protected while it stays on the same short branch. Stability is not unconditional: a [wall of marginal stability](../../../../../wall-of-marginal-stability.md) can permit a charged [BPS state](../../../../../bps-state.md) to decay into other [BPS states](../../../../../bps-state.md) with the same total charge.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 68](../../paper-68-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
