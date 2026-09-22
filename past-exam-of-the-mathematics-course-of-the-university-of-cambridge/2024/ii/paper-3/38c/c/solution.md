<h1 id="38c/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Set

$$
A=\left(\frac{\rho\nu^2}{S}\right)^{1/3},
\qquad U_0=\frac{\nu}{A^2},
\qquad \eta=\frac{y}{A\sqrt x},
$$

and choose stream [function](../../../../../../function-split.md)

$$
\psi=U_0A\sqrt x,f(\eta).
$$

Then

$$
u=U_0f'(\eta),
\qquad
v=-\frac{U_0A}{2\sqrt x}\{f-\eta f'\}.
$$

Substitution gives

$$
f'''+\frac12ff''=0,
$$

with

$$
f(0)=0,
\qquad f''(0)=1,
\qquad f'(\infty)=0.
$$

Treat $f'(0)$ as a shooting parameter, integrate the initial-value problem numerically, and adjust it until the far-field condition holds. The adjacent-fluid speed is then $u(x,0)=U_0f'(0)$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [38C](../../38c.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
