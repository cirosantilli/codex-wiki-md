# Overdamping

↑ **Parent:** [Damping](damping.md)

For $\zeta>1$, let $r_+>r_-$ be the real [characteristic roots](characteristic-root-of-a-constant-coefficient-differential-equation.md). The response with the specified [initial conditions](initial-condition.md) is

$$
x(t)=C_+e^{r_+t}+C_-e^{r_-t},\qquad
C_+=\frac{v_0-r_-x_0}{r_+-r_-},\quad C_-=\frac{r_+x_0-v_0}{r_+-r_-}.
$$

The generic late response is governed by $r_+$, the root nearer zero. For very large [damping ratio](damping-ratio.md), $r_+\sim-\omega_0/(2\zeta)=-k/b$: an increasingly strong brake delays the return to [equilibrium](equilibrium-point-of-a-dynamical-system.md). This approximation comes from balancing the [spring](spring.md) and [viscous damping](viscous-damping.md) terms after the fast transient. Choosing $v_0=r_-x_0$ makes $C_+=0$ and leaves only the faster root; that exception requires different initial [velocities](velocity.md) as $b$ varies.

## ↑ Ancestors (7)

1. [Damping](damping.md)
2. [Wave equation](wave-equation-split.md)
3. [Partial differential equation](partial-differential-equation-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Damping](damping.md)
- [Damping measurement from free decay](damping-measurement-from-free-decay.md)
- [Damping ratio](damping-ratio.md)
