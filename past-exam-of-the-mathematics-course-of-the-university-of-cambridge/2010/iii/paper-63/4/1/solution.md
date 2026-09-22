<h1 id="4/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

For $y'=f(t,y)$ and step $h$, a [collocation Runge-Kutta method](../../../../../../collocation-runge-kutta-method.md) constructs a [polynomial](../../../../../../polynomial-split.md) $P$ of degree at most $s$ on $[t_n,t_n+h]$ satisfying

$$
P(t_n)=y_n,\qquad
P'(t_n+c_i h)=f(t_n+c_i h,P(t_n+c_i h)),\quad 1\le i\le s.
$$

The step value is $y_{n+1}=P(t_n+h)$. Thus the differential equation holds exactly at the prescribed collocation nodes, while the initial value fixes the integration constant. For a smooth vector field and small enough $h$, the implicit stage equations have the local solution branch continuing the zero-step initial state; arbitrary large steps need not have a unique nonlinear solution.

## ↑ Ancestors (11)

1. [1](../1.md)
2. [4](../../4.md)
3. [Paper 63](../../../paper-63-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
