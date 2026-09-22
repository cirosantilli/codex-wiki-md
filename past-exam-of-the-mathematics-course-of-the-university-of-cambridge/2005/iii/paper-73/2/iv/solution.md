<h1 id="2/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

For a fixed $\mathrm{Re}\gg1$, optimize the gain over the initial wave tilt and a later observation time. From the [energy](../../../../../../energy.md) profile,

$$
\frac{d\log E}{dT}=-\frac{2T}{1+T^2}-\frac{1+T^2}{\mathrm{Re}}.
$$

Its stationary points satisfy

$$
-2\mathrm{Re}\,T=(1+T^2)^2.
$$

There are two negative roots in the high-Reynolds-number regime: an early [energy](../../../../../../energy.md) minimum and a later maximum. Write them as $T_-$ and $T_+$. Balancing the large-$|T|$ terms for the early root and the small-$|T|$ terms for the late root gives

$$
T_-=-(2\mathrm{Re})^{1/3}\bigl[1+O(\mathrm{Re}^{-2/3})\bigr],\qquad T_+=-\frac1{2\mathrm{Re}}+O(\mathrm{Re}^{-3}).
$$

Thus the optimum disturbance starts as a sufficiently tightly wound leading wave and reaches its peak slightly before $k_x=0$; finite [viscosity](../../../../../../dynamic-viscosity.md) shifts the peak away from the inviscid swing.

Normalize its initial [energy](../../../../../../energy.md) at $T_-$. The exact maximum ratio is

$$
G_{\max}=\frac{1+T_-^2}{1+T_+^2}\exp\!\left[\frac{g(T_-)-g(T_+)}{\mathrm{Re}}\right].
$$

The prefactor is asymptotic to $(2\mathrm{Re})^{2/3}$, while $g(T_-)/\mathrm{Re}\to-2/3$ and $g(T_+)/\mathrm{Re}\to0$. Therefore [optimal transient amplification of a viscous shearing wave](../../../../../../optimal-transient-amplification-of-a-viscous-shearing-wave.md) gives

$$
\boxed{G_{\max}\sim\left(\frac{2\mathrm{Re}}e\right)^{2/3},\qquad \mathrm{Re}=\frac A{\nu k_y^2}.}
$$

The time between the optimum initial tilt and the peak is approximately $(2\mathrm{Re})^{1/3}/(2A)$. Without [viscosity](../../../../../../dynamic-viscosity.md), ever larger initial tilts would allow unbounded gain; [viscosity](../../../../../../dynamic-viscosity.md) damps them before they can swing, selecting the finite optimum. The coefficient above uses the paper's [Reynolds number](../../../../../../reynolds-number.md) based on $A$, not one based on the full shear rate $2A$.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [2](../../2.md)
3. [Paper 73](../../../paper-73-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
