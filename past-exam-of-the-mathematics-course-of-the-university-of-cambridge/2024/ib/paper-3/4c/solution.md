<h1 id="4c/solution">Solution</h1>

↑ **Parent:** [4C](../4c.md)

For a general [Lagrangian](../../../../../lagrangian.md),

$$
p=\frac{\partial L}{\partial\dot x},
\qquad
H=p\cdot\dot x-L.
$$

Along an Euler-Lagrange trajectory,

$$
\frac{dH}{dt}=-\frac{\partial L}{\partial t},
$$

so energy is conserved when $L$ has no explicit time dependence.

For the given [Lagrangian](../../../../../lagrangian.md), write $v=|\dot x|$. At points where $v\ne0$,

$$
\boxed{p=mc\frac{\dot x}{v}}.
$$

The Euler-Lagrange equation is therefore

$$
\boxed{
\frac d{dt}\left(mc\frac{\dot x}{|\dot x|}\right)
=-\nabla V(x)}.
$$

In expanded form its left-hand side is

$$
mc\left(
\frac{\ddot x}{v}
-\frac{\dot x(\dot x\cdot\ddot x)}{v^3}
\right).
$$

The [momentum](../../../../../momentum.md) has fixed magnitude,

$$
\boxed{p\cdot p=m^2c^2},
$$

so this is constant without needing to solve the equation of motion. The [Hamiltonian](../../../../../hamiltonian.md) is

$$
\boxed{H=p\cdot\dot x-L=V(x)}.
$$

The [singular Legendre transform of a degree-one velocity Lagrangian](../../../../../singular-legendre-transform-of-a-degree-one-velocity-lagrangian.md) applies here: $p$ determines only the direction of $\dot x$, not its magnitude, and the [velocity](../../../../../velocity.md) Hessian is not invertible. Thus the usual inverse Legendre transform cannot reconstruct the [Lagrangian](../../../../../lagrangian.md) from this [Hamiltonian](../../../../../hamiltonian.md).

## ↑ Ancestors (10)

1. [4C](../4c.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
