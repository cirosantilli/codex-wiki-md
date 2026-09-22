<h1 id="18h/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Introduce unrestricted row and column potentials $u_i,v_j$. The dual is

$$
\text{maximize }\sum_i u_is_i+\sum_jv_jd_j
\quad\text{subject to }u_i+v_j\leq c_{ij}.
$$

Primal and dual feasible solutions are optimal precisely when [complementary slackness](../../../../../../complementary-slackness.md) holds:

$$
x_{ij}>0\implies u_i+v_j=c_{ij}.
$$

Indeed, the primal--dual objective gap is $\sum_{ij}x_{ij}(c_{ij}-u_i-v_j)$, a sum of nonnegative terms.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [18H](../../18h.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
