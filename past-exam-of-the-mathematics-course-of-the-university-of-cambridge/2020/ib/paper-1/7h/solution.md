<h1 id="7h/solution">Solution</h1>

↑ **Parent:** [7H](../7h.md)

Write the absolute-value constraint as

$$
x_1-2x_2\leq2,\qquad -x_1+2x_2\leq2.
$$

Introduce slacks $s_1,s_2,s_3$. In the [simplex algorithm](../../../../../simplex-algorithm.md), let $x_2$ enter and $s_2$ leave, then let $x_1$ enter and $s_3$ leave. The final dictionary is

$$
x_1=\frac23+\frac19s_2-\frac29s_3,
\qquad
x_2=\frac43-\frac49s_2-\frac19s_3,
$$



$$
x_1+x_2=2-\frac13s_2-\frac13s_3.
$$

Thus

$$
\boxed{(x_1,x_2)=\left(\frac23,\frac43\right),
\qquad \max(x_1+x_2)=2}.
$$

For sufficiently small perturbations, the same two constraints remain active:

$$
-x_1+2x_2=2+\epsilon_1,\qquad
4x_1+x_2=4+\epsilon_2.
$$

Solving gives

$$
x_1=\frac{6+2\epsilon_2-\epsilon_1}{9},
\qquad
x_2=\frac{12+\epsilon_2+4\epsilon_1}{9},
$$

and therefore the perturbed optimal value is

$$
\boxed{2+\frac{\epsilon_1+\epsilon_2}{3}}.
$$

## ↑ Ancestors (10)

1. [7H](../7h.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2020](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
