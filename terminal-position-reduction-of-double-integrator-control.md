# Terminal-position reduction of double-integrator control

↑ **Parent:** [Linear-quadratic-Gaussian control](linear-quadratic-gaussian-control.md)

For $dx=y\,dt$, $dy=u\,dt+dW$ and terminal cost $x(T)^2$ plus running cost $u^2$, the displayed change of state gives $dz=(T-t)u\,dt+(T-t)dW$. A quadratic value function has coefficient $P(t)=[1+(T-t)^3/3]^{-1}$ and additive noise cost $\log[1+(T-t)^3/3]$. Minimizing its [Hamilton-Jacobi-Bellman equation](hamilton-jacobi-bellman-equation.md) gives the displayed control. The gain is unchanged if the additive noise is removed, illustrating certainty equivalence.

## ↑ Ancestors (5)

1. [Linear-quadratic-Gaussian control](linear-quadratic-gaussian-control.md)
2. [Control theory](control-theory-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ii/paper-3/28i/solution.md)
