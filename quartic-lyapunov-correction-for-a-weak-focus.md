# Quartic Lyapunov correction for a weak focus

↑ **Parent:** [Weak focus](weak-focus.md)

Consider a smooth planar system $\dot x=y+P_3(x,y)+O(r^5)$, $\dot y=-x+Q_3(x,y)+O(r^5)$, where $P_3,Q_3$ are homogeneous cubic [polynomials](polynomial-split.md) and $r^2=x^2+y^2$. The leading [derivative](derivative.md) of $r^2/2$ is the quartic [polynomial](polynomial-split.md) $H_4=xP_3+yQ_3$. Let $\kappa$ be the angular average of $H_4$ on the unit circle. A homogeneous quartic correction $V_4$ solving

$$
(y\partial_x-x\partial_y)V_4=\kappa r^4-H_4
$$

gives $\dot V=\kappa r^4+O(r^6)$ for $V=r^2/2+V_4$. The right side has zero angular average. Since $y\partial_x-x\partial_y=-\partial_\theta$, its nonconstant angular Fourier modes can be integrated individually to obtain a periodic quartic correction; only modes of orders two and four can occur after removing the constant average.

The correction is $O(r^4)$, so $V$ remains positive definite close to zero. If $\kappa<0$, its orbital [derivative](derivative.md) is strictly negative there, and the [Second Lyapunov theorem](second-lyapunov-theorem.md) proves [asymptotic stability](asymptotic-stability.md). If $\kappa>0$, apply the same argument in reversed time to obtain repulsion. If $\kappa=0$, this quartic calculation alone does not decide stability. This method converts the averaged damping of a [weak focus](weak-focus.md) into a pointwise sign for a [Lyapunov function](lyapunov-function.md).

## ↑ Ancestors (6)

1. [Weak focus](weak-focus.md)
2. [Nonhyperbolic equilibrium](nonhyperbolic-equilibrium.md)
3. [Dynamical systems](dynamical-systems-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-algebra-analysis-and-differential-equations-2-course-of-the-university-of-oxford/2012/7/c/solution.md)
