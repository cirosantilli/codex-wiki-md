<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Write $C=e^2/(4\pi\epsilon_0)$. The [shell theorem](../../../../spherical-shell-theorem.md) makes the [potential energy](../../../../potential-energy.md) of the [electron](../../../../electron.md) constant inside the charged [spherical shell](../../../../spherical-shell.md). Relative to the point-proton [Coulomb potential](../../../../coulomb-potential-energy.md), the perturbation is

$$
\Delta V(r)=\begin{cases}
C\left(\dfrac1r-\dfrac1b\right),&0<r<b,\\
0,&r\geq b.
\end{cases}
$$

It is positive: the finite charge distribution weakens the attraction close to the origin.

The [first-order energy correction](../../../../first-order-energy-correction.md) is the [expectation value](../../../../expectation-value.md) of this perturbation in the unperturbed [hydrogen atom](../../../../hydrogen-atom.md) [ground state](../../../../ground-state.md). Integrating its [probability density](../../../../probability-density.md) over spherical volume gives

$$
\Delta E=\frac{4C}{a_0^3}\int_0^b e^{-2r/a_0}\left(r-\frac{r^2}{b}\right)\,dr.
$$

For a [proton](../../../../proton.md) radius much smaller than the [Bohr radius](../../../../bohr-radius.md), expand the exponential uniformly over this short interval. The leading integral is

$$
\int_0^b\left(r-\frac{r^2}{b}\right)\,dr=\frac{b^2}{6},\qquad
\Delta E=\frac{2Cb^2}{3a_0^3}+O\left(\frac{Cb^3}{a_0^4}\right).
$$

Since $E_{1s}=-C/(2a_0)$, the signed fractional change is

$$
\boxed{\frac{\Delta E}{E_{1s}}=-\frac43\left(\frac b{a_0}\right)^2+O\left(\frac{b^3}{a_0^3}\right)}.
$$

Equivalently, $\Delta E/|E_{1s}|=+4b^2/(3a_0^2)$ to leading order: the [energy](../../../../energy-split.md) increases and the binding-energy magnitude decreases. This is the [finite proton-shell correction to hydrogen ground energy](../../../../finite-proton-shell-correction-to-hydrogen-ground-energy.md).

If no small-radius expansion is made, the same [time-independent perturbation theory](../../../../time-independent-perturbation-theory.md) integral gives, with $\beta=b/a_0$,

$$
\frac{\Delta E}{|E_{1s}|}=2\left[1-\frac1\beta+\left(1+\frac1\beta\right)e^{-2\beta}\right].
$$

Its expansion starts with $4\beta^2/3$, in agreement with the leading result. The integral is exact for the first-order calculation; it is not an exact solution of the perturbed [Schrödinger equation](../../../../schrodinger-equation.md).

## ↑ Ancestors (13)

1. [C](../c.md)
2. [1](../../1.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the advanced quantum physics course of the University of Cambridge](../../../split.md)
5. [Advanced Quantum Physics course of the University of Cambridge](../../../../advanced-quantum-physics-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 3 of the natural sciences course of the University of Cambridge](../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)
