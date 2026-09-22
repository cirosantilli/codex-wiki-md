<h1 id="8h/solution">Solution</h1>

↑ **Parent:** [8H](../8h.md)

Introduce nonnegative slack variables $s_1,s_2$ and use the origin as the initial feasible [simplex basis](../../../../../simplex-basis.md):

$$
s_1=10-x_1-x_2-2x_3,\qquad s_2=15-2x_1-x_2-3x_3,\qquad z=x_1+2x_2+x_3.
$$

In the [simplex method](../../../../../simplex-method.md), let $x_2$ enter. The ratio test is $\min(10,15)=10$, so $s_1$ leaves. Solving the first constraint for $x_2$ yields the dictionary

$$
x_2=10-x_1-2x_3-s_1,\qquad s_2=5-x_1-x_3+s_1,\qquad z=20-x_1-3x_3-2s_1.
$$

All nonbasic variables are nonnegative and have negative reduced objective coefficients. Setting them to zero is feasible and optimal:

$$
\boxed{(x_1,x_2,x_3)=(0,10,0),\quad z_{\max}=20}.
$$

Subtracting $\Delta$ from both right-hand sides changes the same dictionary to

$$
x_2=10-\Delta-x_1-2x_3-s_1,\qquad s_2=5-x_1-x_3+s_1,\qquad z=20-2\Delta-x_1-3x_3-2s_1.
$$

It remains feasible throughout $0\le\Delta\le10$, including the degenerate endpoint $\Delta=10$, and the reduced coefficients are unchanged. Hence

$$
\boxed{z_{\max}(\Delta)=20-2\Delta,\quad(x_1,x_2,x_3)=(0,10-\Delta,0)}.
$$

As an independent optimality certificate, $z\le2(x_1+x_2+2x_3)\le2(10-\Delta)$, with equality at the stated point. Negative reduced coefficients also prove uniqueness of the optimal decision vector.

## ↑ Ancestors (10)

1. [8H](../8h.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
