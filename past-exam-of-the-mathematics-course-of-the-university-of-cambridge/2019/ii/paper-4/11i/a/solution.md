<h1 id="11i/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Set

$$
p_{-1}=1,\quad q_{-1}=0,
\qquad
p_0=a_0,\quad q_0=1,
$$

and, for $n\geq1$, define

$$
p_n=a_np_{n-1}+p_{n-2},
\qquad
q_n=a_nq_{n-1}+q_{n-2}.
$$

Writing $M(a)=\left(\begin{smallmatrix}a&1\\1&0\end{smallmatrix}\right)$, these recurrences are equivalent to the [continued-fraction matrix](../../../../../../continued-fraction-matrix.md) identity

$$
M(a_0)\cdots M(a_n)
=\begin{pmatrix}p_n&p_{n-1}\\q_n&q_{n-1}\end{pmatrix}.
$$

The associated [Möbius transformation](../../../../../../mobius-transformation.md) sends a positive tail $\beta$ to the [continued-fraction tail formula](../../../../../../continued-fraction-tail-formula.md)

$$
\boxed{\theta_n=[a_0,\ldots,a_n,\beta]
=\frac{\beta p_n+p_{n-1}}{\beta q_n+q_{n-1}}.}
$$

Since $\det M(a_j)=-1$, taking determinants gives

$$
\boxed{p_nq_{n-1}-p_{n-1}q_n=(-1)^{n+1}=(-1)^{n-1}.}
$$

Moreover,

$$
\theta_n-\frac{p_n}{q_n}
=\frac{p_{n-1}q_n-p_nq_{n-1}}
{q_n(\beta q_n+q_{n-1})},
$$

whereas

$$
\theta_n-\frac{p_{n-1}}{q_{n-1}}
=\frac{\beta(p_nq_{n-1}-p_{n-1}q_n)}
{q_{n-1}(\beta q_n+q_{n-1})}.
$$

Their signs are opposite, so $\theta_n$ lies between the two adjacent convergents. For $n=0$, the second endpoint is interpreted as $p_{-1}/q_{-1}=\infty$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [11I](../../11i.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
