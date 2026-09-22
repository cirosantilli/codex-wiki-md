<h1 id="s31/2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let the step be $h$. Forward [Euler method](../../../../../euler-method.md) gives $x_1=x_0+hv_0$, $v_1=v_0+hF(x_0)$. Applying the same map with $-h$ gives $x_2=x_1-hv_1=x_0-h^2F(x_0)$, which generally differs from $x_0$. It is therefore not its own inverse under time reversal.

A kick–drift–kick [leapfrog integrator](../../../../../leapfrog-integration.md) instead has

$$
v_{1/2}=v_0+\frac h2F(x_0),\quad x_1=x_0+hv_{1/2},\quad v_1=v_{1/2}+\frac h2F(x_1).
$$

The step $-h$ first recovers $v_{1/2}$, then $x_0$, then $v_0$, so $\boxed{\Phi_{-h}=\Phi_h^{-1}}$. This assumes a position-dependent [force](../../../../../force-split.md) and the same fixed step. [Newtonian mechanics](../../../../../newtonian-mechanics-split.md) is reversible; respecting that structure helps avoid artificial directional bias and often improves long-term qualitative behaviour. The usual leapfrog also has a structure preserving [symplectic geometry](../../../../../symplectic-geometry-split.md), which supports bounded oscillatory [energy error](../../../../../energy-error.md), but reversibility by itself does not imply exact [conservation of energy](../../../../../conservation-of-energy.md). Adaptive stepping requires special care to preserve these properties.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [S31](../../../s31.md)
4. [2019](../../../../2019-split.md)
5. [Past exam of the short options paper shared by Parts A and B of the physics course of the University of Oxford](../../../../split.md)
6. [Short options paper shared by Parts A and B of the physics course of the University of Oxford](../../../../../short-options-paper-shared-by-parts-a-and-b-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
