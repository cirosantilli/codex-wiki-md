# Logistic predator-prey model

↑ **Parent:** [Lotka-Volterra predator-prey model](lotka-volterra-predator-prey-model.md)

This [Lotka-Volterra predator-prey model](lotka-volterra-predator-prey-model.md) includes self-limitation of the prey through the term $-bx^2$, with positive constants $a,b,c,d,e$. A positive coexistence [equilibrium point](equilibrium-point-of-a-dynamical-system.md) exists when $a>be/d$, at $x_*=e/d$, $y_*=(a-bx_*)/c$. The [Lyapunov function](lyapunov-function.md)

$$
V=d[x-x_*-x_*\log(x/x_*)]
+c[y-y_*-y_*\log(y/y_*)]
$$

satisfies $\dot V=-bd(x-x_*)^2$: its predator-prey cross terms cancel. Its sublevel sets are compact in the positive quadrant. The only invariant subset of $\{\dot V=0\}$ is the coexistence [equilibrium point](equilibrium-point-of-a-dynamical-system.md), because staying on $x=x_*$ requires $y=y_*$. The [LaSalle invariance principle](lasalle-s-invariance-principle.md) therefore proves convergence to coexistence for every positive initial state.

**Table of contents**

- [Quadratic discrete predator-prey map](quadratic-discrete-predator-prey-map.md)

## ↑ Ancestors (5)

1. [Lotka-Volterra predator-prey model](lotka-volterra-predator-prey-model.md)
2. [Mathematical biology](mathematical-biology-split.md)
3. [Branches of physics](branches-of-physics.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/ia/paper-2/8b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ia/paper-2/6c/a/solution.md)
