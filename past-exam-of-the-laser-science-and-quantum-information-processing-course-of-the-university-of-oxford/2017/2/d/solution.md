<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Place the input plane one [focal length](../../../../focal-length.md) before a single positive [lens](../../../../lens-optics.md) and the output plane one [focal length](../../../../focal-length.md) after it. The [lens](../../../../lens-optics.md) maps each incident transverse spatial [frequency](../../../../frequency.md) to its corresponding point in the back focal plane. Referencing the input to the front focal plane removes the otherwise present output [phase curvature](../../../../phase-curvature.md), giving an exact scaled [Fourier transform](../../../../fourier-transform-split.md) within the same paraxial model.

A short [ray-matrix](../../../../ray-transfer-matrix-analysis.md) check makes the geometry explicit. With free propagation $P(f)$ and [lens](../../../../lens-optics.md) [matrix](../../../../matrix.md) $L(f)$,

$$
\boxed{P(f)L(f)P(f)=
\begin{pmatrix}1&f\\0&1\end{pmatrix}
\begin{pmatrix}1&0\\-1/f&1\end{pmatrix}
\begin{pmatrix}1&f\\0&1\end{pmatrix}
=\begin{pmatrix}0&f\\-1/f&0\end{pmatrix}.}
$$

The vanishing diagonal entries are the Fourier-plane condition; the output is proportional to $\widetilde E_{\mathrm{in}}(kx/f)$. The final panel of the original diagram in part a shows the two focal distances. A [lens](../../../../lens-optics.md) with input immediately on its surface and output at the back focal plane would generally leave a quadratic output [phase](../../../../phase-waves.md); the front-focal-plane choice avoids it.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [2](../../2.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the laser science and quantum information processing course of the University of Oxford](../../../split.md)
5. [Laser science and quantum information processing course of the University of Oxford](../../../../laser-science-and-quantum-information-processing-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
