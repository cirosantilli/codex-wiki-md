<h1 id="1/1/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Let $(\sigma_i,x_i,y_i)$ be the [singular system of a compact operator](../../../../../../../singular-system-of-a-compact-operator.md). Since $P_nx_i=x_i$ for $i\leq n$ and $P_nx_i=0$ for $i>n$, the truncated operator $T_n=AP_n$ has the finite [singular value decomposition](../../../../../../../singular-value-decomposition.md)

$$
T_nx_i=\sigma_i y_i\quad(i\leq n),
\qquad
T_nx_i=0\quad(i>n).
$$

Consequently

$$
T_n^\dagger y
=\sum_{i=1}^n\frac{\langle y,y_i\rangle}{\sigma_i}x_i
=A^\dagger Q_ny,
$$

so $\boxed{T_n^\dagger=A^\dagger Q_n}$.

For completeness, $T_n^\dagger T_n=P_n$ on $(\ker A)^\perp$ and $T_nT_n^\dagger=Q_n$. These are self-adjoint [orthogonal projectors](../../../../../../../orthogonal-projection.md), and hence

$$
T_nT_n^\dagger T_n=T_n,
\qquad
T_n^\dagger T_nT_n^\dagger=T_n^\dagger.
$$

**Thus all four [Penrose equations](../../../../../../../penrose-equations.md) hold, which verifies the formula independently of the singular expansion.**

## ↑ Ancestors (12)

1. [2](../2.md)
2. [1](../../1.md)
3. [1](../../../1.md)
4. [Paper 326](../../../../paper-326-split.md)
5. [Iii](../../../../split.md)
6. [2021](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
