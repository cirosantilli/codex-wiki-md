<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Define the stage states $Y_i=y_n+h\sum_j a_{ij}k_j$, so $k_i=PY_i$. Skew symmetry gives $Y_i^Tk_i=Y_i^TPY_i=0$, and hence

$$
y_n^Tk_i=-h\sum_j a_{ij}k_j^Tk_i.
$$

Insert this into the preceding norm identity and symmetrize the double sum, using $k_i^Tk_j=k_j^Tk_i$. The result is the [Runge-Kutta conservation of quadratic invariants](../../../../../../runge-kutta-conservation-of-quadratic-invariants.md) identity

$$
\lVert y_{n+1}\rVert^2-\lVert y_n\rVert^2=-h^2\sum_{i,j}\left(b_i a_{ij}+b_j a_{ji}-b_i b_j\right)k_i^Tk_j.
$$

Thus

$$
\boxed{M=0\quad\Longrightarrow\quad\lVert y_{n+1}\rVert=\lVert y_n\rVert,}
$$

which proves the sufficient condition for every well-defined step and then for all $n$ by induction. For example the [implicit midpoint rule](../../../../../../implicit-midpoint-rule.md), with $a_{11}=1/2$ and $b_1=1$, has $M_{11}=0$ and preserves this norm exactly. The condition is sufficient, and need not be necessary for a particular matrix or a particular solution.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 71](../../../paper-71-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
