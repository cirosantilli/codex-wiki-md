<h1 id="7h/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Introduce nonnegative dual variables $y$ and $z$ for the two constraints. The [dual of a minimization linear program in inequality form](../../../../../../dual-of-a-minimization-linear-program-in-inequality-form.md) is

$$
\boxed{
\begin{aligned}
\text{maximise}\quad&ty+rz\\
\text{subject to}\quad&b_i y+c_i z\leq a_i
\quad(1\leq i\leq n),\\
&y,z\geq0.
\end{aligned}}
$$

Indeed, if $x$ and $(y,z)$ are feasible, then

$$
ty+rz
\leq y\sum_i b_ix_i+z\sum_i c_ix_i
=\sum_i(b_i y+c_i z)x_i
\leq\sum_i a_ix_i,
$$

which is [weak duality](../../../../../../weak-duality.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [7H](../../7h.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
