<h1 id="12f/iii/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The coefficient of $x^{n+1}$ in $r_j$ is

$$
c_j=\frac1{\prod_{k\ne j}(y_j-y_k)}.
$$

With the increasing enumeration, its sign is $(-1)^{n+2-j}$. Therefore all terms $(-1)^jc_j$ have the same sign $(-1)^{n+2}$, and $R:=\sum_j(-1)^jc_j\ne0$. The leading coefficient of $t$ is $T:=\sum_jf(y_j)c_j$. Canceling the coefficient of $x^{n+1}$ gives the unique value

$$
\boxed{\lambda=\frac TR=\frac{\sum_j f(y_j)/\prod_{k\ne j}(y_j-y_k)}{\sum_j(-1)^j/\prod_{k\ne j}(y_j-y_k)}.}
$$

Both interpolants have degree at most $n+1$, so this single cancellation is equivalent to $\deg(t-\lambda r)\leq n$.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [Iii](../../iii.md)
3. [12F](../../../12f.md)
4. [Paper 3](../../../../paper-3-split.md)
5. [Ii](../../../../split.md)
6. [2011](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
