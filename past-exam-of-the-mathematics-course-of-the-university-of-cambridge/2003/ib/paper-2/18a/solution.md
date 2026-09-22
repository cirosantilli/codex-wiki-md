<h1 id="18a/solution">Solution</h1>

↑ **Parent:** [18A](../18a.md)

Take fixed $E>0$ and define $k=\sqrt{2mE}/\hbar$. For sufficiently large $V_0$, the barrier region has $\kappa=\sqrt{2m(V_0-E)}/\hbar$ and solves $\psi''=\kappa^2\psi$. Solving this constant-[coefficient](../../../../../coefficient.md) equation gives the exact transfer relation

$$
\begin{pmatrix}\psi(a)\\\psi'(a)\end{pmatrix}
=\begin{pmatrix}\cosh(\kappa a)&\sinh(\kappa a)/\kappa\\
\kappa\sinh(\kappa a)&\cosh(\kappa a)\end{pmatrix}
\begin{pmatrix}\psi(0)\\\psi'(0)\end{pmatrix}.
$$

In the specified limit, $a=U/V_0$ and $\kappa a\to0$, while

$$
\kappa^2a\to\frac{2mU}{\hbar^2}=:\eta.
$$

The transfer [matrix](../../../../../matrix.md) therefore tends to $\begin{pmatrix}1&0\\\eta&1\end{pmatrix}$. As the two boundaries collapse to the origin, this proves [continuity](../../../../../continuous-function.md) and the [derivative](../../../../../derivative.md) jump for a [delta potential](../../../../../delta-potential.md):

$$
\psi(0+)=\psi(0-),\qquad
\psi'(0+)-\psi'(0-)=\eta\psi(0).
$$

The vanishing exterior phase shift $e^{ika}\to1$ introduces no further factor.

Write the incoming and reflected waves as $e^{ikx}+r e^{-ikx}$ on the left and the transmitted wave as $t e^{ikx}$ on the right. Matching gives

$$
t=1+r,\qquad ikt-ik(1-r)=\eta t,
\qquad t=\frac{2ik}{2ik-\eta}=\frac1{1+i\eta/(2k)}.
$$

The denominator is nonzero for real $\eta$ and $k>0$, so the limiting matching system is well defined. The [probability currents](../../../../../probability-current.md) on either side have the same factor $\hbar k/m$, making the transmission probability $|t|^2$. Thus [scattering by a delta potential](../../../../../scattering-by-a-delta-potential.md) gives

$$
\boxed{T=\frac1{1+\eta^2/(4k^2)}
=\left(1+\frac{mU^2}{2E\hbar^2}\right)^{-1}.}
$$

The limit retains a finite reflection probability despite the barrier's vanishing width because its integrated strength remains finite.

## ↑ Ancestors (10)

1. [18A](../18a.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
