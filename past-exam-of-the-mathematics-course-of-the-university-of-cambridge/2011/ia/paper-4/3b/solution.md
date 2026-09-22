<h1 id="3b/solution">Solution</h1>

↑ **Parent:** [3B](../3b.md)

In a short time $dt$, the radius vector sweeps an oriented area $d\mathcal A=\tfrac12r^2d\theta$. Thus

$$
\boxed{\frac{d\mathcal A}{dt}=\frac h2.}
$$

The constant $h$ is twice the oriented [areal velocity](../../../../../areal-velocity.md), or the [angular momentum](../../../../../angular-momentum.md) per unit mass. Its constancy is [Kepler's second law](../../../../../kepler-s-second-law.md): equal areas are swept in equal times.

For a [circular orbit](../../../../../circular-orbit.md) of radius $a$, set $\ddot r=0$ in the radial equation. The balance is

$$
h^2=GMa,\qquad |\dot\theta|=\frac{|h|}{a^2}=\sqrt{\frac{GM}{a^3}}.
$$

Hence a [circular orbit](../../../../../circular-orbit.md) exists for any $a>0$ with this nonzero $|h|$. Its period gives [Kepler's third law](../../../../../kepler-s-third-law.md):

$$
\boxed{T=2\pi\sqrt{\frac{a^3}{GM}},\qquad T^2=\frac{4\pi^2a^3}{GM}.}
$$

To check [circular-orbit stability for a power-law central force](../../../../../circular-orbit-stability-for-a-power-law-central-force.md) directly, keep $h$ fixed and set $r=a+\rho$. Expanding

$$
\ddot r=\frac{h^2}{r^3}-\frac{GM}{r^2}
$$

about the balanced radius gives

$$
\ddot\rho=\left(-\frac{3h^2}{a^4}+\frac{2GM}{a^3}\right)\rho+O(\rho^2)
=-\frac{GM}{a^3}\rho+O(\rho^2).
$$

The linear radial perturbation therefore obeys

$$
\boxed{\ddot\rho+\Omega^2\rho=0,\qquad \Omega^2=GM/a^3>0.}
$$

It remains bounded and oscillates, proving stability under the stipulated small perturbations. Equivalently, the specific [effective potential](../../../../../effective-potential.md) $h^2/(2r^2)-GM/r$ has a strict minimum at $a$.

## ↑ Ancestors (10)

1. [3B](../3b.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ia](../../split.md)
4. [2011](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
