<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Put $\alpha=e^{2\pi i/3}$, so $\alpha^3=1$ and $1+\alpha+\alpha^2=0$. Since the [group](../../../../group-split.md) is [Abelian](../../../../abelian-group.md), every [conjugacy class](../../../../conjugacy-class.md) is a singleton. The [character table](../../../../character-table.md) is

$$
\boxed{\begin{array}{c|ccc}
 &0&1&2\\\hline
\chi_0&1&1&1\\
\chi_1&1&\alpha&\alpha^2\\
\chi_2&1&\alpha^2&\alpha
\end{array}.}
$$

For the [character inner product](../../../../character-inner-product.md), complex conjugation gives

$$
\langle\chi_j,\chi_k\rangle
=\frac13\sum_{g=0}^2\overline{\chi_j(g)}\chi_k(g)
=\frac13\left(1+\alpha^{k-j}+\alpha^{2(k-j)}\right).
$$

For $j=k$, all three summands are one, giving unit norm. For $k-j\equiv1\pmod3$ the sum is $1+\alpha+\alpha^2=0$; for $k-j\equiv2\pmod3$ it is $1+\alpha^2+\alpha=0$. This checks every distinct pair, proving

$$
\boxed{\langle\chi_j,\chi_k\rangle=\delta_{jk}.}
$$

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [2018](../../../2018-split.md)
4. [Past exam of the groups and representations course of the University of Oxford](../../../split.md)
5. [Groups and representations course of the University of Oxford](../../../../groups-and-representations-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
