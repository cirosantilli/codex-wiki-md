# Exact Lagrangian of two spring-coupled pendulums

↑ **Parent:** [Simple pendulum](simple-pendulum-split.md)

Two identical planar [simple pendulums](simple-pendulum-split.md) of length $l$ and bob [mass](mass.md) $m$, with pivots separated horizontally by $r>0$, are coupled by a straight [spring](spring.md) of natural length $r$ and [spring constant](spring-constant.md) $k$. In the ideal model without contact restrictions, their [configuration space](mechanical-configuration-space.md) is the [torus](torus.md) $S^1\times S^1$. Measure both [angles](angle.md) from the downward vertical towards the same horizontal direction. Their bob separation is

$$
d=\sqrt{\bigl(r+l(\sin\theta_2-\sin\theta_1)\bigr)^2+l^2(\cos\theta_2-\cos\theta_1)^2}.
$$

The exact [Lagrangian](lagrangian.md) is the expression in the title. To derive it, use bob [positions](position.md) $(l\sin\theta_1,-l\cos\theta_1)$ and $(r+l\sin\theta_2,-l\cos\theta_2)$. [Kinetic energy from Cartesian position vectors](kinetic-energy-from-cartesian-position-vectors.md) gives $T=ml^2(\dot\theta_1^2+\dot\theta_2^2)/2$. Gravitational [potential energy](potential-energy.md) is $-mgl(\cos\theta_1+\cos\theta_2)$ and [spring](spring.md) [potential energy](potential-energy.md) is $k(d-r)^2/2$; subtracting these from $T$ proves the formula. Near the downward [equilibrium](equilibrium-point-of-a-dynamical-system.md), $d-r=l(\theta_2-\theta_1)+O(|\boldsymbol\theta|^3)$ for fixed $r$, giving the familiar [normal modes of two spring-coupled equal pendulums](normal-modes-of-two-spring-coupled-equal-pendulums.md).

## ↑ Ancestors (5)

1. [Simple pendulum](simple-pendulum-split.md)
2. [Classical mechanics](classical-mechanics-split.md)
3. [Branches of physics](branches-of-physics.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-classical-mechanics-course-of-the-university-of-oxford/2023/1/a/solution.md)
