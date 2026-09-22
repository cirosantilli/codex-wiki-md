<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

A superhorizon [density contrast](../../../../../../density-contrast.md) is gauge dependent. The stated growth laws describe the growing [adiabatic mode](../../../../../../adiabatic-mode.md) in the [comoving-gauge density contrast](../../../../../../comoving-gauge-density-contrast.md) (and the corresponding usual synchronous growing mode), not an arbitrary coordinate density perturbation. Work with a flat, single-fluid background with constant $w=p/\rho$, negligible [anisotropic stress](../../../../../../anisotropic-stress.md), $c=1$, and a comoving Fourier wavenumber $K$.

Here is a derivation from the linear gravitational constraints and evolution equation. For an [adiabatic mode](../../../../../../adiabatic-mode.md), the scalar gravitational potential $\Phi$ obeys

$$
\Phi''+3(1+w)\mathcal H\Phi'+wK^2\Phi+
[2\mathcal H'+(1+3w)\mathcal H^2]\Phi=0,
\qquad \mathcal H=\frac{a'}a.
$$

Primes denote [conformal time](../../../../../../conformal-time.md) derivatives. The [Friedmann equation](../../../../../../friedmann-equations.md) gives $a\propto\tau^{2/(1+3w)}$ and $\mathcal H=2/[(1+3w)\tau]$, so the bracket vanishes. On [superhorizon scales](../../../../../../superhorizon-scale.md), $K\tau\ll1$, the leading solutions are a constant potential and a decaying solution proportional to $\tau^{-(5+3w)/(1+3w)}$. Keeping the growing adiabatic branch therefore makes $\Phi$ time independent to leading order.

Combining the time-time and time-space linear Einstein constraints eliminates the coordinate velocity and gives the comoving density constraint

$$
-K^2\Phi=4\pi Ga^2\rho\,\Delta,
\qquad
\Delta=-\frac23\left(\frac{K}{aH}\right)^2\Phi.
$$

This is the relativistic comoving constraint, not a subhorizon Newtonian approximation. Since $\rho\propto a^{-3(1+w)}$, it implies $\Delta\propto(a^2H^2)^{-1}\propto a^{1+3w}$. Also $a\propto t^{2/[3(1+w)]}$ in [cosmic time](../../../../../../cosmic-time.md), whence

$$
\boxed{\frac{\delta(t)}{\delta_i}=
\begin{cases}
t/t_i,&w=1/3\quad\text{(radiation domination)},\\
(t/t_i)^{2/3},&w=0\quad\text{(matter domination)}.
\end{cases}}
$$

Both epochs here mean their respective leading growing solution; matching through [matter-radiation equality](../../../../../../matter-radiation-equality.md) requires the full two-component evolution. The constant superhorizon curvature or potential is consistent with this growth because the comoving density perturbation carries the additional factor $(K/aH)^2$.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 74](../../../paper-74-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
