# Weak focus of an exponential polynomial planar system

↑ **Parent:** [Weak focus](weak-focus.md)

This real planar [dynamical system](dynamical-system.md) has a [saddle point](saddle-point.md) at $(-1,0)$ and a repelling [weak focus](weak-focus.md) at $(1,0)$. The latter has purely imaginary linearized [eigenvalues](eigenvalue.md) $\pm2i$, so its [linearization](linearization.md) has closed elliptical orbits. Nonlinear terms nevertheless produce outward drift.

Set $X=2(x-1)$, $Y=y$, $\tau=2t$ and $r^2=X^2+Y^2$. The cubic expansion is

$$
X_\tau=Y+Y^2+\tfrac12XY^2+\tfrac12Y^3+O(r^4),\qquad
Y_\tau=-X-\tfrac34X^2-\tfrac12Y^2-\tfrac14X^3+O(r^4).
$$

The linear rotation acts on scalar functions by $L=Y\partial_X-X\partial_Y$. For $H_2=r^2/2$, its cubic derivative is $XY^2-3X^2Y/4-Y^3/2$. The homogeneous correction $H_3=7X^3/12+XY^2/2+Y^3/3$ satisfies $LH_3$ equal to the negative of that derivative. The remaining quartic derivative of $H_2+H_3$ is $3X^2Y^2/2-X^3Y$. With

$$
H_4=\tfrac14X^4-\tfrac3{16}X^3Y+\tfrac3{16}XY^3,
$$

direct differentiation gives

$$
\frac d{d\tau}(H_2+H_3+H_4)=\tfrac3{16}r^4+O(r^5)>0
$$

for all sufficiently small nonzero $r$. Meanwhile $H_2+H_3+H_4=r^2/2+O(r^3)>0$. In reversed time it is a strict [Lyapunov function](lyapunov-function.md), proving asymptotic stability of the reversed system and hence repulsion forward in time. The angular speed stays close to $-1$, so the nearby nonzero trajectories spiral rather than approaching along a fixed direction. This explicit calculation illustrates why [a centre in the linearization need not be a nonlinear centre](a-centre-in-the-linearization-need-not-be-a-nonlinear-centre.md).

## ↑ Ancestors (6)

1. [Weak focus](weak-focus.md)
2. [Nonhyperbolic equilibrium](nonhyperbolic-equilibrium.md)
3. [Dynamical systems](dynamical-systems-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-algebra-analysis-and-differential-equations-1-course-of-the-university-of-oxford/2005/7/solution.md)
