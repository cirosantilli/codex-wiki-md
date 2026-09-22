# Mixed-boundary convection-diffusion solution in parabolic coordinates

↑ **Parent:** [Advection-diffusion equation](advection-diffusion-equation.md)

For $y>0$, the displayed function, expressed using the [complementary error function](complementary-error-function.md), satisfies $\Delta u=u_x$, with $u=1$ on the positive boundary ray and $u_y=0$ on the negative boundary ray. Put $x=a^2-b^2$, $y=2ab$, so $u=\operatorname{erfc}b$. Then $\Delta u=u_{bb}/[4(a^2+b^2)]$ and $u_x=-bu_b/[2(a^2+b^2)]$; the derivative identity $u_{bb}=-2bu_b$ verifies the equation. Its boundary traces are $u(x,0)=\operatorname{erfc}\sqrt{-x}$ for $x<0$ and $u_y(x,0)=-1/\sqrt{\pi x}$ for $x>0$. At fixed nonzero polar angle it decays at infinity, but along fixed $y>0$ and $x\to+\infty$ it approaches one. The downstream thermal layer has width $O(\sqrt x)$, so uniform radial decay would be an incompatible far-field condition.

## ↑ Ancestors (7)

1. [Advection-diffusion equation](advection-diffusion-equation.md)
2. [Diffusion equation](diffusion-equation-split.md)
3. [Partial differential equation](partial-differential-equation-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-perturbation-methods-and-applied-complex-variables-course-of-the-university-of-oxford/2010/b/6/iii/solution.md)
