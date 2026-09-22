<h1 id="30k/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Completing the square in the [Hamilton-Jacobi-Bellman equation](../../../../../../hamilton-jacobi-bellman-equation.md) shows that the minimizing feedback is

$$
u^*(x,t)=-\frac{F_x(x,t)}{2c_t}.
$$

This is a [linear-quadratic optimal control](../../../../../../linear-quadratic-optimal-control.md) problem, so set $F(x,t)=a(t)x^2$. The equation and terminal condition become

$$
a'(t)=\frac{a(t)^2}{c_t},
\qquad a(h)=1.
$$

This [Riccati equation](../../../../../../riccati-equation.md) is separable and gives

$$
\frac1{a(t)}=1+\int_t^h\frac{ds}{c_s}.
$$

Consequently the general optimal feedback law is

$$
\boxed{u^*(x,t)=-\frac{x}{c_t\left(1+\displaystyle\int_t^h ds/c_s\right)}}.
$$

When $c_t=c$ is constant,

$$
F(x,t)=\frac{c}{c+h-t}x^2,
\qquad
\boxed{u^*(x,t)=-\frac{x}{c+h-t}}.
$$

Along the corresponding optimal trajectory, $x_s=x(c+h-s)/(c+h-t)$, so the open-loop control is constant: $u_s^*=-x/(c+h-t)$ for $s\in[t,h]$.

## ↑ Ancestors (11)

1. [B](../b.md)
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
