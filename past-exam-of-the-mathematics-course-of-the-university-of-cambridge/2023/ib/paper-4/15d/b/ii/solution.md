<h1 id="15d/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Put $R=f e^{-\gamma r}$. Then

$$
R'=e^{-\gamma r}(f'-\gamma f),
\qquad
R''=e^{-\gamma r}(f''-2\gamma f'+\gamma^2f).
$$

After substitution and cancellation of the $\gamma^2f$ terms, the equation becomes

$$
rf''+(2-2\gamma r)f'+(\beta-2\gamma)f=0.
$$

For the [power series](../../../../../../../power-series.md) $f=\sum_{n=0}^{\infty}a_nr^n$, the coefficient of $r^{n-1}$ is

$$
n(n+1)a_n+(\beta-2\gamma n)a_{n-1}=0.
$$

Thus

$$
\boxed{a_n=\frac{2\gamma n-\beta}{n(n+1)}a_{n-1}}.
$$

If the series does not terminate, then $a_n/a_{n-1}\sim2\gamma/n$, so $f$ acquires the large-$r$ behaviour $e^{2\gamma r}$ and $R$ grows like $e^{\gamma r}$. Normalizability therefore requires termination, which occurs when

$$
2\gamma N-\beta=0
$$

for some positive integer $N$. Hence

$$
\gamma_N=\frac{\beta}{2N},
\qquad
E_N=-\frac{\hbar^2\gamma_N^2}{2m}
=-\frac{mq^4}{2\hbar^2N^2}.
$$

The ground state has $N=1$, so the [hydrogen ground-state energy](../../../../../../../hydrogen-ground-state-energy.md) is

$$
\boxed{E_1=-\frac{mq^4}{2\hbar^2}}.
$$

This is the [series-termination quantization of the Coulomb radial equation](../../../../../../../series-termination-quantization-of-the-coulomb-radial-equation.md).

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [15D](../../../15d.md)
4. [Paper 4](../../../../paper-4-split.md)
5. [Ib](../../../../split.md)
6. [2023](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
