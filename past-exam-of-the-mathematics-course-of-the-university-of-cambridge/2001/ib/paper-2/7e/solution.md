<h1 id="7e/solution">Solution</h1>

↑ **Parent:** [7E](../7e.md)

At a point $z_0=x+iy$, [complex differentiability](../../../../../complex-differentiability.md) means that

$$
f'(z_0)=\lim_{h\to0,\ h\in\mathbb C\setminus\{0\}}\frac{f(z_0+h)-f(z_0)}h
$$

exists and is independent of the direction of approach. Write $f=u+iv$. Restricting to real $h$ gives $f'=u_x+iv_x$. Restricting to $h=it$, with real $t\to0$, gives

$$
f'=\frac{u_y+iv_y}{i}=v_y-iu_y.
$$

These directional limits establish existence of the displayed partial derivatives. Equating their real and imaginary parts gives **the Cauchy-Riemann equations**

$$
\boxed{u_x=v_y,\qquad u_y=-v_x.}
$$

The argument applies at every point of the given open domain; it does not assume continuity of the partial derivatives beforehand.

## ↑ Ancestors (10)

1. [7E](../7e.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
