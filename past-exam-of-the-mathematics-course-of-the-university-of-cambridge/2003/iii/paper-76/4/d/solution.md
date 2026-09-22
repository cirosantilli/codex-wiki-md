<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Assume quasi-steady saturated [Darcy flow](../../../../../../darcy-flow.md), hydrostatic pore pressure, a long shallow barrier, isotropic intrinsic [permeability of a porous medium](../../../../../../permeability-of-a-porous-medium.md) $k$, an impermeable lined base, and negligible capillarity. Maintain upstream and downstream free-surface heads at $H$ and $\eta<H$. The [Dupuit approximation](../../../../../../dupuit-approximation.md) neglects vertical velocity except in small entrance/exit regions. Let $\mu$ be the fluid's dynamic viscosity and $K=k\rho g/\mu=k g/\nu$ its hydraulic conductivity.

Since the pressure is $p=\rho g(h(x)-z)$, the superficial [Darcy velocity](../../../../../../darcy-velocity.md) is $v_D=-K h_x$, uniform with depth at fixed $x$. Integrating over the printed channel width gives

$$
Q=-K A(h)h_x=-\frac{\alpha K}{3}h^3h_x.
$$

The steady discharge is constant, so integration with the two head boundary values gives [Dupuit flow in a channel with cubic wetted area](../../../../../../dupuit-flow-in-a-channel-with-cubic-wetted-area.md):

$$
\boxed{h(x)=\left[H^4-(H^4-\eta^4)\frac xL\right]^{1/4},\qquad
Q=\frac{\alpha k\rho g}{12\mu L}(H^4-\eta^4).}
$$

Here $Q$ is total volume per time, including the changing channel width. The pore-space mean speed is $v_p=v_D/\phi=Q/[\phi A(h)]$. Thus [porosity](../../../../../../porosity.md) affects storage and pore transit time but does not separately multiply this steady discharge when $k$ is the intrinsic permeability in [Darcy's law](../../../../../../darcy-law.md). If “permeability” is instead supplied as hydraulic conductivity, use that value directly for $K$. An exact seepage-face/free-boundary calculation near the outlet would go beyond the shallow Dupuit model.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [4](../../4.md)
3. [Paper 76](../../../paper-76-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
