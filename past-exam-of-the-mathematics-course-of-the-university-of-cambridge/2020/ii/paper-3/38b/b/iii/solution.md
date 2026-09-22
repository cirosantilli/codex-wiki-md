<h1 id="38b/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Let

$$
\epsilon=\sqrt{\frac\nu Q},
\qquad
\eta=\frac{y}{\epsilon x},
\qquad
\psi=\sqrt{\nu Q}\,f(\eta)=Q\epsilon f(\eta).
$$

Using the [Cartesian streamfunction](../../../../../../../cartesian-streamfunction.md) convention $u=\psi_y$, $v=-\psi_x$ gives

$$
u=\frac Qx f'(\eta),
\qquad
v=\frac{Q\epsilon}{x}\eta f'(\eta).
$$

At fixed $y$,

$$
u_x=-\frac Q{x^2}[f'+\eta f''],
\qquad
u_y=\frac Q{\epsilon x^2}f'',
\qquad
u_{yy}=\frac Q{\epsilon^2x^3}f'''.
$$

The terms proportional to $\eta f'f''$ cancel, leaving

$$
u u_x+v u_y=-\frac{Q^2}{x^3}(f')^2.
$$

Since $U=-Q/x$, $UU'=-Q^2/x^3$, while $\nu u_{yy}=Q^2f'''/x^3$. The boundary-layer equation therefore becomes

$$
\boxed{f'''=1-(f')^2}.
$$

Choosing the wall value of the streamfunction as zero, imposing no slip, and matching to $U=-Q/x$ give

$$
\boxed{f(0)=0,
\qquad f'(0)=0,
\qquad f'(\eta)\to-1\quad(\eta\to\infty)}.
$$

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [38B](../../../38b.md)
4. [Paper 3](../../../../paper-3-split.md)
5. [Ii](../../../../split.md)
6. [2020](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
