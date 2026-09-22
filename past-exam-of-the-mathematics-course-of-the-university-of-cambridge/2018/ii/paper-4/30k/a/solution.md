<h1 id="30k/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [dynamic programming](../../../../../../dynamic-programming.md) principle over a short interval $[t,t+\Delta t]$ gives

$$
F(x,t)=\inf_u\left\{c_tu^2\Delta t+F(x+u\Delta t,t+\Delta t)\right\}+o(\Delta t).
$$

A first-order [Taylor expansion](../../../../../../taylor-expansion.md) of the [value function](../../../../../../value-function.md) gives

$$
F(x+u\Delta t,t+\Delta t)
=F(x,t)+F_xu\Delta t+F_t\Delta t+o(\Delta t).
$$

After subtracting $F(x,t)$, dividing by $\Delta t$ and taking the [limit](../../../../../../limit-of-a-function.md), the [Hamilton-Jacobi-Bellman equation](../../../../../../hamilton-jacobi-bellman-equation.md) is

$$
\boxed{F_t=-\inf_u\{c_tu^2+F_xu\}},
\qquad F(x,h)=x^2.
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [30K](../../30k.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
