<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For plume radius $r$, top-hat speed $U$, and plume reduced gravity $g'_B$, define the [volumetric flow rate](../../../../../../volumetric-flow-rate.md), momentum flux, and [buoyancy flux](../../../../../../buoyancy-flux.md)

$$
Q_B=\pi r^2U,
\qquad
M_B=\pi r^2U^2,
\qquad
B=\pi r^2Ug'_B.
$$

The integral balances for a steady [axisymmetric pure plume](../../../../../../axisymmetric-pure-plume.md) in a uniform lower layer are

$$
\frac{dQ_B}{dz}=2\pi\alpha rU,
\qquad
\frac{dM_B}{dz}=\pi r^2g'_B=\frac BU,
\qquad
\frac{dB}{dz}=0.
$$

The source is at the plume's virtual origin $z=0$. Solving these equations gives

$$
r(z)=\frac{6\alpha}{5}z,
$$



$$
U(z)=
\left(\frac{25B}{48\pi\alpha^2}\right)^{1/3}z^{-1/3}.
$$

It is useful to define

$$
C_P=\frac{6\alpha}{5}
\left(\frac{9\alpha}{10}\right)^{1/3}\pi^{2/3}.
$$

Then the remaining similarity laws take the compact form

$$
Q_B(z)=C_PB^{1/3}z^{5/3},
\qquad
g'_B(z)=C_P^{-1}B^{2/3}z^{-5/3}.
$$

The second relation also follows immediately from conservation of [buoyancy flux](../../../../../../buoyancy-flux.md), $B=Q_Bg'_B$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 345](../../../paper-345-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
