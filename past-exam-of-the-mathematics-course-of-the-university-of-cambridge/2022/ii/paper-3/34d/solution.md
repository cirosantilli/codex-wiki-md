<h1 id="34d/solution">Solution</h1>

↑ **Parent:** [34D](../34d.md)

Every primitive basis of the [Bravais lattice](../../../../../bravais-lattice.md) has the form

$$
\boxed{
a_1'=p a_1+q a_2,
\qquad
a_2'=r a_1+s a_2
},
$$

where $p,q,r,s\in\mathbb Z$ and

$$
\boxed{ps-qr=\pm1}.
$$

The unimodular determinant condition is exactly what makes the integer change of basis invertible over $\mathbb Z$.

Let $b_i$ be the primitive vectors of the [reciprocal lattice](../../../../../reciprocal-lattice.md), with

$$
a_i\cdot b_j=2\pi\delta_{ij}.
$$

Solving these four equations gives

$$
\boxed{
b_1=\left(2\pi,\frac{2\pi}{\sqrt3}\right),
\qquad
b_2=\left(0,\frac{4\pi}{\sqrt3}\right)
}.
$$

The six reciprocal-lattice points nearest the origin are

$$
\pm b_1,\qquad
\pm b_2,\qquad
\pm(b_2-b_1),
$$

all at distance $4\pi/\sqrt3$.

The [Wigner-Seitz cell](../../../../../wigner-seitz-cell.md) is bounded by the perpendicular bisectors of the segments joining the origin to those six points. It is the regular hexagon with vertices

$$
\boxed{
\left(\frac{4\pi}{3},0\right),
\left(\frac{2\pi}{3},\frac{2\pi}{\sqrt3}\right),
\left(-\frac{2\pi}{3},\frac{2\pi}{\sqrt3}\right),
\left(-\frac{4\pi}{3},0\right),
\left(-\frac{2\pi}{3},-\frac{2\pi}{\sqrt3}\right),
\left(\frac{2\pi}{3},-\frac{2\pi}{\sqrt3}\right)
}.
$$

Its area equals the reciprocal primitive-cell area:

$$
\boxed{
|b_1\times b_2|=\frac{8\pi^2}{\sqrt3}
}.
$$

This is the [reciprocal lattice and Wigner-Seitz cell of the unit triangular lattice](../../../../../reciprocal-lattice-and-wigner-seitz-cell-of-the-unit-triangular-lattice.md).

For a periodic potential, [Bloch theorem](../../../../../bloch-s-theorem.md) identifies wavevectors differing by a reciprocal-lattice vector. The first [Brillouin zone](../../../../../brillouin-zone.md) is the Wigner--Seitz cell just found. More generally, the $n$th Brillouin zone consists of wavevectors reached from the origin after crossing exactly $n-1$ reciprocal-lattice Bragg planes; its boundaries are the perpendicular bisectors

$$
k\cdot G=\frac{|G|^2}{2},
\qquad G\in\Lambda^*\setminus\{0\}.
$$

For this triangular reciprocal lattice, the first zone is the central regular hexagon. The second is the sixfold-symmetric collection of regions immediately outside its six sides, bounded next by the bisectors associated with the next reciprocal points. These zones organize free-particle states into bands: Bragg coupling is strongest at their boundaries and opens energy gaps when the periodic potential is introduced.

## ↑ Ancestors (10)

1. [34D](../34d.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
