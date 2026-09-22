# Sphere-plane capacitance

↑ **Parent:** [Capacitance](capacitance.md)

For a conducting sphere of radius $R$ at center height $h>R$ above a grounded infinite plane,

$$
C(R,h)=4\pi\epsilon R\sinh\alpha\sum_{n=1}^{\infty}\frac1{\sinh(n\alpha)},
\qquad\cosh\alpha=\frac hR.
$$

The distance $h$ is measured to the center, so the surface gap is $h-R$. Relative to the [capacitance of an isolated conducting sphere](capacitance-of-an-isolated-conducting-sphere.md), the enhancement is $c(R/h)=C(R,h)/(4\pi\epsilon R)$.

The [method of images](method-of-images.md) gives a constructive proof. At fixed sphere potential $V_s$, start with $q_0=4\pi\epsilon RV_s$ at height $z_0=h$ and place its opposite image below the plane. Cancel that image's nonconstant sphere potential by the successive charges

$$
q_{n+1}=\frac R{h+z_n}q_n,
\qquad z_{n+1}=h-\frac{R^2}{h+z_n},
$$

with opposite mirror charges below the plane at every step. The resulting sphere potential is $V_s$ and the plane potential is zero. Since $q_n=4\pi\epsilon RV_s\sinh\alpha/\sinh((n+1)\alpha)$, summing the sphere charges gives the displayed [capacitance](capacitance.md). In particular $c(y)=1+y/2+O(y^2)$ for small $y$.

The exact sphere-plane boundary-value problem is also treated in [Behunin and colleagues' analysis of sphere-plane electrostatics](https://arxiv.org/abs/1206.6034).

## ↑ Ancestors (5)

1. [Capacitance](capacitance.md)
2. [Electromagnetism](electromagnetism-split.md)
3. [Branches of physics](branches-of-physics.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Droplet evaporation near a planar reservoir](droplet-evaporation-near-a-planar-reservoir.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-344/3/e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-344/3/f/solution.md)
