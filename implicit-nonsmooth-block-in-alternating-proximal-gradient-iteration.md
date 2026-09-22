# Implicit nonsmooth block in alternating proximal-gradient iteration

↑ **Parent:** [Alternating proximal-gradient operator](alternating-proximal-gradient-operator.md)

For $f(x,y)=h(x,y)+\phi(y)$, where $h$ is convex with an $L_h$-[Lipschitz gradient](lipschitz-gradient.md) and $\phi$ is convex, use a proximal $y$-step for the full section and an explicit $x$-step for $h$. Monotonicity of the two selected [subgradients](subgradient.md) of $\phi$ combines with [cocoercivity](cocoercivity.md) of $\nabla h$ to make the full update firmly nonexpansive for $0<\tau L_h\leq1$. Existence of a minimizer then gives convergence, even though the full objective is not smooth.

## ↑ Ancestors (8)

1. [Alternating proximal-gradient operator](alternating-proximal-gradient-operator.md)
2. [Proximal gradient method](proximal-gradient-method.md)
3. [Proximal operator](proximal-operator.md)
4. [Convex optimization](convex-optimization-split.md)
5. [Mathematical optimization](mathematical-optimization-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)
