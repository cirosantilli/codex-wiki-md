<h1 id="15d/solution">Solution</h1>

↑ **Parent:** [15D](../15d.md)

Use the original PDF constraints, whose right sides are $8$ and $9$. Introduce nonnegative surplus variables $s_1,s_2$, slack $s_3$, and artificial variables $a_1,a_2$:

$$
2x_1+x_2-s_1+a_1=8,\qquad x_1+3x_2-s_2+a_2=9,\qquad x_1+s_3=6.
$$

All seven variables are nonnegative. Phase I of the [two-phase simplex method](../../../../../two-phase-simplex.md) minimizes $w=a_1+a_2$ with initial basis $(a_1,a_2,s_3)$. The initial [simplex dictionary](../../../../../simplex-dictionary.md) is

$$
\begin{aligned}
a_1&=8-2x_1-x_2+s_1,\\a_2&=9-x_1-3x_2+s_2,\\s_3&=6-x_1,\\w&=17-3x_1-4x_2+s_1+s_2.
\end{aligned}
$$

Enter $x_2$ and leave $a_2$: the ratio test gives $\min(8,9/3)=3$. Substituting $x_2=3-x_1/3+s_2/3-a_2/3$ gives

$$
a_1=5-\frac53x_1+s_1-\frac13s_2+\frac13a_2,\qquad
w=5-\frac53x_1+s_1-\frac13s_2+\frac43a_2.
$$

Now enter $x_1$ and leave $a_1$. The bounds from $a_1,x_2,s_3$ are $3,9,6$, so the ratio test selects $3$. The new dictionary is

$$
\begin{aligned}
x_1&=3+\frac35s_1-\frac15s_2-\frac35a_1+\frac15a_2,\\
x_2&=2-\frac15s_1+\frac25s_2+\frac15a_1-\frac25a_2,\\
s_3&=3-\frac35s_1+\frac15s_2+\frac35a_1-\frac15a_2.
\end{aligned}
$$

The associated basic solution has $a_1=a_2=0$ and $w=0$, which is a global minimum because artificial variables are nonnegative. Delete their columns for Phase II. In the remaining basis $(x_1,x_2,s_3)$ the objective is

$$
z=9-p+\frac{9-4p}{5}s_1+\frac{3p-3}{5}s_2.
$$

For $2\le p\le9/4$, both [reduced costs](../../../../../reduced-cost.md) are nonnegative, so the [simplex method](../../../../../simplex-method.md) has reached the optimum at $(x_1,x_2)=(3,2)$:

$$
\boxed{z_{\min}=9-p.}
$$

For $9/4<p\le3$, the coefficient of $s_1$ is negative. Enter $s_1$; the ratio test gives $10$ from $x_2$ and $5$ from $s_3$, so $s_3$ leaves. Eliminating $s_1$ gives

$$
x_1=6-s_3,\qquad x_2=1+\frac13s_2+\frac13s_3,\qquad s_1=5+\frac13s_2-\frac53s_3,
$$

and hence

$$
z=18-5p+\frac p3s_2+\left(\frac{4p}{3}-3\right)s_3.
$$

The two reduced costs are now positive, so $(6,1)$ is optimal and

$$
\boxed{z_{\min}=18-5p.}
$$

At $p=9/4$ the whole feasible edge from $(3,2)$ to $(6,1)$ is optimal; both value formulas agree. These dictionaries explicitly carry out both phases rather than inferring the answer solely from a feasible-region sketch.

## ↑ Ancestors (10)

1. [15D](../15d.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
