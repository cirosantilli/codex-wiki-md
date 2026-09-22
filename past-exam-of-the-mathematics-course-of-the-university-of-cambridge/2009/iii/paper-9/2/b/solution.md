<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

If either upper norm bound is nonpositive, there are no admissible functions with $\|f\|_q\geq C_q>0$, and the assertion is vacuous. For positive $C_p,C_r$, choose

$$
\varepsilon=\left(\frac{C_q^q}{2C_p^p}\right)^{1/(q-p)},\qquad A=\{x:|f(x)|>\varepsilon\}.
$$

Splitting the integral gives

$$
C_q^q\leq\|f\|_q^q
\leq\varepsilon^{q-p}\|f\|_p^p+\int_A|f|^q
\leq\frac{C_q^q}{2}+\int_A|f|^q.
$$

For finite $r$, [Holder inequality](../../../../../../holder-inequality.md) bounds the last term by $\|f\|_r^q\mu(A)^{1-q/r}\leq C_r^q\mu(A)^{1-q/r}$. Hence

$$
\mu(A)\geq\left(\frac{C_q^q}{2C_r^q}\right)^{r/(r-q)}.
$$

For $r=\infty$, the corresponding bound is $\int_A|f|^q\leq C_r^q\mu(A)$. Thus an explicit choice proving the strict inequality is

$$
\boxed{M=
\begin{cases}
\frac12\left(C_q^q/(2C_r^q)\right)^{r/(r-q)},&r<\infty,\\
C_q^q/(4C_r^q),&r=\infty.
\end{cases}
\quad\mu\{|f|>\varepsilon\}>M.}
$$

This is a [nonvanishing level-set bound between three Lp norms](../../../../../../nonvanishing-level-set-bound-between-three-lp-norms.md): the lower-$p$ bound prevents diffuse low-amplitude mass, and the higher-$r$ bound prevents arbitrarily concentrated spikes.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 9](../../../paper-9-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
