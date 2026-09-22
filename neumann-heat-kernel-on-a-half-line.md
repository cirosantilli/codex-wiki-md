# Neumann heat kernel on a half-line

↑ **Parent:** [Heat kernel](heat-kernel.md)

For the [heat equation](heat-equation.md) $u_t=\frac12u_{xx}$ on $x>0$ with the [Neumann boundary condition](neumann-boundary-condition.md) $u_x(t,0)=0$, the method of images gives

$$
K_t^N(x,y)=p_t(x-y)+p_t(x+y),
\qquad
p_t(z)=\frac1{\sqrt{2\pi t}}e^{-z^2/(2t)}.
$$

Thus $u(t,x)=\int_0^\infty K_t^N(x,y)f(y)dy$. This is also the transition kernel of [Reflected Brownian motion](reflected-brownian-motion.md).

## ↑ Ancestors (8)

1. [Heat kernel](heat-kernel.md)
2. [Heat equation](heat-equation.md)
3. [Diffusion equation](diffusion-equation-split.md)
4. [Partial differential equation](partial-differential-equation-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-202/6/b/solution.md)
