<h1 id="15c/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put

$$
k=\frac{\sqrt{2mE}}{\hbar},
\qquad
K=\frac{\sqrt{2m(E+V_0)}}{\hbar}.
$$

The [Time-independent Schrödinger equation](../../../../../../time-independent-schrodinger-equation.md) has the forms

$$
\psi(x)=
\begin{cases}
Ae^{ikx}+Be^{-ikx},&x<0,\\
Ce^{iKx}+De^{-iKx},&0\leq x\leq a,\\
Fe^{ikx},&x>a.
\end{cases}
$$

The first region contains the incident and [reflected waves](../../../../../../reflected-wave.md), while the final region contains only the transmitted wave.

Continuity of $\psi$ and $\psi'$ at both edges of the [finite square well](../../../../../../finite-square-well.md) gives the standard transmission coefficient

$$
T=\frac{|F|^2}{|A|^2}
=\left[
1+\frac{(K^2-k^2)^2}{4k^2K^2}\sin^2(Ka)
\right]^{-1}.
$$

When $V_0=3E$, one has $K=2k$, and therefore

$$
\frac{(K^2-k^2)^2}{4k^2K^2}=\frac9{16},
\qquad
Ka=\frac{a\sqrt{8mE}}{\hbar}.
$$

Hence the [transmission probability](../../../../../../transmission-probability.md) is

$$
\boxed{
T=\frac{16}{16+9\sin^2\!\left(a\sqrt{8mE}/\hbar\right)}
}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [15C](../../15c.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
