<h1 id="f/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Differentiability at $a$ means that there is a [linear map](../../../../linear-map.md) $L:V\to V_1$ with

$$
\frac{\|f(a+h)-f(a)-Lh\|_1}{\|h\|}\longrightarrow0\quad(h\to0).
$$

This map is the [total derivative](../../../../total-derivative.md) $Df_a$. In the [Frobenius norm](../../../../frobenius-norm.md), $|AB|\le|A||B|$, by the [Cauchy-Schwarz inequality](../../../../cauchy-schwarz-inequality.md) applied to [matrix](../../../../matrix.md) entries. Expanding with the order of all factors preserved gives

$$
(A+H)^3=A^3+A^2H+AHA+HA^2+AH^2+HAH+H^2A+H^3.
$$

The remainder after the terms linear in $H$ has norm at most $3|A||H|^2+|H|^3=o(|H|)$. Hence

$$
\boxed{Df_A(H)=A^2H+AHA+HA^2.}
$$

For $|C|<1$, the [Neumann series](../../../../neumann-series.md) $I-C+C^2-\cdots$ converges absolutely in the finite-dimensional space of [matrices](../../../../matrix.md). Multiplying its partial sums by $I+C$ and passing to the limit shows that it is $(I+C)^{-1}$. Its remainder after $I-C$ has norm at most $|C|^2/(1-|C|)=o(|C|)$, proving the required expansion.

If $A$ is an [invertible matrix](../../../../invertible-matrix.md) and $|H|<1/|A^{-1}|$, then $A+H=A(I+A^{-1}H)$ is an [invertible matrix](../../../../invertible-matrix.md). Thus the [general linear group](../../../../general-linear-group.md) is an open subset of the [matrix](../../../../matrix.md) space. The preceding expansion also gives

$$
(A+H)^{-1}=A^{-1}-A^{-1}HA^{-1}+o(|H|).
$$

Apply the [chain rule](../../../../chain-rule.md) to $g(X)=(X^{-1})^3$, using the cubic [total derivative](../../../../total-derivative.md) at $A^{-1}$ and this [total derivative](../../../../total-derivative.md) of inversion:

$$
\boxed{Dg_A(H)=-A^{-3}HA^{-1}-A^{-2}HA^{-2}-A^{-1}HA^{-3}.}
$$

The three terms generally cannot be combined by commuting $A$ and $H$.

## ↑ Ancestors (12)

1. [2](../2.md)
2. [F](../../f.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the Probability, statistics and options II course of the University of Oxford](../../../split.md)
5. [Probability, statistics and options II course of the University of Oxford](../../../../probability-statistics-and-options-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
7. [Mathematics and statistics course of the University of Oxford](../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
