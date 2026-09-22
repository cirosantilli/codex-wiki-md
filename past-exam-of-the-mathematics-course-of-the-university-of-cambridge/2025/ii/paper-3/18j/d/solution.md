<h1 id="18j/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let $E=\mathbb Q(\alpha,\beta)$. Since

$$
\sqrt3=\alpha^2-3,\qquad
\sqrt6=\alpha\beta,\qquad
\sqrt2=\frac{\sqrt6}{\sqrt3},
$$

part (b) gives $[E:\mathbb Q]=8$. The roots of $X^4-6X^2+6$ are $\mathord\pm\alpha,\mathord\pm\beta$, all in $E$, so $E$ is its splitting field and is Galois. Its action on the four roots is transitive; the order-eight entry in the list from part (a) is $D_8$. Therefore

$$
\operatorname{Gal}(E/\mathbb Q)\cong D_8.
$$

For an explicit [dihedral Galois action on four radical roots](../../../../../../dihedral-galois-action-on-four-radical-roots.md), define

$$
r(\alpha)=\beta,\qquad r(\beta)=-\alpha,\qquad
s(\alpha)=\alpha,\qquad s(\beta)=-\beta.
$$

Then $r^4=s^2=1$ and $srs=r^{-1}$. The subgroup lattice is determined by

$$
\begin{array}{c}
D_8\\[1mm]
\langle r\rangle\qquad
\langle r^2,s\rangle\qquad
\langle r^2,rs\rangle\\[1mm]
\langle r^2\rangle\quad
\langle s\rangle\quad\langle r^2s\rangle\quad
\langle rs\rangle\quad\langle r^3s\rangle\\[1mm]
\{1\}.
\end{array}
$$

Here $\langle r^2\rangle$ lies in all three order-four subgroups; $\langle s\rangle,\langle r^2s\rangle$ lie in $\langle r^2,s\rangle$; and $\langle rs\rangle,\langle r^3s\rangle$ lie in $\langle r^2,rs\rangle$.

Reversing inclusions under the [Galois correspondence](../../../../../../galois-correspondence.md) gives the complete field lattice

$$
\begin{array}{c}
E\\[1mm]
\mathbb Q(\sqrt2,\sqrt3)\quad
\mathbb Q(\alpha)\quad\mathbb Q(\beta)\quad
\mathbb Q(\alpha+\beta)\quad\mathbb Q(\alpha-\beta)\\[1mm]
\mathbb Q(\sqrt2)\qquad
\mathbb Q(\sqrt3)\qquad
\mathbb Q(\sqrt6)\\[1mm]
\mathbb Q.
\end{array}
$$

The incidence is likewise reversed: $\mathbb Q(\sqrt2)$ lies in $\mathbb Q(\sqrt2,\sqrt3)$; $\mathbb Q(\sqrt3)$ lies in that field, $\mathbb Q(\alpha)$, and $\mathbb Q(\beta)$; and $\mathbb Q(\sqrt6)$ lies in that field, $\mathbb Q(\alpha+\beta)$, and $\mathbb Q(\alpha-\beta)$. The hint verifies the last two quartic fields through $\alpha+\beta=\sqrt2\gamma$ and $\alpha-\beta=\sqrt2\delta$.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [18J](../../18j.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
