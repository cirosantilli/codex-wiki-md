<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

To find the [optimal Förster distance for two-state contrast](../../../../optimal-forster-distance-for-two-state-contrast.md), take positive distinct distances $A,B$ and put $x=R_0^6>0$. The magnitude of the efficiency change is

$$
\Delta E=\left|\frac{x}{x+A^6}-\frac{x}{x+B^6}\right|
=\frac{x|B^6-A^6|}{(x+A^6)(x+B^6)}.
$$

Its [derivative](../../../../derivative.md) has the sign of $A^6B^6-x^2$. It rises from zero, has a single maximum at $x=(AB)^3$, then falls back to zero. Hence

$$
\boxed{R_{0,\rm opt}=\sqrt{AB}.}
$$

The printed form is equivalent, since

$$
\frac{A^6-(AB)^3}{(A/B)^3-1}
=\frac{A^3(A^3-B^3)}{(A^3-B^3)/B^3}=A^3B^3.
$$

At this optimum the two efficiencies sum to one and the maximal contrast is $|B^3-A^3|/(B^3+A^3)$. If $A=B$, there is no distance change and the contrast is zero for every $R_0$; the source's unsimplified expression is then $0/0$ and does not specify a unique optimum. For example $A=B=5\,\mathrm{nm}$ yields zero contrast regardless of the fluorophore pair. The geometrical-mean result is a design criterion for distinct distances within the assumed fixed-orientation/photophysics [FRET](../../../../forster-resonance-energy-transfer.md) law, not a correction for dye-orientation changes.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [5](../../5.md)
3. [2018](../../../2018-split.md)
4. [Past exam of the biological physics course of the University of Oxford](../../../split.md)
5. [Biological physics course of the University of Oxford](../../../../biological-physics-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
