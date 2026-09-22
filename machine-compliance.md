# Machine compliance

↑ **Parent:** [Tensile modulus experiment](tensile-modulus-experiment.md)

[Machine compliance](machine-compliance.md) is the extra load-path [displacement](displacement.md) per applied [force](force-split.md) attributed to the apparatus in a specified measurement model. Its units are $\mathrm{m\,N^{-1}}$, the reciprocal units of a [spring constant](spring-constant.md). Here $C_m$ includes the frame, [load cell](load-cell.md), adapters and grips insofar as their deformation contributes to the recorded [crosshead displacement](crosshead-displacement.md) $x$. It is a property of that configuration and readout, rather than a universal constant of the testing machine.

Assume a uniform specimen with initial length $L$, constant $A_0$ and [Young's modulus](young-s-modulus.md) $E$, small axial [elastic deformation](elastic-deformation.md), quasistatic loading, no slip, and a linear, length-independent apparatus response over the chosen [force](force-split.md) window. Equilibrium makes the same [force](force-split.md) act through specimen and apparatus, while their extensions add. The two [springs](spring.md) in series therefore give

$$
x=x_0+\frac{FL}{EA_0}+C_mF,\qquad
q(L)=\frac{dx}{dF}=\frac{L}{EA_0}+C_m,
\qquad k_{\mathrm{obs}}=\frac1{q(L)}.
$$

The offset $x_0$ describes the displacement origin after seating; the slope $q$ describes total compliance. Fitting an intercept avoids forcing an arbitrary zero through the origin, but cannot repair slip or a curved response.

If all of $x-x_0$ is incorrectly attributed to specimen extension, the inferred modulus is

$$
E_{\mathrm{app}}=\frac{L}{A_0q(L)}
=\frac{E}{1+EA_0C_m/L}.
$$

For positive $C_m$, this is too small. The fractional bias is most serious for a short, thick, stiff specimen because its own compliance $L/(EA_0)$ is small. A local [extensometer](extensometer.md) instead has $d(\Delta L_g)/dF=L_g/(EA_0)$ in this ideal model, excluding deformation outside its contacts.

A shaped specimen requires more care. With varying initial cross-sectional [area](surface-area.md) $A(s)$ and uniform $E$, its axial compliance is $\int ds/[EA(s)]$ in the one-dimensional approximation. Shoulder and end deformation must be included explicitly or remain identical between tests and be absorbed into an effective intercept. Changing only the [extensometer](extensometer.md) [gauge length](gauge-length.md) on an unchanged specimen does not change its total compliance and cannot perform a [two-length machine compliance separation](two-length-machine-compliance-separation.md).

**Table of contents**

- [Two-length machine compliance separation](two-length-machine-compliance-separation.md)
  - [Worked two-length tensile compliance example](worked-two-length-tensile-compliance-example.md)

## ↑ Ancestors (8)

1. [Tensile modulus experiment](tensile-modulus-experiment.md)
2. [Young's modulus](young-s-modulus.md)
3. [Linear elasticity](linear-elasticity.md)
4. [Elasticity (physics)](elasticity-physics-split.md)
5. [Continuum mechanics](continuum-mechanics-split.md)
6. [Branches of physics](branches-of-physics.md)
7. [Physics](physics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Crosshead displacement](crosshead-displacement.md)
- [Machine compliance](machine-compliance.md)
- [Tensile modulus experiment](tensile-modulus-experiment.md)
- [Two-length machine compliance separation](two-length-machine-compliance-separation.md)
- [Worked two-length tensile compliance example](worked-two-length-tensile-compliance-example.md)
