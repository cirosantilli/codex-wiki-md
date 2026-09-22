<h1 id="9h/solution">Solution</h1>

↑ **Parent:** [9H](../9h.md)

For a [simple continued fraction](../../../../../simple-continued-fraction.md), define

$$
p_{-2}=0,\ p_{-1}=1,\quad q_{-2}=1,\ q_{-1}=0,\qquad p_n=a_np_{n-1}+p_{n-2},\quad q_n=a_nq_{n-1}+q_{n-2}.
$$

Multiplying the matrices $\begin{pmatrix}a_j&1\\1&0\end{pmatrix}$ gives

$$
\begin{pmatrix}p_{n-1}&p_{n-2}\\q_{n-1}&q_{n-2}\end{pmatrix},\qquad [a_0,\ldots,a_{n-1},\beta]=\frac{\beta p_{n-1}+p_{n-2}}{\beta q_{n-1}+q_{n-2}}.
$$

Their determinants also give $p_nq_{n-1}-p_{n-1}q_n=(-1)^{n-1}$. If the infinite tail is $\beta=[a_{n+1},a_{n+2},\ldots]>a_{n+1}$, the same formula implies

$$
\left|\theta-\frac{p_n}{q_n}\right|=\frac1{q_n(\beta q_n+q_{n-1})}<\frac1{q_nq_{n+1}}.
$$

The denominators of these [continued fraction convergents](../../../../../continued-fraction-convergent.md) tend to infinity, since $q_{n+2}\geq q_{n+1}+q_n$. Hence they converge to $\theta$.

The square-root algorithm for the [periodic continued fraction of a quadratic irrational](../../../../../periodic-continued-fraction-of-a-quadratic-irrational.md), using $M'=Da-M$, $D'=(53-M'^2)/D$ and $a'=\lfloor(7+M')/D'\rfloor$, gives

$$
\sqrt{53}=[7;\overline{3,1,1,3,14}].
$$

The first four [continued fraction convergents](../../../../../continued-fraction-convergent.md) are $7/1,22/3,29/4,51/7$. Direct substitution gives **positive solutions to the requested Pell-type equations**:

$$
\boxed{51^2-53\cdot7^2=4,\qquad29^2-53\cdot4^2=-7.}
$$

## ↑ Ancestors (10)

1. [9H](../9h.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
