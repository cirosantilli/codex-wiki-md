<h1 id="7d/solution">Solution</h1>

↑ **Parent:** [7D](../7d.md)

For constant fluid density $\rho$, steady [Euler equations for an inviscid fluid](../../../../../euler-equations-for-an-inviscid-fluid.md) under a [conservative force](../../../../../conservative-force.md) per unit mass $-\nabla\Phi$ read $(\mathbf u\cdot\nabla)\mathbf u=-\nabla p/\rho-\nabla\Phi$. Here $\mathbf u$ is velocity, $p$ pressure and $\Phi$ potential per unit mass. Dotting with $\mathbf u$ gives

$$
\mathbf u\cdot\nabla\left(\frac12|\mathbf u|^2+\frac p\rho+\Phi\right)=0,
\qquad \boxed{\frac12|\mathbf u|^2+\frac p\rho+\Phi=\text{constant along each streamline}.}
$$

This is the [Bernoulli equation](../../../../../bernoulli-equation.md). The constants can differ between [streamlines](../../../../../streamline.md). If density varies, the same derivation for a [barotropic fluid](../../../../../barotropic-fluid.md) replaces $p/\rho$ by $\int^p dp'/\rho(p')$; constant density is the appropriate water approximation here.

For the draining cone, the radius at height $h$ is $h$ and the horizontal area is $\pi h^2$. Both the free surface and the jet are at atmospheric pressure; their gravitational potential difference is approximately $gh$. The speed of the descending surface is smaller than the jet speed by the area ratio $\epsilon^2/h^2$, so it can be neglected when $h\gg\epsilon$. The [Bernoulli equation](../../../../../bernoulli-equation.md) then gives [Torricelli's law](../../../../../torricelli-s-law.md), $U\simeq\sqrt{2gh}$. [Conservation of mass](../../../../../mass-conservation.md) gives

$$
\pi h^2\dot h\simeq-\pi\epsilon^2\sqrt{2gh},\qquad
h(t)^{5/2}\simeq h_0^{5/2}-\frac52\epsilon^2\sqrt{2g}\,t.
$$

Hence the leading [drainage time of a conical tank](../../../../../drainage-time-of-a-conical-tank.md) is

$$
\boxed{T\simeq\frac{2h_0^{5/2}}{5\epsilon^2\sqrt{2g}}=\left(\frac{2h_0^5}{25\epsilon^4g}\right)^{1/2}.}
$$

Removing the tip places the aperture at height of order $\epsilon$, and the quasi-steady calculation fails in the last layer of that depth. Integrating down only to $h=O(\epsilon)$ changes the displayed leading time by relative order $(\epsilon/h_0)^{5/2}$; replacing the actual head $h-\epsilon$ by $h$ introduces a larger, but still vanishing, relative correction of order $\epsilon/h_0$. The formula is the ideal inviscid estimate under the question's stated approximation, not an exact law for the final transient or a real contracted jet.

## ↑ Ancestors (10)

1. [7D](../7d.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
