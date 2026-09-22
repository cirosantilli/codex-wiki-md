<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Write the unknown pure [photon polarization](../../../../../../photon-polarization.md) [qubit](../../../../../../qubit.md) as

$$
|\psi\rangle=\alpha|H\rangle+\beta|V\rangle,\qquad |\alpha|^2+|\beta|^2=1.
$$

The [polarizing beam splitter](../../../../../../polarizing-beam-splitter.md) sends the $H$ component down the lower path and the $V$ component up the upper path. After rotating the upper [photon polarization](../../../../../../photon-polarization.md) to $H$, both paths have the same internal [quantum state](../../../../../../quantum-state.md) and can interfere at BS2. Absorb fixed apparatus phases into a calibrated zero for the tunable [quantum phase](../../../../../../quantum-phase.md). With the preceding reflection convention, the [quantum state](../../../../../../quantum-state.md) before BS2 is $(\alpha|\ell\rangle+i\beta e^{i\theta}|u\rangle)|H\rangle$, so the two output amplitudes are

$$
a_1=\frac{i}{\sqrt2}(\alpha+\beta e^{i\theta}),\qquad a_0=\frac1{\sqrt2}(\alpha-\beta e^{i\theta}).
$$

Consequently

$$
\boxed{P_1(\theta)=\frac12+\operatorname{Re}(\gamma e^{i\theta}),\qquad \gamma=\alpha^*\beta,\qquad P_0=1-P_1.}
$$

Repeated counts while scanning $\theta$ determine the complex [quantum coherence](../../../../../../quantum-coherence-in-a-specified-basis.md) $\gamma$. The [interference visibility](../../../../../../interferometric-visibility.md) is $2|\gamma|$, and the fringe position determines the relative [quantum phase](../../../../../../quantum-phase.md) $\arg\beta-\arg\alpha$ whenever both components are nonzero.

A fringe alone is not enough to determine an arbitrary [photon polarization](../../../../../../photon-polarization.md) [quantum state](../../../../../../quantum-state.md): it fixes $|\alpha\beta|$ but not which of $|\alpha|^2$ and $|\beta|^2$ is larger. Indeed, $|H\rangle$ and $|V\rangle$ both give the flat fringe $P_1=1/2$. For a general [pure quantum state](../../../../../../pure-state.md), the two possible population differences are

$$
|\alpha|^2-|\beta|^2=\pm\sqrt{1-4|\gamma|^2}.
$$

Resolve this ambiguity by temporarily detecting the two paths before BS2. Their relative counts give $h=|\alpha|^2$ and $1-h=|\beta|^2$ using the same [polarizing beam splitter](../../../../../../polarizing-beam-splitter.md) and detectors. Taking $\alpha=\sqrt h$ as a global-phase choice, the reconstructed [quantum state](../../../../../../quantum-state.md) for $h>0$ is

$$
\boxed{|\psi\rangle=\sqrt h\,|H\rangle+\frac{\gamma}{\sqrt h}|V\rangle.}
$$

If $h=0$, it is $|V\rangle$ up to a [global phase](../../../../../../global-phase.md). This completes [interferometric polarization tomography](../../../../../../interferometric-polarization-tomography.md). The counts are obtained from many identically prepared [photons](../../../../../../photon.md); they do not identify an arbitrary [quantum state](../../../../../../quantum-state.md) from one [photon](../../../../../../photon.md).

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 58](../../../paper-58-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
