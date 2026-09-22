<h1 id="f/f2/solution">Solution</h1>

↑ **Parent:** [F2](../f2.md)

Differentiability at $a$ means that a linear map $L:V\to V_1$ satisfies

$$
\frac{\|f(a+h)-f(a)-Lh\|_1}{\|h\|}\longrightarrow0\quad(h\to0).
$$

This map is unique and is the total derivative $Df_a$. In finite dimensions linear maps are continuous.

The [Frobenius norm](../../../../frobenius-norm.md) is submultiplicative. Expanding the noncommuting cube gives

$$
(A+H)^3=A^3+A^2H+AHA+HA^2+AH^2+HAH+H^2A+H^3.
$$

The last four terms have [norm](../../../../norm.md) at most $3|A||H|^2+|H|^3=o(|H|)$. Thus

$$
\boxed{Df_A(H)=A^2H+AHA+HA^2}.
$$

If $|C|<1$, the [Neumann series](../../../../neumann-series.md) $\sum_{j\ge0}(-C)^j$ converges and is the inverse of $I+C$, as follows by multiplying its partial sums and letting the final power tend to zero. Its terms from degree two onwards have [norm](../../../../norm.md) at most $|C|^2/(1-|C|)$. Hence $(I+C)^{-1}=I-C+O(|C|^2)$.

For invertible $A$, write $A+H=A(I+A^{-1}H)$. Whenever $|A^{-1}||H|<1$, this is invertible, proving the [general linear group](../../../../general-linear-group.md) is open. The same expansion gives

$$
(A+H)^{-1}=A^{-1}-A^{-1}HA^{-1}+O(|H|^2).
$$

Compose this inverse derivative with the cube derivative, setting $B=A^{-1}$. The result is

$$
\boxed{Dg_A(H)=-(A^{-3}HA^{-1}+A^{-2}HA^{-2}+A^{-1}HA^{-3})}.
$$

The three terms cannot generally be combined into a scalar-style $-3A^{-4}H$, because matrix factors need not commute.

This is the cubic case of the [Fréchet derivative of a negative matrix power](../../../../frechet-derivative-of-a-negative-matrix-power.md).

## ↑ Ancestors (12)

1. [F2](../f2.md)
2. [F](../../f.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the options II course of the University of Oxford](../../../split.md)
5. [Options II course of the University of Oxford](../../../../options-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
