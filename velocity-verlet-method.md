# Velocity Verlet method

↑ **Parent:** [Numerical method](numerical-method.md)

For an [ordinary differential equation](ordinary-differential-equation.md) $\ddot x=f(x,t)$ with [acceleration](acceleration.md) independent of [velocity](velocity.md), the [velocity Verlet method](velocity-verlet-method.md) advances [position](position.md) and [velocity](velocity.md) by

$$
a_n=f(x_n,t_n),\qquad x_{n+1}=x_n+h v_n+\frac{h^2}{2}a_n,\qquad
v_{n+1}=v_n+\frac h2\bigl(a_n+f(x_{n+1},t_n+h)\bigr).
$$

Here $h$ is the time step and $t_{n+1}=t_n+h$. For sufficiently smooth $f$, the [global error](global-discretization-error.md) on a fixed time interval is $O(h^2)$, so halving $h$ reduces the leading [global error](global-discretization-error.md) by a factor of four once the asymptotic regime is reached.

## ↑ Ancestors (6)

1. [Numerical method](numerical-method.md)
2. [Numerical analysis](numerical-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Paul trap secular-motion example](paul-trap-secular-motion-example.md)
- [Velocity Verlet method](velocity-verlet-method.md)
