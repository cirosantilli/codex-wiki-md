# Boundary conditions for variational Rayleigh quotients

↑ **Parent:** [Rayleigh quotient](rayleigh-quotient.md)

For real smooth coefficients with $p,w>0$, the [Rayleigh quotient](rayleigh-quotient.md) $\Lambda[y]=\int[p(y')^2+qy^2]dx/\int wy^2dx$ has the displayed [first variation](first-variation.md). Its stationary points solve the [Sturm-Liouville equation](sturm-liouville-equation.md) on an admissible class whose boundary variations make $[py'\eta]_a^b=0$. Homogeneous [Dirichlet boundary conditions](dirichlet-boundary-condition.md) do this by setting $\eta=0$ at the ends; homogeneous [Neumann boundary conditions](neumann-boundary-condition.md) do it through $y'=0$. More general self-adjoint boundary conditions can require a boundary contribution to the quadratic form.

For an [eigenfunction](eigenfunction.md), the weaker identity $[pyy']_a^b=0$ suffices to give $\lambda=\Lambda[y]$ by [integration by parts](integration-by-parts.md), but it does not by itself imply the condition on every variation. An explicit counterexample uses $p=q=w=1$ on $[0,1]$ and $y=\cos\pi x+\sin\pi x$. This solves $-y''+y=(1+\pi^2)y$ and has $[yy']_0^1=0$. Define a nearby family

$$
y_\varepsilon=y+\varepsilon(3x^2-2x^3)+\frac{\pi\varepsilon}{\varepsilon-1}(x^3-x^2).
$$

It keeps $y_\varepsilon(0)=1$, $y_\varepsilon'(0)=\pi$, $y_\varepsilon(1)=-1+\varepsilon$, and $y_\varepsilon'(1)=\pi/(-1+\varepsilon)$, so $[y_\varepsilon y_\varepsilon']_0^1=0$ for small $\varepsilon$. Nevertheless, $\eta=\partial_\varepsilon y_\varepsilon|_0$ has $\eta(0)=0$, $\eta(1)=1$, and $\int_0^1y^2dx=1$, giving $\delta\Lambda=2[y'\eta]_0^1=-2\pi\ne0$. Boundary-energy cancellation alone therefore cannot replace a specified variational domain.

## ↑ Ancestors (7)

1. [Rayleigh quotient](rayleigh-quotient.md)
2. [Operator theory](linear-operator-theory-split.md)
3. [Linear algebra](linear-algebra-split.md)
4. [Algebra](algebra-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2007/paper-1/10/solution.md)
