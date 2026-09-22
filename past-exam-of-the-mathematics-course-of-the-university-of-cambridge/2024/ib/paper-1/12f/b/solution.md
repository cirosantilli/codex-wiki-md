<h1 id="12f/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write the Laurent expansion on the punctured disc as

$$
f(z)=\sum_{n=-\infty}^{\infty}a_nz^n.
$$

For every integer $k\geq1$, the Laurent coefficient formula and the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) give

$$
\begin{aligned}
|a_{-k}|
&=\left|\frac{r^k}{2\pi}
\int_0^{2\pi}f(re^{i\theta})e^{ik\theta}\,d\theta\right|\\
&\leq\frac{r^k}{2\pi}
\left(\int_0^{2\pi}|f(re^{i\theta})|^2d\theta\right)^{1/2}
\left(\int_0^{2\pi}1\,d\theta\right)^{1/2}\\
&\leq\frac{r^k}{\sqrt{2\pi}}.
\end{aligned}
$$

Letting $r\downarrow0$ shows that $a_{-k}=0$. Every coefficient in the principal part vanishes, so the [uniform L2 circle bound for a removable singularity](../../../../../../uniform-l2-circle-bound-for-a-removable-singularity.md) proves that

$$
\boxed{f\text{ has a removable singularity at }0}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [12F](../../12f.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
