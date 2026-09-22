<h1 id="18a/solution">Solution</h1>

↑ **Parent:** [18A](../18a.md)

[Irrotational flow](../../../../../irrotational-flow.md) permits $\mathbf u=\nabla\phi$, and [incompressible flow](../../../../../incompressible-flow.md) imposes $\nabla\cdot\mathbf u=0$, hence $\Delta\phi=0$. In the laboratory frame, the no-penetration condition at the translating sphere is $\partial_r\phi(a,\theta)=U\cos\theta$.

For [separation of variables](../../../../../separation-of-variables.md), take the angular factor $g(\theta)=\cos\theta$, which satisfies $\frac{1}{\sin\theta}(\sin\theta\,g')'=-2g$. The radial equation is

$$
(r^2f')'-2f=0,
$$

with solutions $r$ and $r^{-2}$. Rest at infinity excludes the $r$ term. The normal boundary condition fixes the remaining coefficient, giving the [potential flow around a translating sphere](../../../../../potential-flow-around-a-translating-sphere.md)

$$
\boxed{\phi=-\frac{Ua^3\cos\theta}{2r^2},\qquad \mathbf u=\frac{Ua^3}{r^3}\cos\theta\,\mathbf e_r+\frac{Ua^3}{2r^3}\sin\theta\,\mathbf e_\theta.}
$$

There is no azimuthal velocity. With fluid density $\rho_f$, the [kinetic energy](../../../../../kinetic-energy.md) is

$$
K_f=\frac{\rho_fU^2a^6}{2}\int_a^\infty r^{-4}dr\int_0^{2\pi}\int_0^\pi\left(\cos^2\theta+\frac14\sin^2\theta\right)\sin\theta\,d\theta\,d\varphi.
$$

The angular integral is $2\pi$, and the radial integral is $1/(3a^3)$, so $K_f=\rho_f\pi a^3U^2/3$. Since $M=(4\pi a^3/3)\rho_s$ and $k=\rho_f/\rho_s$, **$K_f=kMU^2/4$**. Thus the [added mass of a sphere](../../../../../added-mass-of-a-sphere.md) is $kM/2$.

During a fall through $h$, gravity does work $Mgh$ and [buoyancy](../../../../../buoyancy.md) does work $-kMgh$. Starting from rest, [conservation of energy](../../../../../conservation-of-energy.md) gives

$$
M(1-k)gh=\frac12MU^2+\frac{kMU^2}{4}.
$$

Consequently **$U=\sqrt{4(1-k)gh/(2+k)}$**. The mass cancels: the reduced speed comes from both [buoyancy](../../../../../buoyancy.md) and the fluid's [added mass](../../../../../added-mass.md).

## ↑ Ancestors (10)

1. [18A](../18a.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
