# Mixed endpoint Green kernel for a first-derivative drift

↑ **Parent:** [Green's function](green-s-function-split.md)

Multiplying the equation for $v=y'$ by the [integrating factor](integrating-factor.md) $e^x$ gives $v(x)=-e^{-x}\int_x^1e^tf(t)\,dt$. Integrating once more and reversing the order of integration gives the [Green's function](green-s-function-split.md)

$$
G(x,t)=\begin{cases}1-e^t,&t\leq x,\\e^{t-x}-e^t,&x\leq t.\end{cases}
$$

It is continuous across $x=t$, its first derivative has jump $+1$, and it satisfies the mixed [Dirichlet boundary condition](dirichlet-boundary-condition.md) and [Neumann boundary condition](neumann-boundary-condition.md). Both homogeneous solutions, $1$ and $e^{-x}$, are eliminated by these two conditions, giving [uniqueness](uniqueness.md). For $f=e^{-x}$ the solution is $-xe^{-x}$.

## ↑ Ancestors (5)

1. [Green's function](green-s-function-split.md)
2. [Analysis](analysis-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)
