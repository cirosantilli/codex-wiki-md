# Double pendulum Lagrangian

↑ **Parent:** [Double pendulum](double-pendulum.md)

Choose [Cartesian coordinates](cartesian-coordinate-system.md) with origin at the upper pivot, $x$ to the right and $y$ upward. The two [position vectors](position-vector.md) are

$$
\mathbf r_1=\ell\begin{pmatrix}\sin\theta_1\\-\cos\theta_1\end{pmatrix},\qquad
\mathbf r_2=\ell\begin{pmatrix}\sin\theta_1+\sin\theta_2\\-\cos\theta_1-\cos\theta_2\end{pmatrix}.
$$

These expressions satisfy the rod [holonomic constraints](holonomic-constraint.md) $|\mathbf r_1|=\ell$ and $|\mathbf r_2-\mathbf r_1|=\ell$ automatically. This is the practical advantage of using the two [angles](angle.md) as coordinates: the rod [tensions](tension.md) need not be unknowns in the motion calculation.[Classical Dynamics, chapter 2, §2.3, printed pp. 17–19: elimination of ideal constraint forces using coordinates adapted to holonomic constraints](classical-dynamics-by-david-tong.md)

Differentiate these [position vectors](position-vector.md) to obtain the [velocities](velocity.md). The [dot product](dot-product.md) between their two rod contributions uses $\cos(\theta_1-\theta_2)=\cos\theta_1\cos\theta_2+\sin\theta_1\sin\theta_2$, giving

$$
|\dot{\mathbf r}_1|^2=\ell^2\dot\theta_1^2,\qquad
|\dot{\mathbf r}_2|^2=\ell^2\left(\dot\theta_1^2+\dot\theta_2^2+2\cos(\theta_1-\theta_2)\dot\theta_1\dot\theta_2\right).
$$

Adding the two [kinetic energies](kinetic-energy.md) and measuring [gravitational potential energy](gravitational-energy.md) from the downward [equilibrium](equilibrium-point-of-a-dynamical-system.md) gives

$$
\begin{aligned}
T&=\frac{m\ell^2}{2}\left(2\dot\theta_1^2+\dot\theta_2^2+2\cos(\theta_1-\theta_2)\dot\theta_1\dot\theta_2\right),\\
V&=mg\ell\left[2(1-\cos\theta_1)+(1-\cos\theta_2)\right],\\
L&=T-V.
\end{aligned}
$$

The coefficient $2$ has a geometric meaning: the upper rod raises both [masses](mass.md), and its motion contributes to both [kinetic energies](kinetic-energy.md). The coupling in $T$ is present because the lower [mass](mass.md) has a moving pivot. The zero chosen for $V$ changes $L$ by a constant and leaves the [Euler-Lagrange equations](euler-lagrange-equation.md) unchanged.[Classical Dynamics, chapter 2, §2.5.2, printed p. 28, equations (2.68)–(2.72): general point-mass double pendulum; the derivation here specializes to equal masses and lengths and uses upward $y$](classical-dynamics-by-david-tong.md)

The [principle of stationary action](principle-of-stationary-action.md) applies to $S=\int L\,dt$. Its fixed-endpoint [first variation](first-variation.md), after [integration by parts](integration-by-parts.md), is

$$
\delta S=\int\sum_{i=1}^2\left(\frac{\partial L}{\partial\theta_i}-\frac{d}{dt}\frac{\partial L}{\partial\dot\theta_i}\right)\delta\theta_i\,dt.
$$

Independent allowed variations therefore give one [Euler-Lagrange equation](euler-lagrange-equation.md) for each [angle](angle.md). Stationary [action](action.md) alone does not assert a minimum.[Classical Dynamics, chapter 2, §2.1, printed pp. 10–12, equations (2.2)–(2.8) and the stationary-action qualification](classical-dynamics-by-david-tong.md)

## ↑ Ancestors (6)

1. [Double pendulum](double-pendulum.md)
2. [Lagrangian mechanics](lagrangian-mechanics-split.md)
3. [Classical mechanics](classical-mechanics-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Double pendulum](double-pendulum.md)
- [Double pendulum equations of motion](double-pendulum-equations-of-motion.md)
