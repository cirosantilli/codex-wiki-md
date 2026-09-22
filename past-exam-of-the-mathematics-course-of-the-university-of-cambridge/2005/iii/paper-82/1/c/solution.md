<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use a [time-harmonic wave](../../../../../../time-harmonic-wave.md) with time dependence $e^{-i\omega t}$ and let the same symbols denote phasors. The [wave amplitude](../../../../../../wave-amplitude.md) vector obeys

$$
\frac{d}{dx}\begin{pmatrix}\phi_+\\\phi_-\end{pmatrix}=\begin{pmatrix}i\omega/\beta&g\\g&-i\omega/\beta\end{pmatrix}\begin{pmatrix}\phi_+\\\phi_-\end{pmatrix}.
$$

At fixed material contrast, the stated low-frequency condition permits neglecting the diagonal [frequency](../../../../../../frequency.md) term to zeroth order. All remaining coefficient [matrices](../../../../../../matrix.md) are scalar multiples of the same exchange [matrix](../../../../../../matrix.md), so they commute. With

$$
L=\int_{x_a}^{x_b}g\,dx=\frac12\log\frac{Z_b}{Z_a},\qquad C=\cosh L,\quad H=\sinh L,
$$

the transfer relation is

$$
\begin{pmatrix}\phi_+(x_b)\\\phi_-(x_b)\end{pmatrix}=\begin{pmatrix}C&H\\H&C\end{pmatrix}\begin{pmatrix}\phi_+(x_a)\\\phi_-(x_a)\end{pmatrix}.
$$

Solve the second row for the outgoing left [wave amplitude](../../../../../../wave-amplitude.md) and substitute in the first. Since $C^2-H^2=1$, this gives the [zero-frequency scattering through an elastic layer](../../../../../../zero-frequency-scattering-through-an-elastic-layer.md) coefficients

$$
\boxed{R_{aa}=\frac{Z_a-Z_b}{Z_a+Z_b},\quad R_{bb}=\frac{Z_b-Z_a}{Z_a+Z_b},\quad T_{ab}=T_{ba}=\frac{2\sqrt{Z_aZ_b}}{Z_a+Z_b}.}
$$

Thus the zero-frequency limit depends only on the endpoint [seismic impedances](../../../../../../seismic-impedance.md). Monotonicity supports the given scale comparison but is not needed to integrate the zero-frequency equation. If $Z_a=Z_b$ in a monotone profile, [seismic impedance](../../../../../../seismic-impedance.md) is constant: there is no directional coupling, with only [wave phase](../../../../../../phase-waves.md) accumulation at nonzero [frequency](../../../../../../frequency.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 82](../../../paper-82-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
