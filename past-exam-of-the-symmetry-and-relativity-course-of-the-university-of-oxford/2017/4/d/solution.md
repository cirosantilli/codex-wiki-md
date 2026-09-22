<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Use a neutral, infinitely long wire on the $x$ axis. Denote the total current by $I=\int j_x\,dA_\perp$, and write $r^2=y^2+z^2$. Outside the wire the [magnetic field](../../../../magnetic-field-split.md) and [electric field](../../../../electric-field-split.md) are

$$
\boxed{\mathbf E=0,\qquad
\mathbf B=\frac{\mu_0I}{2\pi r^2}(0,-z,y).}
$$

These follow from cylindrical symmetry and [Ampère's law](../../../../ampere-s-circuital-law.md). The zero temporal component of the given total [four-current](../../../../four-current.md) specifies lab neutrality; the $\rho$ in $j_x=\rho v_0$ must refer to a carrier density, not that zero net charge density.

**TODO: normalization from a literal volume [current density](../../../../current-density.md) requires the unspecified wire cross-section.** The source does not supply its area or profile. The exterior field family below is fully determined in terms of $I$; it cannot be reduced to $j_x$ alone without that missing datum. If $j_x$ was intended as a cross-section-integrated line current instead, set $I=j_x$ and interpret its accompanying charge density as charge per length. No inside-wire profile is invented.

For a boost $u=v_0$ along positive $y$, let $\Gamma=(1-u^2/c^2)^{-1/2}$. Apply the [Lorentz transformation of electromagnetic fields](../../../../lorentz-transformation-of-electromagnetic-fields.md) at corresponding events:

$$
\boxed{\mathbf E'_\perp=(\Gamma uB_z,0,0),\qquad
\mathbf B'_\perp=(0,B_y,\Gamma B_z).}
$$

Here the subscript labels the perpendicular-to-wire boost, not the direction of the transformed vector. In these formulas evaluate the original field at $y=\Gamma(y'+ut')$, $z=z'$ and $x=x'$. The wire moves in this frame, so the fields are time-dependent. The local current transforms to $J'^0=0$, $J'^x=j_x$, $J'^y=J'^z=0$. A nonzero transformed [electric field](../../../../electric-field-split.md) is possible even with zero net charge density: it is not a purely electrostatic field.

For a boost $u=v_0$ along positive $x$, the transverse coordinates are unchanged. The transformed fields are

$$
\boxed{\mathbf E'_\parallel=(0,-\Gamma uB_z,\Gamma uB_y)
=-\frac{\Gamma\mu_0uI}{2\pi r^2}(0,y,z),\qquad
\mathbf B'_\parallel=\Gamma\mathbf B.}
$$

The transformed line charge and current are $\lambda'=-\Gamma uI/c^2$ and $I'=\Gamma I$. These reproduce the radial [electric field](../../../../electric-field-split.md) through [Gauss's law](../../../../gauss-s-law.md). A boost comoving with the [electrons](../../../../electron.md) removes their individual current contribution, but the positive background then moves and the total current is not zero.

For two identical wires, their lab interaction is attractive, with magnitude $\mu_0I^2/(2\pi d)$ per length. The total [four-current](../../../../four-current.md) is spacelike, $J^2=-j_x^2<0$, so no inertial frame makes it a pure charge density. Also $B^2-E^2/c^2=B^2>0$ forbids a frame in which the exterior field is purely electric. For an arbitrary boost along the wires, the electrical part is repulsive and the magnetic part attractive:

$$
\frac{F'_E}{L'}=+\frac{\Gamma^2u^2}{c^2}\frac{\mu_0I^2}{2\pi d},\qquad
\frac{F'_B}{L'}=-\Gamma^2\frac{\mu_0I^2}{2\pi d}.
$$

The latter always dominates, and their sum remains $-\mu_0I^2/(2\pi d)$.

Even a more general boost cannot make the entire-wire force electrical alone. At the second wire choose $y=d,z=0$, so $\mathbf B=B\mathbf e_z$ and $\mathbf j=j\mathbf e_x$ with $jB>0$. The physical [Lorentz force density](../../../../lorentz-force-density.md) is $f=(0,0,-jB,0)$. If the boosted magnetic force vanished, $\mathbf j'\times\mathbf B'=0$, then $\mathbf E'\cdot\mathbf B'=0$ would also give $\mathbf j'\cdot\mathbf E'=0$. Thus $f'^0=0$, which from the boost of $f$ requires $V_y=0$. But for such a boost $f'^y=-jB<0$, whereas $\rho'E'_y=\Gamma_V^2V_x^2jB/c^2\geq0$. The electrical term alone cannot equal the actual force. Therefore there is no such frame for both complete wires, although the force on [electrons](../../../../electron.md) considered separately can be electrical in their rest frame.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [4](../../4.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the symmetry and relativity course of the University of Oxford](../../../split.md)
5. [Symmetry and relativity course of the University of Oxford](../../../../symmetry-and-relativity-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
