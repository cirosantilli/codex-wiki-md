<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For fixed $L$, expansion of the matrix in part (b) gives

$$
(M_\varepsilon^L)^TM_\varepsilon^L
=
\begin{pmatrix}
(1+O(\varepsilon^4))I&O(\varepsilon^3)I\\
O(\varepsilon^3)I&(1+O(\varepsilon^4))I
\end{pmatrix}.
$$

Hence its largest eigenvalue is $1+O(\varepsilon^3)$. With $z=(x(0),p(0))$ and $z'=M_\varepsilon^Lz$,

$$
H(z')=\frac12\|z'\|^2
\leq(1+C_0\varepsilon^3)H(z).
$$

For each fixed starting state, or uniformly on any bounded set of starting states, this implies

$$
H(z')-H(z)\leq C_1\varepsilon^3.
$$

Using $e^{-u}\geq1-u$ for $u\geq0$ in the acceptance formula gives

$$
\boxed{1-C\varepsilon^3\leq\alpha\leq1}
$$

for sufficiently small $\varepsilon$. The constant necessarily depends on a bound for $\|z\|$: a uniform pointwise constant over all of $\mathbb R^{2d}$ would be impossible because the energy error is quadratic in the starting state.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [6](../../6.md)
3. [Paper 216](../../../paper-216-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
