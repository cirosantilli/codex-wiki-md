<h1 id="16g/solution">Solution</h1>

↑ **Parent:** [16G](../16g.md)

Take zero [electric potential](../../../../../electric-potential.md) at infinity and put $K=(4\pi\varepsilon_0)^{-1}$. By [spherical symmetry](../../../../../spherical-symmetry.md) and [Gauss's law](../../../../../gauss-s-law.md), the [electric field](../../../../../electric-field.md) is radial, with magnitude determined by the total enclosed [electric charge](../../../../../electric-charge.md). Thus, away from the idealized shell surfaces,

$$
\boxed{\mathbf E(r)=Kq\begin{cases}
0,&0\le r<a,\\
\mathbf e_r/r^2,&a<r<b,\\
-\mathbf e_r/r^2,&b<r<c,\\
2\mathbf e_r/r^2,&r>c.
\end{cases}}
$$

Integrating $E_r=-d\Phi/dr$ from infinity, or adding the three spherical-shell potentials, gives

$$
\boxed{\Phi(r)=Kq\begin{cases}
a^{-1}-2b^{-1}+3c^{-1},&r\le a,\\
r^{-1}-2b^{-1}+3c^{-1},&a\le r\le b,\\
-r^{-1}+3c^{-1},&b\le r\le c,\\
2r^{-1},&r\ge c.
\end{cases}}
$$

The expressions agree at each interface, so the potential is continuous everywhere, including the origin. The [electric field](../../../../../electric-field.md) has different interior and exterior limits at each infinitely thin charged surface, with jump equal to [surface charge density](../../../../../surface-charge-density.md) divided by $\varepsilon_0$. An ideal sheet has no single classical field value on the sheet itself; the displayed adjacent limits specify the field there. In conducting material of nonzero thickness the internal field is zero.

The [electrostatic energy](../../../../../electrostatic-energy.md) is the [integral](../../../../../integral.md) of $\varepsilon_0|\mathbf E|^2/2$. There is no contribution from $r<a$, and spherical integration gives

$$
U=\frac{q^2}{8\pi\varepsilon_0}\left[\int_a^b\frac{dr}{r^2}+\int_b^c\frac{dr}{r^2}+4\int_c^\infty\frac{dr}{r^2}\right]
=\boxed{\frac{q^2}{8\pi\varepsilon_0}\left(\frac1a+\frac3c\right).}
$$

The dependence on $b$ cancels because the magnitude of enclosed [electric charge](../../../../../electric-charge.md) is $|q|$ on both sides of the middle shell, even though the field direction changes.

## ↑ Ancestors (10)

1. [16G](../16g.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
