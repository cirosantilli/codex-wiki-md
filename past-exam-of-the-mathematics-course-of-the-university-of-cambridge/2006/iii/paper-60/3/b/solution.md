<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use $t_0=0$ as in the displayed carrier-phase convention. The drift is diagonal, and conjugation gives

$$
\widetilde H_1(t)=\begin{pmatrix}0&e^{i\omega t}\\e^{-i\omega t}&0\end{pmatrix}.
$$

Multiplying by $A(t)\cos(\omega t+\phi)$ and expanding the cosine into exponentials yields

$$
f(t)\widetilde H_1(t)=\frac{A(t)}2
\begin{pmatrix}
0&e^{-i\phi}+e^{i(2\omega t+\phi)}\\
e^{i\phi}+e^{-i(2\omega t+\phi)}&0
\end{pmatrix}.
$$

The [rotating-wave approximation](../../../../../../rotating-wave-approximation.md) averages away the components oscillating at $2\omega$, retaining

$$
\boxed{H_I^{\rm RWA}(t)=\frac{A(t)}2\begin{pmatrix}0&e^{-i\phi}\\e^{i\phi}&0\end{pmatrix}
=\frac{A(t)}2(\cos\phi\,\sigma_x+\sin\phi\,\sigma_y).}
$$

The envelope is slowly varying and the effective coupling is weak compared with the carrier frequency. The pulse phase selects the transverse rotation axis on the [Bloch sphere](../../../../../../bloch-sphere.md); its [pulse area](../../../../../../quantum-pulse-area.md) determines the angle. Counter-rotating corrections are neglected under this approximation, not identically zero.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 60](../../../paper-60-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
