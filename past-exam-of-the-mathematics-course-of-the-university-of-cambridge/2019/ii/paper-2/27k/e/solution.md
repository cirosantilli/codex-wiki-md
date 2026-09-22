<h1 id="27k/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Let $m$ be a nonzero invariant measure. Balance at state $i\geq1$ gives

$$
m_{i-1}\lambda_{i-1}
=m_i\lambda_i(1+\rho_i),
$$

and hence, after choosing $m_0>0$,

$$
m_i=\frac{m_0\lambda_0}
{\lambda_i\prod_{j=1}^i(1+\rho_j)}.
$$

Balance at zero requires

$$
m_0\lambda_0=\sum_{i\geq1}m_i\lambda_i\rho_i
=m_0\lambda_0\sum_{i\geq1}
\frac{\rho_i}{\prod_{j=1}^i(1+\rho_j)}.
$$

The sum telescopes:

$$
\sum_{i=1}^n\frac{\rho_i}{\prod_{j=1}^i(1+\rho_j)}
=1-\frac1{\prod_{j=1}^n(1+\rho_j)}.
$$

Consequently a nonzero invariant measure exists exactly when

$$
\boxed{\prod_{j=1}^{\infty}(1+\rho_j)=\infty.}
$$

It can be normalized to an invariant probability distribution exactly when, in addition,

$$
\sum_{i=0}^{\infty}
\frac1{\lambda_i\prod_{j=1}^i(1+\rho_j)}<\infty,
$$

where the empty product for $i=0$ is one and an overall constant has been suppressed.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [27K](../../27k.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
