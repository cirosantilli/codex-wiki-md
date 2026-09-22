<h1 id="8/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $x\ge0$ denote the radial distance from the axis in the plane, and write $r_h=(x^2+h^2)^{1/2}$. A charge $q$ at height $h$ and its image $-q$ give a combined normal [electric field](../../../../electric-field-split.md) $-2k_eqh/r_h^3$ at $z=0^+$; the tangential components cancel. Superposing the two pairs yields

$$
\boxed{\mathbf E(x,0,0^+)=\frac{Qd}{2\pi\epsilon_0}\left[\frac4{(x^2+4d^2)^{3/2}}-\frac1{(x^2+d^2)^{3/2}}\right]\hat{\mathbf z}}.
$$

The conductor boundary condition gives $\sigma=\epsilon_0E_z$, so

$$
\boxed{\sigma(x)=\frac{Qd}{2\pi}\left[\frac4{(x^2+4d^2)^{3/2}}-\frac1{(x^2+d^2)^{3/2}}\right]}.
$$

To integrate the induced [surface charge](../../../../surface-charge.md), use concentric annuli of area $2\pi x\,dx$. Since $\int_0^\infty x(x^2+h^2)^{-3/2}\,dx=1/h$,

$$
Q_{\rm sheet}=Qd\left(\frac4{2d}-\frac1d\right)=\boxed{+Q}.
$$

The local [surface charge density](../../../../surface-charge-density.md) is negative near the origin but positive farther out; integrating only the negative patch would miss the total. The total real charge is $-Q$, so the induced $+Q$ also agrees with the sum of the two image charges. An isolated finite plate constrained to zero net charge would require a different global boundary-value problem; the formula is the infinite-plane solution just specified.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [8](../../8.md)
3. [2016](../../../2016-split.md)
4. [Past exam of the physics 2 paper of the University of Oxford](../../../split.md)
5. [Physics 2 paper of the University of Oxford](../../../../physics-2-paper-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
