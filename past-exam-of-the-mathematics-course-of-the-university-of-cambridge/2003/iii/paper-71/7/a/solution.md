<h1 id="7/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Model the [polymerization Brownian ratchet](../../../../../../polymerization-brownian-ratchet.md) by a rigid tip and a Brownian load. Let $a$ be the elementary load advance, $\zeta_L$ its drag coefficient, and $D=k_BT/\zeta_L$ its [diffusion coefficient](../../../../../../diffusion-coefficient.md). For a spherical load, $\zeta_L=6\pi\mu R_L$, but no load radius is specified, so the rate is naturally expressed in terms of $D$. Assume addition is effectively instantaneous once the gap $h$ reaches $a$, and removal is negligible. The gap reflects at zero, first arrival at $a$ causes insertion, and insertion resets it to zero.

With no opposing [force](../../../../../../force.md), the mean [first-passage time](../../../../../../first-passage-time.md) satisfies $DT''=-1$, $T'(0)=0$, $T(a)=0$. Integration gives $T(h)=(a^2-h^2)/(2D)$. One advance per passage gives

$$
\boxed{T(0)=\frac{a^2}{2D},\qquad V_0=\frac a{T(0)}=\frac{2D}{a}.}
$$

The advance-event rate is $2D/a^2$, while $V_0$ is a length per time.

A constant resisting [force](../../../../../../force.md) $F\ge0$ produces drift $-u_F=-DF/(k_BT)$. The [diffusion-limited Brownian ratchet with constant load](../../../../../../diffusion-limited-brownian-ratchet-with-constant-load.md) now satisfies

$$
DT''-u_FT'=-1,\qquad T'(0)=0,\quad T(a)=0.
$$

An integrating factor gives $T'(h)=[1-e^{u_Fh/D}]/u_F$. Integrating again from $h$ to $a$ gives $T(0)=D(e^z-1-z)/u_F^2$, where $z=Fa/(k_BT)$. Therefore

$$
\boxed{V(F)=\frac Da\frac{z^2}{e^z-1-z},\qquad \frac{V(F)}{V_0}=\frac{z^2}{2(e^z-1-z)}.}
$$

At weak load the ratio is $1-z/3+O(z^2)$; at large load $V\sim(D/a)z^2e^{-z}$. Replacing the whole [force](../../../../../../force.md) dependence by $e^{-z}$ would discard the first-passage kinetics of this regime.

For two staggered strands that alternately advance the leading tip by half a monomer, $a=\delta/2$ and $V_0=4D/\delta$. Two aligned strands, as schematically drawn, do not automatically have that half-step: an advance may be $a=\delta$, with the other strand filling the same layer afterward. Use the same geometrical step in the passage problem and in converting event rate to [velocity](../../../../../../velocity.md). The limiting formula assumes negligible removal, rigid tips, an overdamped load with constant drag, and fast insertion compared with $a^2/D$. With appreciable removal or additional internal strand states, the renewal reset model must be replaced by a coupled gap/reaction process.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [7](../../7.md)
3. [Paper 71](../../../paper-71-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
