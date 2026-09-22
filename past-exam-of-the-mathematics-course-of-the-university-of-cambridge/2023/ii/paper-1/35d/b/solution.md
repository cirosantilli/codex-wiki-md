<h1 id="35d/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For a potential of period $a$, define the [Floquet matrix for a one-dimensional periodic potential](../../../../../../floquet-matrix-for-a-one-dimensional-periodic-potential.md) by

$$
\begin{pmatrix}\psi(x+a)\\\psi'(x+a)\end{pmatrix}
=M(E)\begin{pmatrix}\psi(x)\\\psi'(x)\end{pmatrix}.
$$

The Schrodinger equation has no first-derivative term, so the Wronskian is constant and $\det M=1$. Its multipliers are therefore reciprocal. They lie on the unit circle precisely when

$$
\boxed{|\operatorname{tr}M(E)|\leq2}.
$$

Those energies form continuous allowed bands of bounded [Bloch theorem](../../../../../../bloch-s-theorem.md) solutions. Values with $|\operatorname{tr}M|>2$ have a growing and a decaying multiplier and form forbidden gaps. The band edges have $\operatorname{tr}M=\pm2$, as in [Floquet discriminant and energy bands](../../../../../../floquet-discriminant-and-energy-bands.md).

For the delta-comb [Kronig-Penney model](../../../../../../kronig-penney-model.md), start immediately to the right of one delta function. Free propagation to the next delta and the derivative jump there are represented by

$$
P=
\begin{pmatrix}
\cos ka&\dfrac{\sin ka}{k}\\
-k\sin ka&\cos ka
\end{pmatrix},
\qquad
D=
\begin{pmatrix}
1&0\\
\dfrac{2mV_0}{\hbar^2}&1
\end{pmatrix}.
$$

Thus

$$
\boxed{
M(E)=DP
=
\begin{pmatrix}
\cos ka&\dfrac{\sin ka}{k}\\
\dfrac{2mV_0}{\hbar^2}\cos ka-k\sin ka&
\cos ka+\dfrac{2mV_0}{\hbar^2k}\sin ka
\end{pmatrix}
}.
$$

Consequently the [Floquet discriminant of the delta-comb Kronig-Penney model](../../../../../../floquet-discriminant-of-the-delta-comb-kronig-penney-model.md) is

$$
\boxed{
\frac12\operatorname{tr}M(E)
=\cos(ka)+\gamma\sin(ka)
},
\qquad
\gamma=\frac{mV_0}{\hbar^2k}.
$$

All band edges are therefore determined by

$$
\cos(ka)+\gamma\sin(ka)=\sigma,
\qquad \sigma=\pm1.
$$

In factorized form, the periodic edges $\sigma=1$ obey

$$
\boxed{
\sin\frac{ka}{2}=0
\quad\text{or}\quad
\tan\frac{ka}{2}=\gamma
},
$$

while the antiperiodic edges $\sigma=-1$ obey

$$
\boxed{
\cos\frac{ka}{2}=0
\quad\text{or}\quad
\tan\frac{ka}{2}=-\frac1\gamma
}.
$$

To express the same edges through the single-barrier scattering data, the [One-dimensional transfer matrix from scattering amplitudes](../../../../../../one-dimensional-transfer-matrix-from-scattering-amplitudes.md) gives

$$
\operatorname{tr}M
=\frac{(t^2-r^2)e^{ika}+e^{-ika}}t.
$$

At an edge put $z=e^{-ika}$ and $\operatorname{tr}M=2\sigma$. Then

$$
z^2-2\sigma tz+t^2-r^2=0,
$$

so the [scattering-amplitude equations for one-dimensional band edges](../../../../../../scattering-amplitude-equations-for-one-dimensional-band-edges.md) are

$$
\boxed{e^{-ika}=\sigma t\pm r}.
$$

Explicitly,

$$
\begin{array}{c|c}
\operatorname{tr}M=2&e^{-ika}=t+r\quad\text{or}\quad t-r\\
\operatorname{tr}M=-2&e^{-ika}=-t+r\quad\text{or}\quad -t-r.
\end{array}
$$

For the delta barrier, $t-r=1$ and

$$
t+r=\frac{1-i\gamma}{1+i\gamma},
$$

which reproduces the four factorized edge equations above.

## ↑ Ancestors (11)

1. [B](../b.md)
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
