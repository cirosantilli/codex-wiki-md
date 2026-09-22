<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Use [pressure](../../../../../pressure.md) with the ambient [hydrostatic pressure](../../../../../hydrostatic-pressure.md) removed, and let $\Delta P$ be the [pressure](../../../../../pressure.md) below the falling [sphere](../../../../../sphere.md) minus that above it. Away from the [sphere](../../../../../sphere.md) the tube flow is [Hagen-Poiseuille flow](../../../../../hagen-poiseuille-equation.md). The upper and lower clear lengths add to $L$ to leading order in $a/L$, so their [pressure](../../../../../pressure.md) drops add:

$$
\boxed{Q=\frac{\pi a^4\Delta P}{8\mu L}.}
$$

The large exterior reservoir returns this flux with negligible [pressure](../../../../../pressure.md) loss compared with the long narrow tube. The [sphere](../../../../../sphere.md) is assumed far enough from the ends that entrance effects and its occupied length give only lower-order corrections.

Now use a frame translating downwards with the [sphere](../../../../../sphere.md), and take $z$ positive upwards from its center. The [sphere](../../../../../sphere.md) is stationary and the tube wall moves upwards with speed $U$. The narrow gap is

$$
h(z)=a-\sqrt{a^2(1-\epsilon/2)^2-z^2}\simeq\frac a2\left[\epsilon+(z/a)^2\right].
$$

It has axial length scale $a\sqrt\epsilon$, making [lubrication theory](../../../../../lubrication-theory.md) appropriate. The [sphere-frame flux in a tube](../../../../../sphere-frame-flux-in-a-tube.md) is constant: the upward relative flux through the whole section is $\pi a^2U-Q$, so its flux per unit circumference is

$$
\boxed{q=\frac{\pi a^2U-Q}{2\pi a}.}
$$

With $y=0$ on the [sphere](../../../../../sphere.md) and $y=h$ on the wall, [Couette-Poiseuille flow in a thin gap](../../../../../couette-poiseuille-flow-in-a-thin-gap.md) gives

$$
u(y)=\frac{p_z}{2\mu}y(y-h)+\frac{Uy}{h},\qquad q=-\frac{h^3p_z}{12\mu}+\frac{Uh}{2},\qquad p_z=\frac{6\mu U}{h^2}-\frac{12\mu q}{h^3}.
$$

Since $\Delta P=-\int p_z\,dz$, the pressure-jump relation is

$$
\boxed{\frac{\Delta P}{6\mu}=2qI_3-UI_2,\qquad I_n=\int_{-\infty}^{\infty}\frac{dz}{h(z)^n}.}
$$

The parabolic inner gap can be extended to infinite $z$ because these integrals are dominated by $|z|=O(a\sqrt\epsilon)$. The [lubrication resistance integrals for a nearly occluding sphere](../../../../../lubrication-resistance-integrals-for-a-nearly-occluding-sphere.md) are

$$
I_n=2^n a^{1-n}\epsilon^{1/2-n}J_n,\qquad J_n=\int_{-\infty}^{\infty}(1+\xi^2)^{-n}\,d\xi.
$$

Setting $\xi=\tan\theta$ evaluates $J_1=\pi$, $J_2=\pi/2$, $J_3=3\pi/8$, hence

$$
\boxed{I_1=2\pi\epsilon^{-1/2},\quad I_2=\frac{2\pi}{a}\epsilon^{-3/2},\quad I_3=\frac{3\pi}{a^2}\epsilon^{-5/2}.}
$$

For the [force](../../../../../force.md), enclose the fluid between sections just above and below the [sphere](../../../../../sphere.md), including the annular layer. The net upward [pressure](../../../../../pressure.md) [force](../../../../../force.md) is $\pi a^2\Delta P$. The tube wall exerts upward shear traction $\mu u_y(h)$ on this fluid; the [sphere](../../../../../sphere.md) exerts a downward [force](../../../../../force.md) equal to the upward hydrodynamic [force](../../../../../force.md) $F$ on itself. From the gap solution,

$$
u_y(h)=\frac{p_zh}{2\mu}+\frac Uh=\frac{4U}{h}-\frac{6q}{h^2}.
$$

The axial [control volume](../../../../../control-volume.md) [force](../../../../../force.md) balance therefore gives the [control-volume drag formula for a sphere in a tube](../../../../../control-volume-drag-formula-for-a-sphere-in-a-tube.md):

$$
\boxed{F=\pi a^2\Delta P+2\pi a\mu(4UI_1-6qI_2).}
$$

Using a [control volume](../../../../../control-volume.md) avoids having to integrate the curved-sphere normal [pressure](../../../../../pressure.md) and tangential shear separately.

With $Q^*=Q/(\pi a^2U)$, $\Delta P^*=a\Delta P/(6\mu U)$, $q^*=2q/(aU)$, $F^*=F/(6\pi\mu aU)$, $I_n^*=a^{n-1}I_n$ and $L^*=4L/(3a)$, the three flux/[pressure](../../../../../pressure.md) equations become

