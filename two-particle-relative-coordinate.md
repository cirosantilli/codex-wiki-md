# Two-particle relative coordinate

↑ **Parent:** [Reduced mass](reduced-mass.md)

Choose [positions](position.md) in one [inertial frame](inertial-frame.md) and let $M=m_1+m_2$. The [centre of mass](center-of-mass.md) and [two-particle relative coordinate](two-particle-relative-coordinate.md) are

$$
\mathbf R=\frac{m_1\mathbf r_1+m_2\mathbf r_2}{M},\qquad \mathbf r=\mathbf r_2-\mathbf r_1,\qquad
\mathbf r_1=\mathbf R-\frac{m_2}{M}\mathbf r,\quad \mathbf r_2=\mathbf R+\frac{m_1}{M}\mathbf r.
$$

The lighter body is farther from the [centre of mass](center-of-mass.md). Reconstructing both [positions](position.md) from these equations is part of solving the [two-body problem](two-body-problem.md); $\mathbf r$ alone describes their separation, not either body's laboratory [position](position.md).[Reduced Mass, equations 324–326: centre and reconstruction of both particle positions](newtonian-dynamics-by-richard-fitzpatrick.md)

<a id="image-reduced-mass-center-of-mass-relative-motion"></a>
![](reduced-mass-center-of-mass-relative-motion.png)

**[Figure 13](#image-reduced-mass-center-of-mass-relative-motion). Centre of mass translation and internal two-particle relative coordinate for a pair with mass ratio three**. Original illustrative [free two-mass spring](free-two-mass-spring.md) model, with $m_2=3m_1$, equilibrium separation $\ell$, relative extension $s/\ell=0.3\cos\tau$, $\tau=\omega t$, and $R/\ell=0.08\tau$. The right plot subtracts both the translating [centre of mass](center-of-mass.md) and each body's equilibrium offset. It shows internal [displacements](displacement.md), not full distances from the [centre of mass](center-of-mass.md).

Substitute the reconstructed [velocities](velocity.md) into the [kinetic energy](kinetic-energy.md). The result is the exact two-particle instance of [kinetic-energy decomposition about the centre of mass](kinetic-energy-decomposition-about-the-centre-of-mass.md):

$$
T=\frac12m_1|\dot{\mathbf r}_1|^2+\frac12m_2|\dot{\mathbf r}_2|^2
=\frac12M|\dot{\mathbf R}|^2+\frac12\mu|\dot{\mathbf r}|^2.
$$

The mixed [dot product](dot-product.md) has coefficient $-m_1m_2/M+m_2m_1/M=0$; the coefficient of $|\dot{\mathbf r}|^2$ is $(m_1m_2^2+m_2m_1^2)/M^2=\mu$. This algebra needs constant positive [masses](mass.md) but no particular [force](force-split.md) law. In the stationary [centre of mass](center-of-mass.md) frame, the fraction of internal [kinetic energy](kinetic-energy.md) carried by body 1 is $m_2/M$, and by body 2 is $m_1/M$: the lighter body carries more.

For a closed pair with no external [forces](force-split.md), write $\mathbf F$ for the [force](force-split.md) on body 2 and $-\mathbf F$ for that on body 1, as required by [Newton's third law](newton-s-third-law.md). Adding and subtracting their [Newton's second law](newton-s-second-law.md) equations yields

$$
M\ddot{\mathbf R}=\mathbf0,\qquad
\ddot{\mathbf r}=\left(\frac1{m_2}+\frac1{m_1}\right)\mathbf F,\qquad
\mu\ddot{\mathbf r}=\mathbf F.
$$

Thus the [centre of mass](center-of-mass.md) moves uniformly while the [two-particle relative coordinate](two-particle-relative-coordinate.md) behaves like one body of [reduced mass](reduced-mass.md). Equal-opposite internal [forces](force-split.md) suffice for these equations. For an internal [central force](central-force.md), $\mathbf F=f(r)\widehat{\mathbf r}$ with $r=|\mathbf r|>0$, the internal [torque](torque.md) vanishes and [conservation of angular momentum](conservation-of-angular-momentum.md) gives constant $\mathbf L_{\rm rel}=\mu\mathbf r\times\dot{\mathbf r}$. If the [central force](central-force.md) comes from a time-independent [potential energy](potential-energy.md) $U(r)$, then $f(r)=-dU/dr$ and the internal [mechanical energy](mechanical-energy.md) $E_{\rm rel}=\mu|\dot{\mathbf r}|^2/2+U(r)$ is conserved. The [kinetic energy](kinetic-energy.md) split alone does not establish either conservation law.

## ↑ Ancestors (6)

1. [Reduced mass](reduced-mass.md)
2. [Center of mass](center-of-mass.md)
3. [Classical mechanics](classical-mechanics-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Circular-orbit derivation of the Bohr model](circular-orbit-derivation-of-the-bohr-model.md)
- [Diatomic bond stretch](diatomic-bond-stretch.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2016/paper-2/section-b/b8/d/solution.md)
- [Reduced mass](reduced-mass.md)
- [Two-particle relative coordinate](two-particle-relative-coordinate.md)
