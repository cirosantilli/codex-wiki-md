<h1 id="1/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

Write $\cos\omega_1t=(e^{i\omega_1t}+e^{-i\omega_1t})/2$ and $\Delta\omega=\omega_2-\omega_1$. Multiplication of the matrix from part (e) gives

$$
\begin{aligned}
fH_I=\frac{A_1(t)}2\{&d_1(1+e^{-2i\omega_1t})E_{12}+d_1(1+e^{2i\omega_1t})E_{21}\\
&+d_2[e^{i\Delta\omega t}+e^{i(2\omega_1+\Delta\omega)t}]E_{23}\\
&+d_2[e^{-i\Delta\omega t}+e^{-i(2\omega_1+\Delta\omega)t}]E_{32}\}.
\end{aligned}
$$

These are exactly the constant, difference-frequency, and sum-frequency terms in the PDF, with each Hermitian pair visible. For a weak, slowly varying envelope, the terms at $2\omega_1$ and $\omega_1+\omega_2$ average out by the [rotating-wave approximation](../../../../../../rotating-wave-approximation.md). To discard the other transition as well, its detuning must be nonzero and large compared with the drive coupling and envelope bandwidth. Sufficient scale conditions are

$$
|A_1d_j|,\ B\ll\omega_1,\omega_2,\qquad
|A_1d_2|,\ B\ll|\Delta\omega|,
$$

where $B$ is a characteristic envelope bandwidth; turn-on transients must satisfy the same spectral restrictions. Then

$$
\boxed{fH_I\simeq\frac{A_1(t)d_1}{2}(E_{12}+E_{21}).}
$$

Small coupling compared with the optical frequencies alone is not enough for this selective approximation: if $|\Delta\omega|$ is comparable with the pulse bandwidth or Rabi scale, the spectator transition remains driven. A long selective gate also accumulates a small off-resonant Stark phase of order $(A_1d_2)^2/\Delta\omega$, so that error must be acceptable or compensated. These assumptions distinguish [resonant quantum control](../../../../../../resonant-quantum-control.md) from an exact decoupling.

## ↑ Ancestors (11)

1. [F](../f.md)
2. [1](../../1.md)
3. [Paper 61](../../../paper-61-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
