<h1 id="35d/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a wave incident from the left, define the reflection and transmission amplitudes by

$$
\psi(x)\sim
\begin{cases}
e^{ikx}+r e^{-ikx},&x\to-\infty,\\
t e^{ikx},&x\to+\infty,
\end{cases}
\qquad
E=\frac{\hbar^2k^2}{2m}.
$$

Reflection invariance gives the same amplitudes for incidence from the right. If the incoming amplitudes from the left and right are ordered first, and the outgoing amplitudes toward the left and right second, the [One-dimensional S-matrix](../../../../../../one-dimensional-s-matrix.md) is

$$
\boxed{
S=\begin{pmatrix}r&t\\t&r\end{pmatrix}
}.
$$

For $V(x)=V_0\delta(x)$, the [wavefunction](../../../../../../wave-function.md) is continuous and its derivative has the jump

$$
\psi'(0^+)-\psi'(0^-)
=\frac{2mV_0}{\hbar^2}\psi(0).
$$

The scattering ansatz gives

$$
1+r=t,
\qquad
2ik r=\frac{2mV_0}{\hbar^2}t.
$$

With

$$
\gamma=\frac{mV_0}{\hbar^2k},
$$

we obtain the [scattering by a delta potential](../../../../../../scattering-by-a-delta-potential.md) amplitudes

$$
\boxed{
t=\frac1{1+i\gamma},
\qquad
r=\frac{-i\gamma}{1+i\gamma}
}.
$$

They satisfy

$$
|r|^2+|t|^2=1,
\qquad
r^*t+t^*r=0.
$$

Therefore

$$
S^\dagger S
=\begin{pmatrix}
|r|^2+|t|^2&r^*t+t^*r\\
t^*r+r^*t&|r|^2+|t|^2
\end{pmatrix}
=I,
$$

so the scattering matrix is unitary.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [35D](../../35d.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