$$
Q^*=\frac{\Delta P^*}{L^*},\qquad\Delta P^*=q^*I_3^*-I_2^*,\qquad q^*=1-Q^*.
$$

Solving these linear relations gives

$$
\boxed{Q^*=\frac{I_3^*-I_2^*}{L^*+I_3^*},\qquad q^*=\frac{L^*+I_2^*}{L^*+I_3^*},\qquad\Delta P^*=\frac{L^*(I_3^*-I_2^*)}{L^*+I_3^*}.}
$$

The [force](../../../../../force.md) relation is $F^*=\Delta P^*+\tfrac43I_1^*-q^*I_2^*$. Substitution first yields

$$
F^*=\frac{L^*I_3^*-2L^*I_2^*+\tfrac43L^*I_1^*+\tfrac43I_1^*I_3^*-(I_2^*)^2}{L^*+I_3^*}.
$$

Because $I_2^*/I_3^*=2\epsilon/3$ and $I_1^*/I_3^*=2\epsilon^2/3$, the terms $-2L^*I_2^*$ and $\tfrac43L^*I_1^*$ are lower order than $L^*I_3^*$. Keeping the uniformly relevant leading terms gives

$$
\boxed{F^*\simeq\frac{L^*I_3^*+\tfrac43I_1^*I_3^*-(I_2^*)^2}{L^*+I_3^*}=\frac{3\pi L^*\epsilon^{-5/2}+4\pi^2\epsilon^{-3}}{L^*+3\pi\epsilon^{-5/2}}.}
$$

The squared $I_2^*$ is essential; replacing it by $I_2^*I_3^*$ would give the wrong sign and scaling. This establishes the [three drag regimes for a nearly occluding sphere](../../../../../three-drag-regimes-for-a-nearly-occluding-sphere.md).

For $L^*\ll\epsilon^{-1/2}$,

$$
\boxed{F^*\sim\frac{4\pi}{3}\epsilon^{-1/2},\quad Q^*\sim1,\quad q^*\sim\frac23\epsilon,\quad\Delta P^*\sim L^*,\quad\frac{F^*}{\Delta P^*}\gg1.}
$$

The [sphere](../../../../../sphere.md) nearly carries the tube's fluid down with it: the far-field flux is close to the piston displacement rate. The relative annular leakage is small in total volume, and the dominant [force](../../../../../force.md) comes from the local annular shear term. The [pressure](../../../../../pressure.md) [force](../../../../../force.md) associated with the overall tube resistance is smaller.

For $\epsilon^{-1/2}\ll L^*\ll\epsilon^{-5/2}$,

$$
\boxed{F^*\sim L^*,\quad\Delta P^*\sim L^*,\quad Q^*\sim1,\quad q^*\simeq\frac23\epsilon+\frac{L^*\epsilon^{5/2}}{3\pi}\ll1,\quad\frac{F^*}{\Delta P^*}\sim1.}
$$

The flow remains approximately piston-like, but the dominant [force](../../../../../force.md) is now the [pressure](../../../../../pressure.md) needed to drive [Hagen-Poiseuille flow](../../../../../hagen-poiseuille-equation.md) through the long clear tube. Both displayed terms in $q^*$ are retained because their relative size changes inside this regime without producing an additional leading drag regime.

For $L^*\gg\epsilon^{-5/2}$,

$$
\boxed{F^*\sim\Delta P^*\sim3\pi\epsilon^{-5/2},\quad Q^*\sim\frac{3\pi\epsilon^{-5/2}}{L^*}\ll1,\quad q^*\sim1,\quad\frac{F^*}{\Delta P^*}\sim1.}
$$

The large tube resistance makes its net through-flow negligible. The [sphere](../../../../../sphere.md)'s displaced fluid instead passes upwards relative to it through the thin annular gap, with gap [velocity](../../../../../velocity.md) of order $U/\epsilon$. Its [pressure](../../../../../pressure.md) drop and resulting [pressure](../../../../../pressure.md) [force](../../../../../force.md) dominate.

Finally consider two identical co-moving [spheres](../../../../../sphere.md), with nonoverlapping lubrication regions and the same total clear-tube length to leading order. The common through-flux is not doubled. In the middle regime it is still approximately $\pi a^2U$, so the same total tube [pressure](../../../../../pressure.md) drop is shared equally between the two identical [spheres](../../../../../sphere.md). The [load sharing between co-moving spheres in a tube](../../../../../load-sharing-between-co-moving-spheres-in-a-tube.md) gives **half the single-sphere [force](../../../../../force.md) on each [sphere](../../../../../sphere.md) in regime (ii)**. In regime (i), drag is set locally by the nearly pressure-balanced annular shear and is unchanged on each [sphere](../../../../../sphere.md). In regime (iii), each [sphere](../../../../../sphere.md) must pass essentially its own displacement flux through its annular gap, giving the same local [pressure](../../../../../pressure.md) drag as before; adding another [pressure](../../../../../pressure.md) jump changes the already small tube flux but not either leading drag. **The [force](../../../../../force.md) is unchanged in regimes (i) and (iii).**

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 73](../../paper-73-split.md)
3. [Iii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
