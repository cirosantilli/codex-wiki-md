<h1 id="10/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Model the uniformly wound air-core [solenoid](../../../../solenoid.md) as coaxial circular turns with [solenoid turn density](../../../../solenoid-turn-density.md) $n=N/L$. Put its ends at $x'=0,L$ and an internal axial point at $x\in[0,L]$. By the [superposition principle](../../../../superposition-principle.md), integrating the [on-axis magnetic field of a circular current loop](../../../../on-axis-magnetic-field-of-a-circular-current-loop.md) gives

$$
B(x)=\frac{\mu_0nIa^2}{2}\int_0^L\frac{dx'}{[a^2+(x-x')^2]^{3/2}}.
$$

Since $d[u/\sqrt{a^2+u^2}]/du=a^2/(a^2+u^2)^{3/2}$, this evaluates to the [on-axis magnetic field of a finite solenoid](../../../../on-axis-magnetic-field-of-a-finite-solenoid.md):

$$
B(x)=\frac{\mu_0NI}{2L}\left[
\frac{x}{\sqrt{a^2+x^2}}+
\frac{L-x}{\sqrt{a^2+(L-x)^2}}\right].
$$

The source's acute endpoint [angles](../../../../angle.md) satisfy $\cos\alpha=x/\sqrt{a^2+x^2}$ and $\cos\beta=(L-x)/\sqrt{a^2+(L-x)^2}$. Hence

$$
\boxed{B=\frac{\mu_0NI}{2L}(\cos\alpha+\cos\beta).}
$$

Although the paper calls this a “flux”, $B$ is [magnetic flux density](../../../../magnetic-field-split.md), measured in teslas. [Magnetic flux](../../../../magnetic-flux.md) is an [surface integral](../../../../surface-integral.md) $\Phi_B=\int\mathbf B\cdot d\mathbf A$, measured in webers, and cannot be assigned to a point. For example, two differently sized small disks at the same point have the same limiting $B$ but different [magnetic fluxes](../../../../magnetic-flux.md), approximately $B$ times their normal [areas](../../../../surface-area.md). The displayed plus sign uses the internal-point angle convention shown in the source. Outside the coil, the [integral](../../../../integral-split.md) expression still works, but one must retain signed axial projections rather than adding two acute-angle cosines.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [10](../../10.md)
3. [2021 resit](../../../2021-resit-split.md)
4. [Past exam of the physics 2 paper of the University of Oxford](../../../split.md)
5. [Physics 2 paper of the University of Oxford](../../../../physics-2-paper-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
