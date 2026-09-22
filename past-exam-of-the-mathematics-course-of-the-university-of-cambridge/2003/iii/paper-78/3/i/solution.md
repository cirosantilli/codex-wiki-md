<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let the layer occupy $0<z<h$, with a free surface at $z=0$ and rigid base at $z=h$. Write an [SH-wave](../../../../../../sh-wave.md) as $u_y=Y(z)e^{i(kx-\omega t)}$. The equation and boundary conditions give

$$
Y''+q^2Y=0,\qquad q^2=\frac{\omega^2}{\beta'^2}-k^2,
\qquad Y'(0)=0,\quad Y(h)=0.
$$

Thus $Y=A\cos(qz)$ and the [guided SH modes between rigid and free planes](../../../../../../guided-sh-modes-between-rigid-and-free-planes.md) have

$$
q_n=\frac{\chi_n}{h},\quad\chi_n=(n+\tfrac12)\pi,\quad n=0,1,2,\ldots,
\qquad\omega^2=\beta'^2k^2+\omega_n^2,\quad\omega_n=\frac{\beta'\chi_n}{h}.
$$

The propagating branch has $\omega>\omega_n$ and $k=\sqrt{\omega^2-\omega_n^2}/\beta'$. Hence the [rigid-base approximation to Love waves](../../../../../../rigid-base-approximation-to-love-waves.md) predicts

$$
\boxed{c_n(\omega)=\frac{\beta'}{\sqrt{1-\omega_n^2/\omega^2}},\qquad
U_n(\omega)=\beta'\sqrt{1-\omega_n^2/\omega^2},\qquad c_nU_n=\beta'^2}.
$$

At each threshold $c_n\to\infty$ and $U_n\to0$. As [frequency](../../../../../../frequency.md) rises, the [phase velocity](../../../../../../phase-velocity.md) decreases towards $\beta'$ and the [group velocity](../../../../../../group-velocity.md) increases towards $\beta'$. [Frequencies](../../../../../../frequency.md) below $\omega_n$ have imaginary horizontal [wavenumber](../../../../../../wavenumber.md) and do not give propagating guided modes. The infinite threshold phase speed does not violate causality: the limiting group speed is zero. These quarter-wave thresholds differ from the actual [Love-wave cutoff frequencies](../../../../../../love-wave-cutoff-frequencies.md) of an elastic substrate.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 78](../../../paper-78-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
