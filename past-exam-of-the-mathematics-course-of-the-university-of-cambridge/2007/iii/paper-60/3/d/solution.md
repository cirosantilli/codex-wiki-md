<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Write $X=\sigma_x$, $Y=\sigma_y$, $Z=\sigma_z$. The specified diagonal [two-qubit gate](../../../../../../two-qubit-gate.md) has the exact factorization

$$
C_{\mathrm{phase}}=-Z\otimes Z=R_z(\pi)\otimes R_z(\pi).
$$

Thus one exact implementation is to set the controllable [Ising coupling](../../../../../../ising-coupling-of-two-qubits.md) to zero and perform the two local [rotations about the z-axis](../../../../../../rotation-about-the-z-axis.md), synthesized from the available $x,y$ pulses as in part (c). Alternatively, turn off the local fields and choose the interaction area $\int J_{12}(t)dt=\pi/2$. Then

$$
U_I=e^{-i\pi Z\otimes Z/2}=-iZ\otimes Z=iC_{\mathrm{phase}},
$$

which implements the same physical gate up to [global phase](../../../../../../global-phase.md). **The printed gate is local, not entangling**; the pulse construction does not change that fact.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 60](../../../paper-60-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
