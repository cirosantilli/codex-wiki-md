<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Now let the basic buoyancy be

$$
B=M^2x+N^2z.
$$

[Thermal-wind balance](../../../../../../thermal-wind.md) requires the basic along-front velocity to have vertical shear $V_z=M^2/f$, so

$$
\boldsymbol U=\left(0,\Lambda x+\frac{M^2}{f}z,0\right).
$$

The basic absolute vorticity and buoyancy gradient are

$$
\boldsymbol\omega_a
=\left(-\frac{M^2}{f},0,f+\Lambda\right),
\qquad
\boldsymbol\nabla B=(M^2,0,N^2),
$$

and hence

$$
Q=\boldsymbol\omega_a\mathbin{\cdot}\boldsymbol\nabla B
=(f+\Lambda)N^2-\frac{M^4}{f}.
$$

For the prescribed disturbance the [buoyancy perturbation](../../../../../../buoyancy-perturbation.md) vanishes, so the linearized buoyancy equation and [incompressibility](../../../../../../incompressible-flow.md) give

$$
M^2u+N^2w=0,\qquad ku+mw=0.
$$

The wavevector must therefore satisfy

$$
\frac{m}{k}=\frac{N^2}{M^2};
$$

the disturbance velocity lies along a basic [isopycnal](../../../../../../isopycnal.md). The along-front momentum equation becomes

$$
-i\omega v+
\left(f+\Lambda-\frac{M^4}{fN^2}\right)u=0
=-i\omega v+\frac{Q}{N^2}u.
$$

Projecting the remaining momentum equations onto the divergence-free direction eliminates the pressure and yields

$$
\omega^2=\frac{fQ}{N^2}\frac{m^2}{k^2+m^2}
=\frac{fQN^2}{N^4+M^4}.
$$

Thus this isopycnal disturbance grows if and only if $fQ<0$. Geometrically, $Q$ is the component of the absolute vorticity along the buoyancy gradient, multiplied by $|\boldsymbol\nabla B|$; the horizontal buoyancy gradient reduces that component through the term $-M^4/f$. When $M=0$, the result reduces to the most unstable, nearly horizontal-wavevector limit of part i.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 333](../../../paper-333-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
