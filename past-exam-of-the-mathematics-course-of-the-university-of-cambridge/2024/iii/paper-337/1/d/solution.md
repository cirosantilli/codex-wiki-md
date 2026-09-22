<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For bosonic [Matsubara frequencies](../../../../../../matsubara-frequency.md) $\omega_n=2\pi nT$, set $a=vk/(2\pi T)$. Applying the [residue theorem](../../../../../../residue-theorem.md) to $\pi\coth(\pi z)/(z^2+a^2)$, whose integer poles reproduce the desired summands, gives

$$
\sum_{n\in\mathbb Z}\frac1{n^2+a^2}=\frac\pi a\coth(\pi a).
$$

It follows that

$$
T\sum_n\frac1{\omega_n^2+v^2k^2}
=\frac1{2vk}\coth\left(\frac{vk}{2T}\right).
$$

Using the area $S_{d-1}=2\pi^{d/2}/\Gamma(d/2)$ of the unit sphere, the [thermal phase fluctuation](../../../../../../thermal-phase-fluctuation.md) becomes

$$
\langle\theta^2\rangle=
\frac{S_{d-1}}{2\chi v(2\pi)^d}
\int_0^\Lambda dk\,k^{d-2}
\coth\left(\frac{vk}{2T}\right).
$$

At small $k$, $\coth(vk/(2T))\sim2T/(vk)$, so the [infrared divergence](../../../../../../infrared-divergence.md) is governed by $\int_0 dk\,k^{d-3}$. It diverges for $d=1,2$ and is finite for $d=3$. Therefore short-range systems cannot have true finite-temperature breaking of this continuous symmetry in one or two dimensions, in agreement with the [Mermin-Wagner theorem](../../../../../../mermin-wagner-theorem.md), whereas it is allowed in three dimensions. In two dimensions a [Berezinskii–Kosterlitz–Thouless transition](../../../../../../berezinskii-kosterlitz-thouless-transition.md) may still produce quasi-long-range order.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 337](../../../paper-337-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
