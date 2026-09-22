<h1 id="7/solution">Solution</h1>

↑ **Parent:** [7](../7.md)

Encode $|0\rangle=|H\rangle$ and $|1\rangle=|V\rangle$ in two orthogonal linear [polarizations](../../../polarization-waves.md). Then $|\pm\rangle=(|H\rangle\pm|V\rangle)/\sqrt2$ are linear polarizations at opposite forty-five-degree angles, while $(|H\rangle\pm i|V\rangle)/\sqrt2$ are the two circular polarizations. Their right/left names depend on the viewing convention. A [half-wave plate](../../../half-wave-plate.md) with its axis at $22.5^\circ$ to H implements H up to a common phase, since its Jones matrix has entries $\cos2\theta,\sin2\theta$ and $-\cos2\theta$.

In principle, a nonlinear interaction producing $e^{i\pi n_{1V}n_{2V}}$ supplies a deterministic [Controlled-Z gate](../../../controlled-z-gate.md): only the joint VV component acquires a minus sign. A strongly coupled matter mediator can also provide the required conditional interaction. At optical single-photon energies the direct nonlinear interaction is weak; loss, unwanted noise and maintaining indistinguishable spatial and temporal modes make a high-fidelity deterministic gate difficult. Passive linear optics by itself does not supply this deterministic entangling interaction; measurement-based optical gates introduce additional resources and success conditions.

For the printed circuit, the first three H gates create $|+\rangle^{\otimes3}$. The two controlled-Z operations from the first qubit to the others give

$$
\frac1{\sqrt2}\left(|0\rangle|+\rangle|+\rangle+|1\rangle|-\rangle|-\rangle\right).
$$

The final H gates on the last two qubits therefore produce the [GHZ state](../../../greenberger-horne-zeilinger-state.md)

$$
\boxed{|\psi\rangle=\frac{|000\rangle+|111\rangle}{\sqrt2}.}
$$

Define $|s_X\rangle=(|0\rangle+s|1\rangle)/\sqrt2$ and $|s_Y\rangle=(|0\rangle+is|1\rangle)/\sqrt2$ for $s=\pm1$. In any of the XYY, YXY and YYX bases, direct overlaps give

$$
\langle s_Xt_Yu_Y|\psi\rangle=\frac{1-stu}{4},
$$

with the same coefficient formula when the X position is permuted. Hence the three explicit expansions can be written compactly as

$$
|\psi\rangle=\frac12\sum_{stu=-1}|s_Xt_Yu_Y\rangle=\frac12\sum_{stu=-1}|s_Yt_Xu_Y\rangle=\frac12\sum_{stu=-1}|s_Yt_Yu_X\rangle.
$$

In each sum the four sign triples are $(+,+,-),(+,-,+),(-,+,+),(-,-,-)$. They have equal probabilities $1/4$. Thus two Y outcomes determine the X outcome with certainty: their product times the X outcome is $-1$.

In the XXX basis,

$$
\langle s_Xt_Xu_X|\psi\rangle=\frac{1+stu}{4},\qquad\boxed{|\psi\rangle=\frac12\sum_{stu=+1}|s_Xt_Xu_X\rangle.}
$$

The four allowed triples are $(+,+,+),(+,-,-),(-,+,-),(-,-,+)$, so the XXX outcome product is $+1$.

The [GHZ theorem](../../../ghz-theorem.md) follows without a statistical inequality. If local predetermined values $X_i,Y_i\in\{\pm1\}$ reproduced the three mixed-basis correlations, multiplying them would give

$$
(X_1Y_2Y_3)(Y_1X_2Y_3)(Y_1Y_2X_3)=-1\quad\Longrightarrow\quad X_1X_2X_3=-1,
$$

because every Y value is squared. Quantum mechanics instead predicts the XXX product $+1$. This is an all-versus-nothing contradiction with [local realism](../../../local-realism.md) using ideal perfect correlations. Standard two-qubit Bell-state tests compare statistical correlations through a [Bell inequality](../../../bell-inequality.md); the GHZ construction makes the inconsistency visible already at the level of these deterministic parity constraints.

## ↑ Ancestors (11)

1. [7](../7.md)
2. [2016](../../2016-split.md)
3. [Past exam of the laser science and quantum information processing course of the University of Oxford](../../split.md)
4. [Laser science and quantum information processing course of the University of Oxford](../../../laser-science-and-quantum-information-processing-course-of-the-university-of-oxford.md)
5. [Year 4 of the physics course of the University of Oxford](../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
