# Implicit factorization can reveal nonunique initial solutions

↑ **Parent:** [Initial value problem](initial-value-problem.md)

The displayed implicit [ordinary differential equation](ordinary-differential-equation.md) has a singular initial point at the origin. On a nonconstant regular branch, treating $x$ as a function of $y$ gives $dx/dy+x\cot y=2\cos y$. The [integrating factor](integrating-factor.md) $\sin y$ yields the [first integral of an ordinary differential equation](first-integral-of-an-ordinary-differential-equation.md)

$$
x\sin y-\sin^2y=C.
$$

One can verify this identity without dividing by $\sin y$: its [derivative](derivative.md) along a solution is $\sin y-(2\sin y-x)\cos y\,y'=0$.

The initial point forces $C=0$, so $\sin y(x-\sin y)=0$. Near the origin this gives the two differentiable solutions $y=0$ and $y=\arcsin x$, with initial slopes zero and one. A division by $\sin y$ would lose the first solution. A piecewise switch between the two at zero would fail [differentiability](differentiability.md) because their one-sided slopes differ.

There is no conflict with the [Picard-Lindelöf theorem](picard-lindelof-theorem.md): solving explicitly for $y'$ requires division by $2\sin y-x$, which vanishes at the initial point. A regular implicit equation or a local uniqueness theorem must be checked before claiming a unique solution through a singular point.

## ↑ Ancestors (7)

1. [Initial value problem](initial-value-problem.md)
2. [Ordinary differential equation](ordinary-differential-equation.md)
3. [Differential equation](differential-equation-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)
