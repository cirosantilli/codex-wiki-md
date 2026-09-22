<h1 id="18h/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Apply the [Charnes-Cooper transformation](../../../../../../../charnes-cooper-transformation.md) to any feasible point $x$ of $Q$:

$$
y=\frac{x}{d^Tx},
\qquad
t=\frac1{d^Tx}.
$$

Then

$$
y\geq0,\quad t>0,\quad Ay=bt,\quad d^Ty=1,
$$

so $(y,t)$ is feasible for $R$, and

$$
c^Ty=\frac{c^Tx}{d^Tx}.
$$

In particular, the given solution $x^*$ of $Q$ produces a feasible point of $R$ with the same objective value, so

$$
\max R\geq\max Q.
$$

Moreover, because every $d_i>0$, the equation $d^Ty=1$ implies

$$
0\leq y_i\leq\frac1{d_i}.
$$

The linear objective $c^Ty$ is therefore bounded on the feasible set. The feasible $y$ lie in the compact simplex $\{y\geq0:d^Ty=1\}$. Their subset arising in $R$ is closed: if $b\ne0$, any nonzero component of $b$ determines $t$ continuously from $Ay=bt$, while if $b=0$ the condition is simply $Ay=0$. Hence the feasible $y$ form a [compact set](../../../../../../../compact-space.md), on which the continuous objective $c^Ty$ attains a finite maximum. Thus $R$ has a finite maximum at least as large as that of $Q$.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [C](../../c.md)
3. [18H](../../../18h.md)
4. [Paper 4](../../../../paper-4-split.md)
5. [Ib](../../../../split.md)
6. [2021](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
