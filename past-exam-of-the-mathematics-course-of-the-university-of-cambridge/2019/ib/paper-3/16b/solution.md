<h1 id="16b/solution">Solution</h1>

↑ **Parent:** [16B](../16b.md)

Inside the [infinite square well](../../../../../infinite-square-well.md), the stationary [Schrödinger equation](../../../../../schrodinger-equation.md) for unit mass is

$$
-\frac{\hbar^2}{2}\psi''=E\psi,
\qquad \psi(0)=\psi(\pi)=0.
$$

Its normalized eigenstates and energies are

$$
\boxed{\psi_n(x)=\sqrt{\frac2\pi}\sin(nx),
\qquad E_n=\frac{\hbar^2n^2}{2}},
\qquad n=1,2,\ldots.
$$

The general normalized time-dependent solution is

$$
\boxed{\Psi(x,t)=\sum_{n=1}^\infty c_n\psi_n(x)e^{-iE_nt/\hbar},
\qquad \sum_{n=1}^\infty|c_n|^2=1}.
$$

Immediately after removing the barrier, the normalized wavefunction is

$$
\Psi(x,0)=
\begin{cases}
\sqrt{4/\pi}\sin(2x),&0\leq x\leq\pi/2,\\
0,&\pi/2<x\leq\pi.
\end{cases}
$$

Its [Fourier sine series](../../../../../fourier-sine-series.md) coefficients in the full-well basis are

$$
c_n=\frac{\sqrt8}{\pi}\int_0^{\pi/2}\sin(nx)\sin(2x)\,dx.
$$

They are

$$
c_2=\frac1{\sqrt2},
\qquad
c_n=\frac{4\sqrt2}{\pi}\frac{\sin(n\pi/2)}{4-n^2}\quad(n\ne2).
$$

The [Born rule](../../../../../born-rule.md) therefore gives

$$
\boxed{
\mathbb P(E_n)=
\begin{cases}
\dfrac12,&n=2,\\[4pt]
\dfrac{32}{\pi^2(n^2-4)^2},&n\text{ odd},\\[4pt]
0,&n\text{ even and }n\ne2.
\end{cases}}
$$

## ↑ Ancestors (10)

1. [16B](../16b.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
